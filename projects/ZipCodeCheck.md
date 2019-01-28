---
layout: project
type: project
image: images/hawaii.jpg
title: ZipCode Check
permalink: projects/ZipCode Check
# All dates must be YYYY-MM-DD format!
date: 2017-11-30
labels:
  - Html
  - Atom
  - Zipcode
  - javascript
summary: An assignment for ICS 215 to get familiar with html notation. 
---

<img class="" src="">

This program takes in a zipcode and uses regular expressions to check if the zipcode is a valid Hawaii zipcode.
The program also implements the use of a checkbox to see if the user checked the box or not. Valid Hawaii Zipcodes are
967?? or 968??. The appropriate message is outputted if the user entered a valid zipcode or not.

By creating this program I became familiar with the use of script tags in html, so that I would be able to recognize where
the javascript was inserted into html. I also became familiar with manipulating html by using javascript.

Here is an example of the javascript function used to test zipcodes:

'''js
function checkHiZip(inputZipParam) {

      // HI ZIP codes are 968XX or 967XX.
      var hiZipRegex = /^96[78]\d\d$/;

      // The <p> used to output feedback to the user.
      var feedbackNode = document.getElementById("feedback");

      // Check if the user entered a HI ZIP code, output feedback in <p id="feedback">
      if (hiZipRegex.test(inputZipParam)) {
        feedbackNode.innerHTML = "Yes, that is a HI zip code";
      } else {
        feedbackNode.innerHTML = "No, that is NOT a HI zip code";
      }

    }
Source code provided on request.
