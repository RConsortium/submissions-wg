## Minutes for R Submissions WG 2022-11-04
Compiled by Joseph Rickert (JBR)

### Attendees 

* Saghir Bashir -Argenx
* Gregory Chen
* HyeSoo Cho - FDA
* Robert Devine - J&J 
* Bob Engle
* Ellis Hughes - FSK
* Joel Laxamana
* Yutong Liu
* Ning Leng - Roche
* Tadeusz Lewandoski - Roche
* Stephanie Lussier
* Eric Nantz - Lilly
* Joseph Rickert - R Consortium / RStudio
* Heng Wang
* Nan Xiao - Merck
* Paul SCHUETTE
* Renping Zhang - J&J
* Yilong Zhang
* Lei Zhao
* Jizu Zhi - FDA
* Honghong Zhou - Moderna
* Lian
* Yiwen


The [video](https://www.youtube.com/watch?v=LDVWXgDhzzo) is available on the [R Consortium YouTube Channel](https://www.youtube.com/channel/UC_R5smHVXRYGhZYDJsnXTwg) 

The meeting began with EN summarizing his understanding of the comments made by PS about his preliminary look at the Pilot 2 submission package.

The following is a summary of Paul's comments which were made in a email exchange with the workgroup members on 10-27-22:

* Paul has management approval to proceed with Phase 2 of the pilot, with the proviso that the Demographic, Primary and Efficacy Tables are static.
* There is a minor error in the app: the low dose and high dose column settings reversed. 
* The efficacy table is slightly misleading as it currently stands. Suggest that the text for the first row read “Study Drug (High Dose)” or similar.
* Suggest an additional table: "Subjects Remaining in the Study" showing how dropouts proceed. (See Paul's email of 10-27-22 for details) This might show how exploratory analysis might add value over the prespecified
* The number of decimal places displayed in the demographic table isn’t always the same as in pilot 1. 
* Suggest that the model specification information be included with the efficacy table rather than left to the app information.  
* We would like the app to be able to serve as a model for future submissions.

Eric stated that the updates appear to be relatively minor and would not be difficult to accomplish.

The submission team agreed to target 11-18-2022 as the target submission date.

**Action:** JBR to put a 9AM 11-18-2022 on the calendar for the submission.

JBR asked Paul to describe the boundary between a useful amount and too much interactivity in a shiny submissions app. Paul replied that it a way to think about it would be the difference between exploratory and inferential analysis. The problem with inferential analysis is the usual problem with p-values, subgroups and cherry picking. Inferential analysis is not the way to go. A Kaplan-Meier curve would be considered an exploratory safety analysis.

When asked if the guidance on interactivity was likely to stand for some time or change with familiarity Paul replied that it was his personal opinion that since it is consistent with the [ASA Statement on p-values](https://www.amstat.org/asa/files/pdfs/p-valuestatement.pdf) it will probably stand.

Paul also remarked that interactivity facilitating pre-specified analyses would probably be fine.

The following links may be helpful with understanding potential problems with on subgroup analyses:

* [Alosh et al. (2015)](https://www.tandfonline.com/doi/full/10.1080/19466315.2015.1077726)
* [Alosh et al. (2016)](https://onlinelibrary.wiley.com/doi/full/10.1002/sim.7167)

Joel Laxamana gave an update on the Pilot 3 effort:

* The kickoff meeting for the team was held this past Wednesday
* There are 13 people on the team
* The goal of Pilot 3 is to duplicate Pilot 1 but also generate the ADaM data sets used for the TLGs in Pilot 1
* The idea is to start with the [STDM](https://www.cdisc.org/standards/foundational/sdtm) and show the traceability to [ADaM](https://www.cdisc.org/standards/foundational/adam)
* Pilot 3 will use the `admiral` package along with `tidyverse` packages.

**Action:** Joel will add this explanatory material to the Pilot 3 GitHub repo.

**Action:** Joel will send a list of Pilot 3 team members to be added to the invitation list for this meeting.

**Action:** The Pilot 3 team will submit a written proposal to the FDA describing the process of unpacking the submission and setting up for analysis. The target date is to have this proposal ready for the 12-02-2022 Submissions WG meeting.

Lei Zhao asked if it would be a problem submitting data in SAS in doing the analysis in R. In general there is no problem, however the FDA suggests using a limited number of tools and using standard tools to do any translations between formats. The FDA prefers using scripted languages as opposed to using a GUI.

Ning will be presented at the R/Pharma conference on Wednesday, November 9, 2022 at 11AM Eastern Time.
The next meeting of the regular meeting of the group will be at 9AM Pacific Time on Friday, December 2, 2022.
