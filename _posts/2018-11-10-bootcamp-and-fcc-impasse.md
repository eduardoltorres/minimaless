---
title: 'Bootcamp and fCC Impasse'
author: Eduardo
layout: post
permalink: /bootcamp-and-fcc-impasse/
categories:
  - Blog post
tags: studies
---
On Colt Steele’s The Web developer Bootcamp: completed the sections on Adding Authentication to YelpCamp, on Cleaning Up the code and part of the section on updating and deleting data (which is also in part related to authentication). At this point, I’m really not retaining much from the videos, I’m just aiming to finish the course as I’m just a couple of hours away. I’m definitely learning still, but I’ll definitely have to come back when dealing with the backend. Super excited to get to the Git and GitHub section (2 sections away); can’t wait to start contributing in GitHub.

On fCC: today I did encounter some challenges related to accessing nested objects and arrays. Nothing too fancy but glad I’m getting stuck as I really feel that that’s the way to learn coding and that that’s the life of the coder. Currently stuck—and happy to be—in a problem related to accessing an a nested array with a for loop.

This is the code (my code is the one between the commented lines that indicate so):
```javascript
//Setup
var contacts = [
  {
  "firstName": "Akira",
  "lastName": "Laine",
  "number": "0543236543",
  "likes": ["Pizza", "Coding", "Brownie Points"]
  },
  {
  "firstName": "Harry",
  "lastName": "Potter",
  "number": "0994372684",
  "likes": ["Hogwarts", "Magic", "Hagrid"]
  },
  {
  "firstName": "Sherlock",
  "lastName": "Holmes",
  "number": "0487345643",
  "likes": ["Intriguing Cases", "Violin"]
  },
  {
  "firstName": "Kristian",
  "lastName": "Vos",
  "number": "unknown",
  "likes": ["JavaScript", "Gaming", "Foxes"]
  }
];

function lookUpProfile(name, prop){
// Only change code below this line
  for (var i = 0; i < contacts.length; i++) {
    if (name == contacts[i].firstName && prop == contacts[i][prop]) {
      return contacts[i][prop];
    } else if (name !== contacts[i].firstName) {
      return "No such contact";
    } else if (name == contacts[i].firstName && prop !== contacts[i][prop]) {
      return "No such property";
    }
  }
  // Only change code above this line
}

// Change these values to test your function
lookUpProfile("Akira", "likes");
```
I still don’t get why this line doesn’t work...
```javascript
if (name == contacts[i].firstName && prop == contacts[i][prop]) {
  return contacts[i][prop];
}
```
...but this one does.
```javascript
if (name == contacts[i].firstName && contacts[i].hasOwnProperty(prop)) { 
  return contacts[i][prop]; 
}
```