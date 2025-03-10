+++
author = "Staff"
description = ""
title = "Research Data Storage"
date = "2020-02-03T10:08:29-05:00"
draft = false
tags = ["storage","security","ivy","rivanna","project","standard"]
categories = ["userinfo"]
images = [""]
aliases = [ "/storage" ]
+++

![Project Storage](https://img.shields.io/badge/dynamic/json?color=color&label=Research%20Project%20Storage&query=message&url=https%3A%2F%2Ftja4lfp3da.execute-api.us-east-1.amazonaws.com%2Fapi%2Fbadge%2Fproject&style=for-the-badge)
![Standard Storage](https://img.shields.io/badge/dynamic/json?color=color&label=Research%20Standard%20Storage&query=message&url=https%3A%2F%2Ftja4lfp3da.execute-api.us-east-1.amazonaws.com%2Fapi%2Fbadge%2Fstandard&style=for-the-badge)

<p class="lead">There are a variety of options for storing large-scale research data at UVA. Public and internal use data storage systems can be accessed from the <a href="/userinfo/rivanna/overview/">Rivanna</a> high performance computing system. Sensitive and highly sensitive data can be stored and accessed within the <a href="/userinfo/ivy/overview">Ivy</a> secure computing environment. Information Security at UVA provides an overview of the <a href=https://security.virginia.edu/university-data-protection-standards>data sensitivity classifications</a>.  <br /><br />UVA graduate and undergraduate students are not permitted to request storage accounts. This must be done by their faculty advisor[s].</p>


{{< highlight >}}
  Information Technology Services (ITS) also provides <a href="https://virginia.service-now.com/its?id=kb_article&sys_id=2ca18093db7ac744f032f1f51d9619eb" target="_new"><b>multiple tiers of data storage</b></a> for personal and non-research storage needs.</alert>
{{< /highlight >}}


<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;border-color:#ccc;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:0px;overflow:hidden;word-break:normal;border-color:#ccc;color:#333;background-color:#fff;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:0px;overflow:hidden;word-break:normal;border-color:#ccc;color:#333;background-color:#f0f0f0;}
.tg .tg-hy9w{background-color:#eceeef;border-color:inherit;vertical-align:top}
.tg .tg-dc35{background-color:#f9f9f9;border-color:inherit;vertical-align:top}
.tg .tg-0qmj{font-weight:bold;background-color:#eceeef;border-color:inherit;vertical-align:top}
</style>

- - -

# Public & Internal Use Data Storage

**Public data** are intentionally made available to the public. Examples of public data in research computing include: 

- Data intended for a public website
- Datasets downloaded obtained from a publicly available source
- Open source code

**Internal use data** are classified as public records available to anyone in accordance with the Virginia Freedom of Information Act (FOIA) but are not intentionally made public. Examples of internal use data within a research computing context include but are not limited to: 

- Files collected or generated from experiments that contain no personally identifying information (PII) or otherwise protected information
- Models, scripts, and logfiles
- Preliminary analyses

<table class="table table-striped table-sm" style="font-size:90%;">
  <thead class="thead-dark">
  <tr>
    <th class="" style="width:16%;">Feature</th>
    <th class=""><a href="/userinfo/storage/non-sensitive-data/#research-project-storage">Research Project Storage<br>(currently unavailable)</a></th>
    <th class=""><a href="/userinfo/storage/research-standard">Research Standard Storage</a></th>
  </tr>
  </thead>
  <tbody>
  <tr>
    <td class="">Quota</td>
    <td class="">1TB increments</td>
    <td class="">1TB increments</td>
  </tr>
  <tr>
    <td class="">Price</td>
    <td class="">{{% storage-pricing project %}}/TB/yr</td>
    <td class="">{{% storage-pricing standard %}}/TB/yr</td>
  </tr>
  <tr>
    <td class="">Snapshots</td>
    <td class="">{{% backup-policy project %}}</td>
    <td class="">No</td>
  </tr>
  <tr>
    <td class="">Replication</td>
    <td class="">No</td>
    <td class="">No</td>
  </tr>
  <tr>
    <td class="">Backup</td>
    <td class="">No</td>
    <td class="">No</td>
  </tr>
  <tr>
    <td class="">Access</td>
    <td class="">Rivanna, <a href="/userinfo/howtos/storage/drive-mapping/">mountable on local workstation</a></td>
    <td class="">Rivanna, <a href="/userinfo/howtos/storage/drive-mapping/">mountable on local workstation</a></td>
  </tr>
  <tr>
    <td class="">Use cases</td>
    <td class="">Ideal for long-term storage of data to be accessed from Rivanna. Research Project storage is ideal for sharing data within a research group and for running jobs with smaller files.</td>
    <td class="">Budget solution for storing data that can be accessed by a personal computer or Rivanna. It is not recommended to run Slurm jobs against research standard storage unless absolutely necessary. File operations on Research Standard storage are slower than on Rivanna <code>/home</code>, <code>/scratch</code>, or <code>Research Project</code> storage.</td>
  </tr>
  </tbody>
</table>


- - -

# Sensitive & Highly Sensitive Data Storage

**Highly sensitive data** are data that require restrictions on access under the law or that may be protected from release in accordance with applicable law or regulation. Highly sensitive data (HSD) currently include personal information that can lead to identity theft. HSD also include health information that reveals an individual's health condition and/or medical history. Examples of HSD include, but are not limited to: 

- Personally identifying information (PII) such as social security number, passport number, driver's license number, military identification number
- Information defined by the Health Insurance Portability and Accountability Act (HIPAA) as protected health information (PHI)
- Cardholder data (CHD) such as credit card numbers, primary cardholder account numbers, cardholder names, expiration date, and/or service code

**Sensitive data** is the default classification for all data that is not explicitly defined as highly sensitive data, may be held from release under FOIA, or that is not intended to be made publicly available. Examples of sensitive data include:

- University ID numbers
- FERPA-protected student information not covered by the definition of highly sensitive data
- Personnel and financial information not covered by the definition of highly sensitive data, but not intended to be public
- Any information that doesn't fit into the other three categories

<table class="table table-striped table-sm" style="font-size:90%;">
  <thead class="thead-dark">
  <tr>
    <th class="" style="width:16%;">Feature</th>
    <th class=""><a href="/userinfo/storage/sensitive-data/#ivy-central-storage">Ivy Central Storage (ICS)</a></th>
  </tr>
  </thead>
  <tbody>
  <tr>
    <td class="">Quota</td>
    <td class="">1TB increments</td>
  </tr>
  <tr>
    <td class="">Price</td>
    <td class="">{{% storage-pricing ivy %}}/TB/yr</td>
  </tr>
  <tr>
    <td class="">Snapshots</td>
    <td class="">No</td>
  </tr>
  <tr>
    <td class="">Replication</td>
    <td class="">No</td>
  </tr>
  <tr>
    <td class="">Backup</td>
    <td class="">No</td>
  </tr>
  <tr>
    <td class="">Access</td>
    <td class="">Ivy Virtual Machine</td>
  </tr>
  <tr>
    <td class="">Use cases</td>
    <td class="">Ideal for long-term storage of highly sensitive data and is suitable for computation with smaller file sizes. Files stored in ICS are read-write only.</td>
  </tr>
  </tbody>
</table>

Researchers who request space on ICS must first request an Ivy account using the [Ivy request form](https://services.rc.virginia.edu/ivyvm). Further information on Ivy and the ICS can be found [here](/userinfo/storage/sensitive-data/#ivy-central-storage).

Ivy Central Storage is accessible by using [Globus](/userinfo/globus/) and connecting to the Ivy DTN.

- - -

# Request Storage

Storage requests can be made via this form:

[<button class="btn btn-success">Request / Purchase Storage</button>](/form/storage/)
