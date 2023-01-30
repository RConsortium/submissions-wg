## Minutes for R Submissions WG 2022-10-07
Compiled by Joseph Rickert (JBR)

### Attendees 

* Saghir Bashir -Argenx
* Phil Bowsher - RStudio
* Robert Devine - J&J 
* Miriam Fosatti - Merck
* Sean Healey - Pfizer
* Ellis Hughes - FSK
* Ryan Johnson Rstudio
* Ning Leng - Roche
* Tadeusz Lewandoski - Roche
* Qin Li
* Eric Nantz - Lilly
* Thomas Neitmann - Roche
* Sam Parmar - Lilly
* Joseph Rickert - R Consortium / RStudio
* Nan Xiao - Merck
* Renping Zhang - J&J
* Yilong Zhang
* Lei Zhao
* Jizu Zhi - FDA
* Honghong Zhou - Moderna


The meeting was recorded and the [video](https://rstudio.zoom.us/rec/share/OfSxaPPUsLuFJtZeUjzsZ6kZoAtCn7GTAj-N1j4zU9gUXOI8NqU5SUXf7rbeG2eu.q4s5o6ZiCBJHId8h?startTime=1665158653000) is available.

### Pilot 2 Submission
Ning began her update on the Pilot 2 Submission by thanking everyone who helped with the testing.

Status:
The submission package is ready. However, the submissions team must address some last minute comments from the FDA. One comment is a request to mask p-values that are automatically reported. The apparent concern is that by default p-values will automatically be updated and reported when users filter the data by subgroups. Because we only have a small test data set this will likely lead to widely varying p-values which could be misinterpreted by general reviewers who are not statisticians. The FDA may request additional outputs to me masked. These comments appear to address the long term use of interactive applications in submissions and are not related to the technical aspects of making the submission.

Consequently, the meeting scheduled for next Tuesday which was intended for submitting Pilot 2 will now be devoted to addressing FDA comments. The team will reschedule the submission as soon as possible after addressing the comments. We do not anticipate a long delay. There are no technical difficulties with masking additional default outputs.

In the meantime more testing would be helpful and appreciated.
Follow the instructions in the Appendix for Pilot 2: https://github.com/RConsortium/submissions-pilot2/issues/46
Put issues here: https://github.com/RConsortium/submissions-pilot2/issues/

JBR noted that there is now significant material in the GitHub repository for the working group which is indicative of the scope and scale of cooperation of the project. This is itself a success story of some interest. 

### Pilot 3 - ADaM 

(**13:51min** into the video) Thomas Neitmann presented a proposal by Joel Laxamana and himself to extend Pilot 1 to include ADaM datasets programmed in R. The purpose of the proposal is to:

1. Demonstrate the viability of using R for ADaM dataset creation in the context of an FDA submission
2. Provide the industry with an end-to-end example of an R-based FDA filing

Thomas' presentation may be found here: https://github.com/RConsortium/submissions-wg/tree/main/Documents

Yilong suggested taking ODM XML as the source to make it more representative of an end-to-end process. This started a discussion about the value of beginning end-to-end examples from various different starting file formats.

The present team team includes:

* Thomas Neitmann - Roche (Co-Lead)
* Joel Laxamana - Roche (Co-Lead)
* Lei Zhao - Roche
* Nicole Jones - Merck 

The team is looking for additional help. Please have a look at the presentation and contact one of the Co-Leads if you would like to get involved.

The working group agreed to change the name of the project from Pilot 1-ADaM Extension to Pilot 3-ADaM to emphasize that the project will include a significant amount of new work.

**Action Item** JBR will make Paul Schuette aware of this new project and ask for his feedback.


## DA Japan Talk

(**31:30** min into video)  Tadeusz presented a Shiny application that he developed for a presentation he is going to make at the [DIA Japan conference](https://www.diaglobal.org/en/conference-listing/meetings/2022/10/19th-dia-japan-annual-meeting-2022) on October 9, 2022. The intention of the presentation is to gauge the interest of the Japanese authorities. The session in which Tadeusz will present is called [LS09 Innovative and Dynamic Statistical Analytics for Regulatory Submissions](https://www.diaglobal.org/en/conference-listing/meetings/2022/10/19th-dia-japan-annual-meeting-2022/agenda/09/ls09?ref=LS09)

## Subgroups
The working group discussed writing writing some material for the GitHub repository explaining the purpose of the various subgroups, listing the members, and explaining how newcomers can get involved.

**Action Item** Joe and Eric will meet after the Pilot 2 submission to discuss documenting the subgroups.

## Containers

The working group agreed that the planned project to submit a containerized version of the Pilot 2 submission will require a significant amount of new work and pose several challenges. It should therefore be new, independent pilot submission, perhaps Pilot 4-Containers.

