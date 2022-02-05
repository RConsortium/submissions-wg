## Minute R Submissions WG 2022-02-04

Compiled by Joseph Rickert

## Attendees:
* Michael Blanks - Beigene
* Phil Bowsher - RStudio 
* Gregory Chem - MSD
* Hey Soo Choo - FDA
* Heidi Curinckx - Johnson & Johnson 
* Bob Engle - Biogen
* Bella Feng - EQRx
* Miram Fossati - Merck
* Steven Hassendinckx 
* Graeme Hickey - BD 
* Ellis Hughes - GSK
* Ryan Johnson - RStudio
* Christopher Kania - Biogen
* Ning Leng - Genentech
* Tadeusz Lewandowski - Roche 
* Shannon Lewis - Beigene
* Michael Mayer - RStudio
* Eli Miller - Atorus
* Eric Nantz - Lilly 
* Emily Nguyen - FDA 
* Xin Qiu - JnJ
* Joseph Rickert - R Consortium / RStudio
* Paul Schuette - FDA 
* Jonathan Tisack - Beigene
* Shiva Kalyan Voruganti
* CG Wang  
* Nan Xiao - Merck 
* Jiang Xu - FDA 
* Hong Yan - Regeneron
* Renping Zhang - FDA 
* Yilong Zhang - Merck 
* Patruchi

The meeting was recorded and the [video](https://rstudio.zoom.us/rec/share/szar9nFQH0BF-BOn134TSLzfGH6n4VOJP8iibLdHnqgluDC7PAPn6C3sg0TiyLHg.b97ETbrhnfYgr3Wb?startTime=1643994263000) (Passcode: &nET4J?I) is available.

JR began the meeting and asked NL to give an overview of the GitHub repositories for the Submissions WG. Every submission will have two repositories: a development repo and a repo that follows the FDA ECTD structure that contains the files that will go through the gateway.  

* [submissions-wg](https://github.com/RConsortium/submissions-wg) is he umbrella repo that contains the [kanban board](https://github.com/RConsortium/submissions-wg/projects/2) for the project.
* [submissions-pilot1](https://github.com/RConsortium/submissions-pilot1) is the development repository for the Pilot 1 submission
* [submission-pilot1-to-fda](https://github.com/RConsortium/submissions-pilot1-to-fda) contains the only the files that will go to the FDA
* [submissions-pilot2](https://github.com/RConsortium/submissions-pilot2) is the development repo for Pilot 2
* [https://github.com/RConsortium/submissions-pilot2]

The group then summarized the present status of the project. The Pilot 1 submission of last year was mostly successful but the FDA response flagged a couple of problem areas:
* An apparent but the resulted in column labels being switched
* An unexplained rounding discrepancy in a p-value may be due to different operating systems.
* Several good practice issues to address

HSC who helped to conduct the FDA review of the Pilot 1 submission offered to share the code that flagged the rounding error. She will enter it as an issue on the submissions repo.

The Pilot 1 team has been working on the Pilot 1 resubmission. The team will will review the FDA code and test it on multiple operating systems. They expect to be able to resubmit in a couple of weeks. NL asked if HSC could look over the new code before they do so. Assuming that the resubmission goes well the group will prepare a blog for posting on the RC blog.

NL then reviewed plans of the Pilot 2 shiny submission. It is envisioned as a simple four tab Shiny app that contains the same analyses as the previous submission. The plan is to use the Roche teal framework because of its filtering structure. 

YZ then outlined work required to complete the Pilot 2 work and identified three dependencies:

1. teal must become open source
2. The scope of Pilot 2 needs to be clarified
3. A template needs to be developed for submission documentation that includes a Shiny app.

YZ recommended that a separate Pilot 2 documentation team be formed to work on the Shiny documentation in parallel with the code development for Pilot 2.

EN said that he had experience preparing this sort of documentation and agreed to lead the documentation task.

JR asked when teal would become open source and whether the fact that it is not now open source prohibiting other companies from contributing to the project. TL responded that project to open source teal is currently with the Roche lawyers and that he expects it will be complete within three months. No one present believed that not currently having teal as open source code was prohibiting participation. Everyone will be able to run the Shiny app from a public website. EN noted that work on infrastructure can proceed in parallel.

The team working on Pilot 2 said that a submission in Q2 is feasible.

Currently there are not plans for multiple Pilot 2 submissions. However, it is likely that we would want to have a submission in the future that includes a more complicated Shiny app. JR noted that it would be optimal if the FDA could provide guidance on what features they would like to see in a more robust Shiny app.

Moving beyond Shiny JR asked if by the end of the year we would be looking a submission based on container technology. EN remarked that that is the direction the group would like to see but since Docker is not suitable (because of licensing issues) it will be necessary to research alternative container technology.

JR noted that having 29 people in the meeting indicated that there was considerable industry interest in the work being done and whether it would be possible to recruit a team to do the research for long range projects. He asked group members who are not involved in immediate work to get involved in long term planning. EN noted that we definitely need to help from the regulatory side to help effect any changes that would have to be made to make use of container technology.

The discussion then turned to the possibility of making a submission to [CDE](https://credevo.com/articles/2021/02/25/china-drug-registration-process/) the Chinese health authority. (See issue [#62](https://github.com/RConsortium/submissions-wg/issues/62) ) They are trying their own submissions gateway. They have shared validation software with Roche that could check a submission. NL suggested that we undertake an effort to see if we could validate a test submission using the Chinese supplied software. If that worked the only additional work to be done to make a viable submission to the CDE would be to translate the documentation into Chinese. 

NL asked if anyone has contacts with the CDE that could review a test submission from the Submissions WG. JR asked EN if she could check with PS about possible FDA contacts with the CDE.

BF noted that her company, EQRx, has the opposite problem. They have had a compound approved by the CEA and now want to submit it to the FDA. She noted that there are high level regulations about the transfer of data between China and the FDA. The CDE has an HGR application that must be approved by the Human Genetic Resources Agency for China. HY offered that she has some experience dealing with the CDE, having done two or three submissions to the CED in the past when she worked for Novartis. At that time the CDE accepted the FDA package. 

The discussion they turned to other countries
HY noted that she is working on a submission to the Japanese [PMDA](https://www.pmda.go.jp/english/about-pmda/index.html) which the group aggreed is more strict than the CDE an offered to look for a contact there. 

YL noted that the German authorities have strict requirements about the table formats. 

JR asked if there is there is a European authority that we should have on our radar. Apparently, the EMA does not presently require a data submission, but that may be changing. TL noted that they have had a proof of concept sharing data with the EMA.

YL also raised the possibility of following the [PHUSE ADGR](https://advance.phuse.global/display/WEL/Analysis+Data+Reviewer%27s+Guide+%28ADRG%29+Package) template. He suggested that we contact PHUSE and ask if they would be willing to update the template so that it does not specify SAS data sets. JR agreed to look for a contact within PHUSE. We would want a language agnostic template.

NL noted that this would be a good time to revisit our effort to develop suggested language for section 14 ([issue #38](https://github.com/RConsortium/submissions-wg/issues/38)).

JR suggested that we need some high level planning document to capture all of the ideas presented.

At 47:10 in the video NL explains the contents of the Submission WG GI Hub sites.

### Some useful links from the chat box
R Consortium GitHub sites: https://github.com/RConsortium/

WG web page: https://rconsortium.github.io/submissions-wg/

Tracker for the pilot1 submission: https://github.com/RConsortium/submissions-pilot1-to-fda/issues

https://github.com/RConsortium/submissions-wg/issues/38

Issue filed for pilot 2 documentation : https://github.com/RConsortium/submissions-wg/issues/63

