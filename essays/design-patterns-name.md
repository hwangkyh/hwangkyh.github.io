---
layout: essay
type: essay
title: It's In The Name, Design Patterns
# All dates must be YYYY-MM-DD format!
date: 2021-12-02
labels:
  - Software Engineering
  - Design Patterns
  - Final Project
  - Meteor
---

## Patterns for Design

What are design patterns? It's in the name really, design patterns are general solutions to general problems that have been developed for and by software developers through trial and error. The benefit of having design patterns is that they use standard terminology and provide solutions to different scenarios whilst also being the best option due to the long time and hours being poured into making design patterns. There are three main pattern types as defined by the Gang of Four: creational, structural, and behavioral. Diving in specifically to the behavioural pattern types, these largely deal with communication between objects. The iterator pattern is a behavioral pattern that is very commonly used to access elements by traversing containers sequentially without the need for the underlying representation. 

## Graphic Design Patterns are my Passion

<img class="ui floated image" align="center" src="../images/spotifygraphic.jpg" width="25%">

It's that time of the year when everyone who uses Spotify checks their Spotify Unwrapped and is presented with tasteful graphics of their music tastes over the last year. As much as I would love to express my personal distaste of 2021's graphic design choices (exemplified in the parody graphic on the left), this is not the reason I bring this up. The iterator pattern can be seen in media players such as Spotify, where in a playlist there is a list of songs of to choose from and I can select any one of them. By traversing through the playlist, I do not access the underlying representations of each song, i.e. album, artist, genre, but can still play a song of my choice.


## Final Design Pattern

For Bloombugs' final project for ICS314, we have been working on improving our [HACC application](https://bloombugs.github.io/). Due to the complexity of the application, we have implemented many different design patterns to concisely and effectively write the application. We specifically use the iterator pattern to represent the data collections of distress reports via a table. After users submit their distress reports, they are aggregated on a table that is only accessible to admin users. Here, the [DistressTable.jsx](https://github.com/bloombugs/application/blob/master/app/imports/ui/pages/DistressTable.jsx) file

