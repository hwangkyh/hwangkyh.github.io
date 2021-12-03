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

## General Problems Require General Solutions

What are design patterns? It's in the name really, design patterns are general solutions to general problems that have been developed for and by software developers through trial and error. The benefit of having design patterns is that they use standard terminology and provide solutions to different scenarios whilst also being the best option due to the long time and hours being poured into making design patterns. There are three main pattern types as defined by the Gang of Four: creational, structural, and behavioral. Diving in specifically to the behavioural pattern types, these largely deal with communication between objects. The iterator pattern is a behavioral pattern that is very commonly used to access elements by traversing containers sequentially without the need for the underlying representation. 

## Graphic Design Patterns are my Passion

<img class="ui floated image" align="center" src="../images/spotifygraphic.jpg" width="10%">

It's that time of the year when everyone who uses Spotify checks their Spotify Unwrapped and is presented with tasteful graphics of their music tastes over the last year. As much as I would love to express my personal distaste of 2021's graphic design choices (exemplified in the parody graphic on the left), this is not the reason I bring this up. The iterator pattern can be seen in media players such as Spotify, where in a playlist there is a list of songs of to choose from and I can select any one of them. By traversing through the playlist, I do not access the underlying representations of each song, i.e. album, artist, genre, but can still play a song of my choice.


## Final Design Pattern

```
const columns = [
  { name: 'Date', selector: row => row.date, sortable: true },
  { name: 'Time', selector: row => row.time, sortable: true },
  { name: 'Animal', selector: row => row.animal, sortable: true },
  { name: 'Name', selector: row => row.name, sortable: true },
  { name: 'Phone', selector: row => row.phone, sortable: true },
  { name: 'Location', selector: row => row.location, sortable: true },
  { name: 'Latitude', selector: row => row.latitude, sortable: true },
  { name: 'Longitude', selector: row => row.longitude, sortable: true },
  { name: 'Description', selector: row => row.description, sortable: true },
  { name: 'Image', selector: row => row.image, sortable: true },
  { name: 'Edit', selector: row => <Link to={`/edit/${row._id}`}>Edit</Link> },
];
```

For Bloombugs' final project for ICS314, we have been working on improving our [HACC application](https://bloombugs.github.io/). Due to the complexity of the application, we have implemented many different design patterns to concisely and effectively write the application. We specifically use the iterator pattern to represent the data collections of distress reports via a table. After users submit their distress reports, they are aggregated on a table that is only accessible to admin users. Here, the [DistressTable.jsx](https://github.com/bloombugs/application/blob/master/app/imports/ui/pages/DistressTable.jsx) page displays all of the distress reports submitted as a table by an iterator iterating over the collections in the database. There is the initial constructor of columns (as shown in the code snippet above) that populates a row with all of the variables of a single distress report, then the iterator (as shown in the code snippet below) iterates through all of the data that the admin can access (which code is in yet another file, modularity is winning) and displays each report in a row in the table.

```
export const DistressTable = (props) => {
  // eslint-disable-next-line
  const data = props.reports;
  const tableData = {
    columns,
    data,
  };
  return (
    <DataTableExtensions {...tableData}>
      <DataTable>
        columns={columns}
        data={data}
        noHeader
        pagination
      </DataTable>
    </DataTableExtensions>
  );
};
```

## Rinse and Repeat

And so, by using design patterns to succinctly write streamlined code, developers and readers alike are happy. Plus it makes debugging much easier as there is less quantity of code to sift through. I, for one, am glad that these design patterns exist and that the developers before me, through their blood, sweat, and tears, toiled away to arrive at these best practices. Of course this does not mean I can be complacent, I will try and successfully use design patterns throughout my body of work and who knows, maybe I'll join that gang to become a Gang of Five.
