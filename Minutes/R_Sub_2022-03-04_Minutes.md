## Minute R Submissions WG 2022-03-04

Compiled by Joseph Rickert

## Attendees:
* Michael Blanks - Beigene
* Phil Bowsher - RStudio 
* Bob Engle - Biogen
* Bella Feng - EQRx
* Miram Fossati - Merck
* Graeme Hickey - BD 
* Ryan Johnson - RStudio
* Christopher Kania - Biogen
* Ning Leng - Genentech
* Tadeusz Lewandowski - Roche 
* Eli Miller - Atorus
* Eric Nantz - Lilly 
* Joseph Rickert - R Consortium / RStudio
* Paul Schuette - FDA 
* Bryan Spells - FDA
* Jonathan Tisack - Beigene
* Nan Xiao - Merck 
* Hong Yan - Regeneron
* Renping Zhang - FDA 
* Yilong Zhang - Merck 

The meeting was recorded and the [video](
https://rstudio.zoom.us/rec/share/wcjMwWAnnqi_5DVOOgZ2hL1ssPlUsUnIbGSNVSwLr0ERWcKWMB1TWRDgTy3ECXU.JHDMBCOK8bg-yU4N) is available with Passcode: &G46ac&7

JR began the meeting by asking NL to update the group on the status of the recent submission of the adjudicated version of Pilot 1. NL noted that the content of the resubmission included:

* Fixing the table heading bug
* Addressing the rounding error that was due to using 1.96 in the calculation of a confidence as opposed to using the exact value
* Implementing some best practices that had been suggested by the FDA

NL also stated that although we heard back informally from the FDA, we have not yet received a formal reply. PS  confirmed that the FDA reviewer was able to open the submission and access the contents. PS stated that he would check with his supervisor to provide an update, and noted that the fact that we are still going through the test process and not through an actual submission, might account for the slow response.

JR asked BS if there was any channel we should use to communicate with the FDA when we had questions. BS suggested that sending an email to **edata@fda.hhs.gov** might be helpful.


NL then provided an update for Pilot which involves sending a `shiny` app through the gateway, but using the same data set and same analyses as used in Pilot 1.

* HY has begun programming the `shiny` app
* EN and EM are working on improving the formatting of tables in the `shiny` app
* The app will be published to a shiny.io server in order to get feedback from the WG
* EN is leading the effort to write the ADRG reviewers guide. A conversation has started in the issue tracker.
* Work is going well NL and EN believe that will have something to show in a month or so.

There was a short discussion on how much documentation the `shiny` app needs. EN and others stressed that the goal of this pilot is to prove the concept of passing the app through the gateway what is being planned will be more than sufficient.

JR asked if we have he bandwidth to begin thinking about Pilot 3. He stated that people who are discovering the WG are asking how they can get involved, and asked if there were certain task we could point them to and also are there any particular skill sets we need?

The WG thought that we do have the bandwidth to assimilate new members and run parallel tasks.

HY offered that she is in contact with colleagues who are working with the Japanese PMDA, and she should be able to have some information to share in Q2. She noted that the Japanese are beginning to accept R submissions.

The WG agreed that we should initiate new projects for Pilot 1 submissions for both Japan and China. We should stand up new repos for each of these projects and begin to sub teams to work on them in parallel with the other WG projects. 

JR asked if the technical approach we have taken with Pilot 1 for the FDA would work for Pilot 1 Japan. NL noted that we would Japanese and Chinese translation for all documents submitted to Japan and China respectively. However, the strategy of wrapping the R code into text for transmission, passing it through the gateway, and then unpacking it is appropriate. 

JR asked we need help researching container technology for Pilot 3. EN replied that he has already begun this research and his goal is to identify multiple orchestrators of container technology. He would like to have at least two potential solutions. [Singularity](https://sylabs.io/guides/3.5/user-guide/introduction.html) and [Rocker](https://www.rocker-project.org/) ar both possibilities.

EN agreed to put an issue into the main repo and stand up a Pilot 3 repo for the project details. JR noted that getting the folks behind the Rocker project would open up even more connections and opportunities to get help.

JR pointed out the as we progress further through the different projects we will need help writing blog posts and communicating what we have done. He then asked if anyone was planning to send a talk to [rstudio::conf](https://www.rstudio.com/conference/) which will happen in July or [useR! 2022](https://user2022.r-project.org/). NL offered that she has submitted to [SDSS](https://ww2.amstat.org/meetings/sdss/2022/) and would be happy to submit something similar to rstudio::conf. NL will start and issue to discuss upcoming projects.

EN offered to put a contact list on the website to organize people wishing to help.

NL noted that many of the WG members are also participating in [Shiny for Submissions Task Force](https://www.linkedin.com/posts/philip-bowsher-67151015_rpharma-activity-6879137760716886016-C-2Z/) and suggested we have a standing agenda to coordinate the two groups. 

The WG will next meet at 9AM Pacific Time on Friday, April 1, 2022.


