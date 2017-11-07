# Table of contents

* [About OpenHRS](#about-openhrs)
  * [Inspiration](#inspiration)
* [What we built](#what-we-built)
* [Running the app](#running-the-app)
  * [Search](#search)
  * [Browse](#browse)
  * [Taking a pic](#taking-a-pic)
  * [Searching nearby Laws](#searching-nearby-laws)
* [Installation](#installation)
* [About OpenHRS development](#about-openhrs-development)
  * [Milestone 1: Updated Scraper and Code Cleanup](#milestone-1:-updated-scraper-and-code-cleanup)

# About OpenHRS

[![youtube](http://img.youtube.com/vi/ysAzR5RSkQk/0.jpg)](http://www.youtube.com/watch?v=ysAzR5RSkQk)

OpenHRS is the forward looking iteration of HRS App, a second place winning submission for the Hawaii Code Challenge 2017. The HRS App has been opened, in many different respects, to be improved by not only its original four developers, but by the community it was designed for. The opening of our original HRS App was the logical next step to keep it self sustaining. The HRS App was developed to effectively search the current Hawaii Revised Statutes in a way that was new and innovative. But innovation is finite if the technology behind it is restricted to a small group of students, and thus it has evolved into OpenHRS.

OpenHRS takes into account the following issues:

* Can't effectively search the current HRS.
* Can't find cross references in the HRS.
* Difficult to search for statutes located on signs around Hawaii.
* Not knowing what laws are relevant to your location.
* Having to note down laws you reference daily.

## Inspiration
Our inspiration comes from our core belief that “boring” subjects aren’t destined to be boring, but are misrepresented and unimaginatively produced. When designed with creativity, anything can be fun, interesting, and yet still as enlightening.

Rather than taking the easy route and creating a basic search and browse, we thought outside the box and added additional but necessary features in hopes that it’d help modernize the way the people of Hawaii build software in the future

# What we built
We created a powerful retrieval system for Hawaii’s laws built upon the latest human computer interaction principles and mobile design patterns. What you might expect from our app is countless directories of laws to navigate through, but instead you are presented with an app elegantly designed and engineered to enhance your exploration through thousands of laws waiting to be discovered.

Some issues that the current Hawaii Revised Statutes has include:

* No database for nearly 20,000 statutes
* Can't effectively search the current HRS site.
* Can't find cross references in the HRS site.
* Difficult to search for statutes located on signs around Hawaii.
* Not knowing what laws are relevant to your location.
* Having to note down laws you would like to reference in the future.

To combat those issues, we implemented:

* MongoDB database, with the future in mind for scalability.
* An organized RESTful API to allow anyone to interpret our statute data.
* Gorgeous, streamlined, user-friendly User Interface.
* State of the art search engine.
* Optical Character Recognition (OCR) system to allow a user to take a picture of a physical sign and receive the relevant statute.
* Statute locations near the user for extra awareness.

# Running the app
After opening the app, you are first welcomed with the homepage:

![homepage](./docs/photos/homepage.png)

From there, you are able to do a general search, browse the HRS, take a picture, or search nearby laws.
## Search
Using search is very easy. Just type in a term you are looking for, a chapter, section, or both chapter and section. The search engine will do its best to return the closest results.

Here's an example:

![search](./docs/photos/search.png)

![search_results](./docs/photos/search_results.png)

Searching for 'speeding' yields results related to speeding.

## Browse
When opening browse, you will reveal the list of divisions within the HRS.

![browse_main](./docs/photos/browse_main.png)

From there, you can browse through the divisions, titles, chapters, and sections.

Here is what a section may look like

![browse_section](./docs/photos/browse_sections_1-1.png)

Here, you can see the information about the statute.

In some sections, you may see a cross reference to another statute like this.

![cross_reference_select](./docs/photos/cross_reference_select.png)

You can select it to reveal information about it as well.

![cross_reference_result](./docs/photos/cross_reference_result.png)
## Taking a Pic
This feature allows the user to quickly snap a photo on their mobile device and our image recognition software will redirect the user to a found statute.

![ocr_demo](./docs/photos/ocr.gif)

## Searching nearby Laws
This feature allows the user to use their location to view nearby laws. These laws are generated from signs that have been successfully scanned with our application.

![location](./docs/photos/location.gif)

# Installation
Select the 'client' or 'server' directory to see respective local installation instructions.

# About OpenHRS development
OpenHRS was developed as part of an effort to improve the efficiency of the Hawaii State Government.

## Milestone 1: Updated Scraper and Code Cleanup
The bulk of this milestone consisted of improving the quality of our existing code, making it more understandable,
maintainable, and modifiable. In essence, our code has been updated to align with our current philosophy of openness.
Due to the nature of coding competitions, much of our code was rushed and could've been written more elegantly. On the front end,
much of the CSS has been removed from the ionic templates and put into the respective component's scss files. Bugs that have
crippled user experience have been patched, for example the arrow keys on each search result page have been fixed to function as they
were meant to. Global CSS variables have been moved to their respective component files to allow for easier customization. Insignificant files
that may confuse potential contributors have been removed.

On the backend,

The team includes:

  * [Jonathan Robello](https://www.linkedin.com/in/jonathan-robello/)
  * [Terry Palomares](https://www.linkedin.com/in/terry-palomares/)
  * [Chris Oh](https://www.linkedin.com/in/christopher-oh-9a1135133/)
  * [Dan Paguirigan](https://www.linkedin.com/in/danpaguirigan/)
  * [Derek Chan](https://www.linkedin.com/in/derek-chan-152378128/)
  * [Kurt Noe](https://www.linkedin.com/in/kurt-noe-39ab19112/)
