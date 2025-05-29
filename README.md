# bmc-art
BMC Alliance Recruiting and Tracking: full lifecycle partner management from application to integrated solution marketing

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)

- [My process](#my-process)
  - [Built with](#built-with)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

My team and I managed hundreds of technology partners at BMC Software, coaching them to build integrations between their software and BMC's speeding their time to delivery with sample code, development environments, and more. I built Alliance Recruiting and Tracking (ART) in order to manage the partnership process more efficiently across the full alliance lifecycle:

- A streamlined, responsive application for partnership form (https://developer.bmc.com/ar/apply-isv.jsp) that mirrors the BMC corporate look and feel for a consistent user experience. The form was written in JSP, since we were already running an Apache Tomcat server. Data was saved to the ART system via Java API calls.
- ART is primary built on the BMC Helix ITSM (fka Remedy AR System) platform running on a Windows Server with MS SQL Server database.
- Application data saved onto ART and immediately acknowledged to the applicatnt.
- Applications are reviewed manually to avoid spam and then automatically sent for review via email to a wide-range of product managers and others for their feedback.
- Reviewers can provide input with an easy, no-login form that is saved and visible to the other reviewers.
- When approved, the relevant info (name, address, etc.) is sent to the contracts team for them to setup an e-sign in Ironclad. Unfortunately, BMC legal did not allow us to use Ironclad's API (https://clickwrap-developer.ironcladapp.com/).
- Once the partnership contract has been signed, ART is used to record the contract terms, dates, etc.
- The system was also integrated into the BMC Community site via REST API, in order to provide a partnership and integrated product directory. All directory details (name, description, URL, contact, logo, etc.) were stored in ART and pushed to the Community automatically. This gave us consistent formatting with updated links between pages without the need for partner managers to be CMS experts.
- Interested customers can download more details on partner integrations (https://developer.bmc.com/ar/inote.jsp), which automatically provides lead details to the partner and BMC sales.
- Built-in reporting provided easy access to full partner details for status updates and annual partnership renewals.

### Screenshot

![]([https://fiel.us/src/Screenshot-ISV.png])

## My process

### Built with

- BMC Helix ITSM platform (https://www.bmc.com/it-solutions/itsm.html)
- Jive social platform (https://www.jivesoftware.com/solutions/collaboration)
- Apache Tomcat (https://tomcat.apache.org)
- MS SQL Server (https://www.microsoft.com/en-us/sql-server)
- JSP pages, Java API, REST API

## Author

David Fiel

- Website - [David Fiel](https://fiel.us)

## Acknowledgments

Thanks to BMC Software for all the ongoing support to build and maintain the ART system, which made managing so many partnerships a much happier process.
