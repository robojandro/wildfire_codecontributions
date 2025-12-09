# Marco Palma's GitHub code contribution graphs while at WildFire

It's a shame that I can't go into much detail about what I actually implemented in the 3 years and 9 months that I spent at WildFire, but at least I had the forethought to take screen captures of my GitHub contributions graphs.

You can be sure that these weren't just a bunch of documentation and comments slapped into existing files.

That being said good documentation specially about how business logic is implemented is truly worth its weight in gold and sadly I didn't take snapshots about all the new docs I did publish to the wiki-like system we used there.

Regardless here is one way to gauge what I did affect while I was there:

## 2025

![Marco Palma's January and February of 2025 at Wildfire](mpalma_contributions_at_wildfire_feb2025_tall.png "January and February of 2025")

As I got busy with projects I neglected to keep taking screen shots, but had some very interesting work specially towards the latter part of 2025 updating Opensearch (an Apache-licensed fork of Elasticsearch) indexes.

A large part of 2024 was spent automating our partner billing system which previously lived as separate manual processes could take more than 24 hours to complete due to the volume of end user data that had to be processed.  The old way was problematic because it relied on humans to get all the steps executed correctly and to be able to maintain uninterrupted connections to production systems.

Obviously, this was less than optimal.  We managed to replace it with a new API wrapping the previous steps in several CRUD endpoints. Due to the execution running within the same network infrastructure as the database, the execution time was whittled down to 30 minutes.  More importantly, as a service, we now had proper logs and the rest of expected scaffolding that typical production systems are supposed to have.

## 2024

![Marco Palma's 2024 at Wildfire](mpalma_contributions_at_wildfire_2024.png "2024")

It's interesting to see the next 2 years line up around 620 contributions per year.

Given that there's ~260 working days a year, that works out to an average of 2.38 contributations per workday.

According to Google, [GitHub](https://docs.github.com/en/account-and-profile/reference/profile-contributions-reference)

    Key activities that count as contributions:

    **Commits:** Pushing commits to a repository's default branch (e.g., main or master) or gh-pages branch. The email address used for the commit must be linked to your GitHub account for it to be counted.

    **Pull Requests:** Opening a pull request or having a pull request you opened merged.

    **Pull Request Reviews:** Submitting a review on a pull request.

So PR reviews would seem to be a part of that and I do think one of my more important contributions at WF was making sure the code from the team kept flowing while at the same time not bring down quality. 

## 2023

![Marco Palma's 2023 at Wildfire](mpalma_contributions_at_wildfire_2023.png "2023")

After a few months at WF I noticed that our testing infrastructure was lacking when it came to the full life cycle of user transactions so I decided to go mildly rogue and put together a demo of how this could be done by using ephemeral databases.  Leveraging the database was a hard requirement because of the reliance on triggers which I did not want to simulate in mocks.

It helped that soon after I started developing this in my off hours, the company had a hackathon which gave me the time to polish up the proof-of-concept.  As of the writing of this document, those integration tests execute with every push of a branch to GitHub (thanks to the dedicated DevOps staff). Of all the things I worked on while at WF, this is probably what I'm proudest of.

## 2022

![Marco Palma's 2022 at Wildfire](mpalma_contributions_at_wildfire_2022.png "2022")

My first year kicked off with a bang.  Primarily addressing a backlog of tech debt resulting from the team having been small but then leading into work like our offer translation system which was a requirement to do business with partners needing to make sure that only offers available in all of a given countries official languages were present to end users.

