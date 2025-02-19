![Insights Solution logo](./images/insights-solution.png)

# Insights Solution Issues, Announcements and Live Incidents 

This repository serves as a centralised location for tracking issues and announcements pertaining to the [Insights Solution](https://bmrs.elexon.co.uk/).

These include any part of Insights Solution:
 - the [Insights website](https://bmrs.elexon.co.uk/)
 - [Insights Real-Time Information Service (IRIS)](https://bmrs.elexon.co.uk/iris)
 - the [Insights API](https://bmrs.elexon.co.uk/api-documentation)

# Announcements and Incidents

Breaking changes to the Insights Solution and planned outages will be announced here.

## 2025-02-17 TLS 1.0 no longer supported by IRIS from 28 February 2025

As of 28 February 2025, TLS 1.0 and TLS 1.1 will no longer be supported by IRIS. The minimum TLS version will be 1.2.

IRIS users must check their client compatibility with TLS version 1.2 before this date.

For help configuring TLS for a client application, see [Azure documentation](https://learn.microsoft.com/en-us/azure/service-bus-messaging/transport-layer-security-configure-client-version).

## 2024-10-01 Deprecation of Generation Forecast summary endpoints

The following four endpoints are now all deprecated and will be removed in early 2025.
- `/generation/availability/summary/14D` (currently redirects to `/forecast/availability/summary/14D` below)
- `/generation/availability/summary/3YW` (currently redirects to `/forecast/availability/summary/3YW` below)
- `/forecast/availability/summary/14D`
- `/forecast/availability/summary/3YW`

Users should migrate over to using the following endpoints instead:
- [`forecast/availability/daily`](https://bmrs.elexon.co.uk/api-documentation/endpoint/forecast/availability/daily)
- [`forecast/availability/weekly`](https://bmrs.elexon.co.uk/api-documentation/endpoint/forecast/availability/weekly)

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
