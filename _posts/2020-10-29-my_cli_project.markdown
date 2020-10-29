---
layout: post
title:      "My CLI Project"
date:       2020-10-29 16:52:07 +0000
permalink:  my_cli_project
---


For my CLI Project, I decided to use the PokeAPI. With this came a few struggles that I couldn't quite figure out, however I was still able to pull through and create a functioning CLI.

## What I saw and did

When looking at the API I saw a few things. First off, I saw results which contained a list of 20 pokemon and I saw that at the top of the JSON was "next" which gave a URL to the next set of 20 pokemon. With this, in my CLI I was able to access results to print out the list of pokemon and return the name and a url to more information about whichever pokemon a user selected.

## My Challenges
1. I could not figure out how I could possibly delve deeper into the API because the PokeAPI had a lot of it's information behind URLs and I was unable to solve how to open those and retrieve data from multiple URLs.

2. When creating pokemon_choice (A method I made to allow users to choose a pokemon from the list of 20 I was able to pull) I tried making it so that the user would have to input an option between 1-20. This worked for the most part, however I found out that if I tried inputting 21 rather than returning invalid input as it should do, it simply broke the code. The fix I found for this, was to rather than doing index.between?(0, 20) I would do index.between?(0, Pokemon.all.length - 1)

## What I could add in the future
Something that really dissapointed me with my CLI, is that I couldn't delve deeper into the PokeAPI because I was unsure of how I could use the URLs that the API gave. In the future if possible, I would love to expand the list of data you can view within my CLI if I can figure out how to access multiple URLs.


