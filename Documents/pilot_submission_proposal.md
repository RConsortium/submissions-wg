R Pilot Submission for eCTD Compliance
================
Mike Stackhouse, Yilong Zhang
5/6/2021

## Problem Statement

Interest in R has been growing steadily over the last few years, and
several companies have their eyes set of producing a regulatory
submission with significant portions of the analysis written in R. While
we know that this is acceptable given the Statistical Software
Clarifying Statement, there are still several challenges to overcome.
Many initiatives across industry are focused on different aspects of
this challenge, including the R Validation Hub, PHUSE Clinical
Statistical Reporting in a Multilingual World, R Package Validation, the
R Consortium R for Regulatory submission, and the R Consortium R Tables
for Regulatory Submissions. Most of these initiatives focus on topics
like validation, production of expected outputs, and anticipated
questions that may arise when interfacing with a regulatory agency, but
one question relatively unexplored is the physical delivery of code to
the agency.

The FDA has strict submission guidelines within documents like Technical
Conformance Guide, and strict expectations of delivery format following
the eCTD. Aspects of these requirements can make the delivery of R code
non-trivial, particularly when it comes to R packages. Most R packages
exist in open-source, accessible through sources like GitHub or the
Comprehensive R Archive Network (CRAN), but it is inevitable that
sponsors submitting to the FDA will need a method of delivering a
package that cannot be generally accessible to the public. This project
will address this challenge in the context of a pilot submission.

## Problem Impact

This project has the potential to give a roadmap to submitting sponsors
actively working towards R submissions. Many questions about the process
of submitting R code to the FDA will be answered, and there is a large
potential to identify questions that must be explored in more detail.

## Problem Scope

Fortunately there is a solid foundation already in existense on which to
build this project:

-   [The PHUSE Test Data Factory project upversion of the CDISC Pilot
    Data](https://github.com/phuse-org/TestDataFactory/tree/main/Updated)
-   [The Atorus replication of the CDISC Pilot Project in
    R](https://github.com/atorus-research/CDISC_pilot_replication)
-   [Merck’s open-source R package
    pkglite](https://merck.github.io/pkglite/)

Atorus’ replication of the CDISC pilot gives us a baseline of code to
utilize as a starting place. This project replicated the original CDISC
pilot’s outputs, and thus gives a solid foundation of analysis programs
to submit as a test case.

Merck’s R package pkglite was specifically developed to enable the
delivery of an R package through the eCTD. This package is able to
package the code into a submittable format, and then unpack the code and
restore its state to an installable R package, enabling the agency to
utilize the delivered code as expected.

The goal of this project is to conduct a pilot submission using these
available tools. The CDISC pilot replication will be submitted, and an R
package will be delivered through the eCTD to evaluate if all compliance
checks relevant to the programs can be met.

The scope of this project is limited to evaluating the consumability of
the code. Rather than evaluate the entire submission package, we intend
to verify that: - The packaged code is compliant with the eCTD - A
consumer of the eCTD on the agency side is able to unpack and install
the delivered R package - A consumer of the eCTD on the agency side is
able to rerun the analaysis package delivered and replicate the results

Different questions may arise during this process, but those questions
will be left for further exploration in follow-ups to this project

This project is a good candidate for collaboration between PHUSE and the
R Consortium. With the R Consortium’s wealth of technical expertise, and
PHUSE’s experience with navigating regulatory agencies (including a
recent pilot submission within PHUSE’s [Best Practices for Interactive
Vizualiations](https://advance.phuse.global/display/WEL/Best+Practices+for+Interactive+Analysis+for+Decision+Making+Submissions)
project) and relationship with the FDA.

## Project Deliverable(s) and Timeline(s):

-   Submission of pilot \~6 months
-   White paper outlining the process and lessons learned \~ 10 months

## Tools Required/Planned to be Developed

Primary tools have been developed. Project requires a pilot submission
process through the eCTD, so need collaboration with FDA.

## Stakeholders:

Pharma, CRO, regulators, tech companies
