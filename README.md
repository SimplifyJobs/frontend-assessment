![logo](https://user-images.githubusercontent.com/21349718/227146863-399bdd2b-2091-4461-9775-141af610f9ef.svg)

# Simplify Frontend Exercise

Hello! If you're reading this then we're likely in the process of considering you for a role at Simplify. If so, congratulations 🎉 !

We'd like to know a little more about how you work, so this repository contains a short (approximately 2-3 hours) exercise that you can use demonstrate your skills and abilities.

We know that 2-3 hours is not a lot of time and you may not be able to complete everything you'd like, and will feel pressure to do more. We're not looking for perfection in the UI and are not evaluating your skills as a designer so be sure to focus on functionality and showing your knowledge of NextJS and React best practices. Of course if time permits, feel free to polish the UI and flex any design skills. Best of luck!

# Overview

In this exercise you will be using React, NextJS, and TailwindCSS to make three pages of an ecommerce app. You will be getting familiar with TailwindCSS and exploring the features of NextJS like server-side rendering, app layouts, and dynamic slugs. Your task will be to create pages/components based on the designs from a Figma file, mock an api to provide data to the pages, and follow instructions on which NextJS features to use for the pages.

The goal of this exercise is to evaulate your ability to:
* translate specs into well organized components
* successfully implement advanced features of NextJS you may be unfamiliar with
* showcase your experience with styling components with TailwindCSS

# Instructions

Clone this repo to get started. We've provided a starter project for you with React 18, Typescript, [NextJS 13](https://beta.nextjs.org/docs/getting-started), [TailwindCSS](https://tailwindcss.com/docs/installation), and [SWR](https://swr.vercel.app/docs/getting-started) already added and default configured. Be sure to read through the docs for these libraries if you are unfamiliar. You're also welcome to use any other packages if you'd like, just be sure to explain why you decided to use them and meet all the project requirements with the provided stack.

1. Mock ecommerce API

Using the api route feature in NextJS mock the following routes:
* Getting a list of favorite items
* Getting details of an item from its ID

We've provided a json file with mock data to use called `data.json`. Feel free to modify it or add to it if you wish. Though we are't expecting you to do error handling, you may add error responses to the api if you have time.

2. Make three pages using NextJS App Router format. Implement a root layout and individual layout files where needed.

The designs for the three pages can be found in this [Figma file](https://www.figma.com/file/lUbwgHr7OTh4IEf1Y4szwf/NextJS-Ecommerce?node-id=0%3A1&t=bHXi1DmZpSYk17Wd-1). Implement the designs, creating components where it makes sense and following best practice organization. 

* `/dashboard/list`
  * Following the `List page` design, create a page that uses a top navigation bar layout with the main content showing a list of the user's favorite items. 
  * Use swr to load the data client side from the mock API you made in step 1. Before the data is loaded, show a loading icon in place of the list. 
  * The list items do not need to have any functionality other than when clicking on an item it will take you to the /item/[id] page of its id. 
  * The appearace/UI of the top navigation is not important and does not need to match the design if it is time consuming. 
* `/dashboard/card`
  * Following the `Card page` design, create a page that uses a side navigation bar layout with the main content showing a grid of cards of the user's favorite items. 
  * Use swr to load the data client side from the mock API you made in step 1. Before the data is loaded, show a loading icon in place of the grid. 
  * The card items do not need to have any functionality other than when clicking the View button it will take you to the /item/[id] page of its id. 
  * The appearace/UI of the top navigation is not important and does not need to match the design if it is time consuming.  
* `/item/[id]`
  * Following the `Detail page` design, create a page with the Catch-all Segment to show details of a certain item. This page can use either layout configuration (Route groups may be helpful) and does not need to contain all text content from the design. 
  * This page should be Server-Side Rendered with NextJS - load the items details from the API and pass it to the page.

# Submission

When you're done just zip the project and email it back to us -- **be sure to keep your repository private**. Include instructions for running the app locally in the README as well as any additional explanation you'd like to add. If you used any AI tooling during this take home be sure to outline which tools and how you used them.
