---
title: 'UGRC Voter Count Tool for Redrawing Precincts'
author:
  display_name: Erik Neemann
  email: eneemann@utah.gov
date: 2021-11-23 9:30:01
categories:
  - Featured
tags:
  - voting
  - tools
  - political
---

Utah's [statewide election districts](https://opendata.gis.utah.gov/search?q=election) have been released and many local governments are now in the process of redrawing their precincts to accommodate the changes and manage their upcoming elections.  To help facilitate these "precincting" efforts, UGRC has created an ArcGIS Pro tool that counts up the number of actively registered voters within a given polygon layer.  The primary use case for the tool is to help counties adjust precinct boundaries to optimize the number of voters within their precincts.  The tool can be run iteratively as precinct boundaries are adjusted to update voter counts and guide further adjustments.  The Python Script Tool resides within an ArcGIS Pro Toolbox that can be installed and run locally from your desktop computer.

[![Voter Counts in Precincts]({% link images/voter_counts.PNG %} "Voter Counts in Precincts")]({% link images/voter_counts.PNG %})
{: .flex .flex--center }
_Precincts with voter counts labeled_
{: .flex .flex--center}

Behind the scenes, the tool grabs voter count totals from a voter points layer in ArcGIS Online (AGOL).  This data has access restrictions placed on it, so only specific AGOL users or groups that have been granted permission, can access it.  This means that the user must be logged into AGOL from ArcGIS Pro in order for the tool to work correctly and to have access granted to the voter points layer.

The ArcGIS Pro Toolbox can be [downloaded](https://drive.google.com/file/d/1i9OZdYVBkDs-EeFu9JItVTk8rNCs1K0M/view?usp=sharing) by anyone and a [user guide](https://docs.google.com/document/d/1BG-FPROoZkfsoAScDLLSvHGMLuFucdlzaJRILp33rSk) has been created with information on installing and using the tool.  Additionally, we recorded a [UGRC Voting Tools](https://drive.google.com/file/d/1i6ZIwuJjlA0MXdaIxbQcsvUO8nTrkFqe/view) Webinar earlier this year that demonstrates the voter counts tool and data validation checks done by UGRC.

[![Voter Counts Tool]({% link images/voter_tool.PNG %} "Voter Counts Tool")]({% link images/voter_tool.PNG %}){: .flex .flex--center }

If you're interested in using the voter counts tool to help with redrawing your precincts, please reach out to us and we can help set you up.  {% capture contact %}{% include contact.html subject=page.title contact=site.data.contacts.voter_count_tool %}{% endcapture %}
{{ contact }}
