![Insights Solution logo](./images/insights-solution.png)

# Insights Solution Issues, Announcements and Live Incidents 

This repository serves as a centralised location for tracking issues and announcements pertaining to the [Insights Solution](https://bmrs.elexon.co.uk/).

These include any part of Insights Solution:
 - the [Insights website](https://bmrs.elexon.co.uk/)
 - [Insights Real-Time Information Service (IRIS)](https://bmrs.elexon.co.uk/iris)
 - the [Insights API](https://bmrs.elexon.co.uk/api-documentation)

# Announcements and Incidents

Breaking changes to the Insights Solution and planned outages will be announced here.

## 2024-03-26 Planned outage

Planned infrastructure outage between 4:30 (GMT) to 17:30 (GMT) on Tuesday 26 March 2024 impacting upstream data sent to Insights. During the outage window Insights Platform will not be publishing data via IRIS, website and APIs.

## 2024-03-27 Breaking change to DISBSAD

We are releasing a breaking change to fix a discrepancy in the DISBSAD data schema between IRIS and the Insights API. IRIS previous returned `IsTendered` as a string with possible values `"Tendered"` or `"Non-tendered"`; after this release it will return a nullable boolean value, where `true` corresponds to `"Tendered"`.

# Issues

Issues should be raised wherever any functionality relating to the services doesn't work as expected; this could also include non-functional aspects e.g. performance. For any feature requests or improvement suggestions, please use the feedback form on the [Insights website](https://bmrs.elexon.co.uk/).

For any issues with [iris-clients](https://github.com/elexon-data/iris-clients), please raise an issue in that repository.

## How to raise an issue

*Before reporting an issue, please check the [issues page](https://github.com/elexon-data/insights-issues/issues) to see if it has already been reported. This helps to avoid duplicates, but please feel free to add a 👍🏽 reaction or provide a comment on the open issues thread.*

Create a report by [opening a new GitHub issue](https://github.com/elexon-data/insights-issues/issues/new?assignees=&labels=&projects=&template=issue-report.md&title=).

**Great Reports** include:

- A quick summary and required background context
- Steps to reproduce
  - Please be very specific!
  - Give screenshots or HTTP responses if relevant
- What you expected would happen
- What actually happens
- Notes - possibly including why you think this might be happening, or things you tried that didn't work

## Next steps

Once you have submitted your issue, someone from the Insights team will read it thoroughly and respond. Issues raised within this repository will be a key part of the backlog for fixes made to the Insights solution.

We recommend that you watch any issue that you wish to receive updates about.
