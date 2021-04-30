# splunk-dmc-dashboards
This repo contains several useful Splunk dashboards that I have developed over the years.

## Deployment Clients
Useful for environments with multiple deployment servers.  It steals liberally from Splunk monitoring console code (api calls, macros, and fields) putting them together in a way that makes it easier to find info about deployment clients quickly.

Requires permissions for the following macros in the splunk_monitoring_console app be set to global:
- dmc_rename_forwarder_type

## UF Troubleshooting
Extends where the previous one leaves off, assisting with doing detailed investigations into individual UFs to find things that need to be fixed like duplicate hostnames/GUIDs (poorly implemented imaging with the UF) or get details on the indexes/sources/sourcetypes a host is sending.

Requires permissions for the following macros in the splunk_monitoring_console app be set to global:
- dmc_get_forwarder_tcpin macro
- dmc_set_index_internal

## Index Checker
Queries for a list of all indexes in your environment and then allows you to view quick details of each one: sourcetypes, hostnames, sources, and earliest/latest data for each.

## Data Parsing
Looks for parsing issues for lines too long and events with too many lines and has drilldowns to examine these errors in detail.
