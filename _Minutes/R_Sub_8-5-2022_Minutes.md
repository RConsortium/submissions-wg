## Minutes for R Submissions WG 2022-08-05
Compiled by Joseph Rickert (JBR)

### Attendees 

* Saghir Bashir -Argenx
* Gabriel Becker
* Robert Devine - J&J 
* Sean Healey - Pfizer
* Ning Leng - Roche
* Eric Nantz - Lilly
* Xin Qiu J&J
* Joseph Rickert - R Consortium / RStudio
* Paul Schuette - FDA
* Henry Wang - Genetech
* Dadong Zhang - Illuminia
* Renping Zhang - J&J
* Yilong Zhang


The meeting was recorded and the [video](https://rstudio.zoom.us/rec/share/LUb3xNKOTGzzC3kzAmElw-ye0vvdcvalqDV9oRpEUaIHjaHzUdb9gBORXxhYjRPi.7jbqiKpboFOHCHpH) with passcode: wW@9+Lbx

NL asked if the R Consortium could establish an RStudio connect server to host the Pilot 2 Shiny submission App which is currently deployed on a Genentech server (https://genentech.shinyapps.io/FDA-app/). 

**Action Item**: JR will contact RStudio to see what it would take to set up the server.

NL and EN reported that the Pilot 2 team is in the final stages of preparation. The team recently set up Pilot 2 on the [`golem`](https://thinkr-open.github.io/golem/) framework. `teal` has been fully incorporated, and the team is in the finals stages of completing the documentation preparing the submission. NL estimates that a submission in mid August is possible.

**Action Item**: JR will connect with James Black to determine how Roche wants to announce the open sourcing of `teal`.

JR asked for updates from the efforts to make pilot submissions to the authorities in Japan and China. Based on conversations with her Roche colleagues, NL reported that there have be no new developments. The Japanese agency doubts that they have the resources to evaluate a pilot submission. The Chinese authority still appears to be interested in an industry collaboration. Roche China is attempting to form a working group, Ning offered to put anyone interested in touch with here Chinese colleague leading this effort.

JR asked: under the assumption that Pilot 2 goes really well, does the WG have any concrete suggestions for advancing the use of Shiny in submissions. EN noted that just getting Shiny in the process is a big step.

There was some discussion about the target audience for the Pilot 2 submission, and how the Shiny app might appeal to a larger FDA audience than the statisticians who would review a submission. 

There was a questions about whether FDA reviewers would want to reproduce the Shiny app interactivity. PS noted that FDA reviewers are not Shiny app developers and it is unlikely that the FDA would want to go down that path. GB asked for clarity on the term "independent reproducibility". PS noted that running the sponsors code in the same environment used by the sponsor is not considered to be independent verification.

NL asked about specific use cases that may be of interest to the FDA. PS noted that standing up a Shiny app in a real product submission workflow would be more complicated than one might expect because it would have to be integrated into an FDA contractor's workflow. Using the current infrastructure, it is best to think of a Shiny app being run on an individual's computer.

The discussion turned to the use of containers for submissions. JR asked PS whether about the FDA landscape for containers. PS replied that currently [podman](https://podman.io/) has been approved by NCTR, and that if we would like to use that he would have to get approval for [CDAR](https://www.fda.gov/about-fda/center-drug-evaluation-and-research-cder/cder-offices-and-divisions) use. Docker is not viable in the short term because of the subscription model, which would require coordination among multiple offices.

ER noted that in addition to podman and Docker he had identified singularity as a possible candidate container technology, but that this product is not as accessible to developers. In his organization, singularity requires an IT administrator to setup. PS noted that if this working group would identify a preferred container technology, he could begin promoting our choice within the FDA.

YZ asked if we should think about writing up the Pilot 1 and Pilot 2 experience for a journal publication, perhaps a two page letter. The group liked the idea and suggested R journal, ASA Journals, Significance, Chance, DIA Journals, JSS, JAMA and a clinical trials journal were suggested as possibilities.

NL asked about the possibility of presenting to FDA statisticians. PS said that he would have to consult with FDA management. 

PS suggested something like the recent R Adoption Series Webinar which drew 600 people from industry would be viable. He would invite members of the internal FDA Statistics Association to attend. He suggested a discussion / capstone effort: "Working through the R Consortium industry and the FDA have collaborated with industry in an appropriate way and gone through a step by step process that has involved the FDA at each step.

**Action Item** JR and NL to arrange this webinar.

Next the grouped discussed whether it would be worthwhile to do an additional pilot that would include data generation. The idea would be to start with [CDISC SDTM](https://www.cdisc.org/standards/foundational/sdtm) data and derive the data for analysis such as change from baseline etc. PS said that this would be interesting, but that most reviewers start with the analysis data steps. More motivated reviewers will trace key variables to show that they can be independently reproduced. No decision was reached on this matter.

PS suggested that the WG consider participating in the [CDISC TFL Designer Virtual Workshop](https://www.cdisc.org/events/webinar/tfl-designer-virtual-workshop) which will be held on 13 September 2022, 11am - 2pm Eastern Time. [Register Here](https://cdisc.zoom.us/webinar/register/WN__4u86BaeQImcA-U5tJ1pyQ).

**Action Item** The group will try to find someone from CDISC who may involved and also search for someone from the working group who might want to attend. JR will write to James Black to see if he has any knowledge of the event.

The next meeting of the working group will be at 9AM Pacific Time on Friday, September 2, 2022.
