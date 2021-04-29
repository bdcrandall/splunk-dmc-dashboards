# splunk-dmc-dashboards
This repo contains several useful Splunk dashboards that I have developed over the years.

## Deployment Clients
This dashboard is useful for environments with multiple deployment servers.  It steals liberally from Splunk monitoring console code (api calls, macros, and fields) putting them together in a way that makes it easier to find info about deployment clients quickly.

## UF Troubleshooting
This dashboard extends where the previous one leaves off, assisting with doing detailed investigations into individual UFs to find things that need to be fixed like duplicate hostnames/GUIDs (poorly implemented imaging with the UF) or get details on the indexes/sources/sourcetypes a host is sending.

## Index Checker
This is a simple one that queries for a list of all indexes in your environment and then allows you to view quick details of each one: sourcetypes, hostnames, sources, and earliest/latest data for each.
