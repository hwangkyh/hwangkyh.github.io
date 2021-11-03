---
layout: essay
type: essay
title: Final Project Idea
# All dates must be YYYY-MM-DD format!
date: 2021-11-02
labels:
  - Software Engineering
  - Meteor
  - HACC
---

## HACC Team
[Jacob Hardy](https://jakehardy95.github.io/), [Kelly Hwang](https://hwangkyh.github.io/), [Kiana Walters](https://kianaleilani.github.io/), [Kylie Higashionna](https://kyliehigashionna.github.io/), [Taryn Takebayashi](https://microtaryn.github.io/)


## Overview

For [HACC 2021](https://hacc.hawaii.gov/), we decided to ​choose the challenge proposed by NIC Hawaii, the [Hawaii Marine Animal Response (HMAR) Sighting & Reporting App](https://hacc.hawaii.gov/wp-content/uploads/2021/10/NIC_Challenge-Submission-Form_2021.pdf). Currently HMAR handles all animal sighting reports by phone. HMAR and NIC mentioned that they would like to have the ability to handle reports via an application as well - to decrease the amount of phone traffic and confusion as well as make it easier to record each sighting.

Our solution for HMAR HACC’s problem is twofold: one application for the mobile user who is the public or volunteers reporting animal sightings on the go, and another for the desktop user who is the HMAR staff that is managing the sighting reports database. We are using Microsoft’s Azure Portal to host our database, which we built using MySQL. The webpages are served out by Apache and we are using PHP to provide the middleware and the front-end. For our mobile application, we are using Cordova.

Since the final project requirements for ICS 314 do not directly align with our choices of software (i.e. database, server) for the HACC competition, we are creating a new application with similar functionality but with the 314 tech stack. For our 314 project, we are condensing our web and mobile applications into one application that will use Meteor and React/Semantic UI. Our 314 app will not be specifically designed for the mobile user, but it will be formatted so that the content and forms are still user-friendly when viewed from the mobile. We will use Node.js and Express to serve out our webpages, Mongoose to connect our pages to our backend database built with MongoDB, and a Droplet on Digital Ocean to host our 314 application.


## ICS 314 Tech Stack
The following technologies will be used for the 314 app of our HMAR app:
* Digital Ocean
* ESLint
* GitHub
* IDPM (Issue Driven Project Management)
* Javascript
* Meteor
* Mongo
* Semantic UI/React


## Mockup Page Ideas

The landing page will have basic information about the entire application, similar to Digits, and give a brief introduction to HMAR alongside links, FAQs, and contact numbers, which will possibly be located in a footer. To access any further functionalities for both public and admin users, there will be sign in and sign up pages that are accessible from the header. Upon signing up, the user will then be signed in to fill in a basic profile which will only be triggered for first sign in, any additional edits will also be permissible. Ultimately, to decrease spam and streamline reporting, possible e-mail or phone verification would also be introduced at this step.

For the desktop public user, upon signing in, the public user landing page will ask them to select the option of reporting either an “Animal in Distress” or an “Animal Sighting”, and if the public user does not know what would classify as an animal in distress, there will also be a “Click for More Information” button as well. These three different buttons will direct the public user to different pages. The page that is directed from “Animal in Distress” will first encourage them to call the HMAR phone number as well as have them fill out a form about the animal. It will ask the user to input the date, location, type of animal, and possible distress it is in. The page that is directed from “Animal Sighting” will show them the form, that is similar to the “Animal is Distress” form, which will ask for the date, location, and type of animal. The “Click for More Information” button will direct them to a page that shows multiple photos of animals that are in distress and explicitly state the reasonings they are distressed under the photos. This page will also have a button called “Return to Home Page” which will allow the user to go back to the public landing page.

For the desktop admin user, upon signing in, the admin user landing page will have two options of “Enter a New Report” for when the desktop admin user receives a phone call about an animal in distress or animal sighting and needs to log it, or “Look at Records” to see past and current reports. The page from “Enter a New Report” will be the same as the public user landing page with options of “Animal is Distress”, “Animal Sighting”, and “Click for More Information”, where these buttons will direct the user to the same pages as noted in the previous paragraph. The “Look at Records” button will direct them to a page which will show a database table that lists the information of submission such as the data, location, type of animal, and any notes of distress from most recent to old. This page will also have a “Return to Home Page” button which will allow the user to go back to the admin user landing page.

Mockup pages:
* Landing page
* Sign in page
* Sign up page
* Profile edit page
* Public user landing page (same as admin user "Enter a New Report" page)
* "Animal in Distress" page
* "Animal Sighting" page
* "Click for More Information" page
* Admin user landing page
* "Look at Records" page


## Use Case Ideas

As mentioned above, there will be two types of users: “public” users and “office” admin users. As the original HACC app was developed into two different apps, one for the public to report sightings and the other for the office admins to access reported sightings but also be able to report it themselves, the 314 app will integrate both apps into one app.


## Beyond the Basics

For the admin user “Look at Records” page, the different fields of data would be initially organized by date from most recent to old. To increase functionality, the table will be able to be sorted according to different filters and sorts, so that the admin user can see by date, location, type of animal, and be able to search for specific keywords under the different distress categories.

To standardize the date, time, and locations across all users, we will be using the jQuery datepicker and timepicker to make the date and time entry format easy for the user, and a clickable SVG map that lets the user select the location of the sighting. The clickable SVG map will auto populate the location field with the longitude and latitude GPS coordinates of the selected beach.

Due to the presumed success of standardizing location by using the clickable SVG map, we also plan to make clickable graphics wherever applicable to standardize sighting information as much as possible to relieve HMAR staff from having to manually group together similar or filter database entries. For example, the HMAR staff is interested in knowing if Hawaiian Monk Seals have any identifying markings as this helps them track if a seal is getting injured or sick often during a given time period. By providing a clickable graphic of a monk seal, both a top view and bottom view, users will be able to easily click on where they see scars or identifying tags on the animal.

Since many seabird species are similar in appearance, often varying shades of gray with black and white, we also plan on either 1) using clickable pictures of seabirds when the user is filling in a report for the seabird, or 2) linking to and/or embedding a page with example photos of the different seabirds that HMAR monitors. This feature will be useful especially for the public or layperson that may not be as familiar with what each species of seabird looks like.

The “Click for More Information” page, a button available on the public user landing page, is a page that describes what an animal in distress looks like. It can sometimes be hard to determine what would be categorized as a reportable distress, so with having multiple pictures and descriptions on what counts as distress, users will have an easier time knowing whether to choose between reporting a “Animal is Distress” or “Animal Sighting”.


## Schedule

Final Project, F Nov 12 - F Dec 10
* Final Project Milestone 1, Nov 18
  * Combine HACC apps by using 314 tech stack
* Final Project Milestone 2, Nov 30
  * Add users / admin functionality
* Final Project Milestone 3, Dec 09
  * Polishing, database filtering, optimizing for all devices
