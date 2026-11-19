# Project 2 - Web Service Application

### Overview

For this project you are creating a JavaScript driven Web application that utilizes a Web service: your GIF Finder, with the GIPHY API switched out for a different Web API.

- Ideally the experience will run in all modern browsers, but at a bare minimum it must run in recent versions of Chrome.

You will be evaluated on:
  - how well you met the requirements of the assignment.
  - the soundness of your programming.

Resources:
  - Our entire Web apps series: [Web Apps 0 - About this Web App Tutorial Series](https://github.com/rit-igm-web/igme-235-shared/blob/main/tutorial/web-apps-0.md)
  - Starter code: GIF Finder rewritten with `fetch`, released on myCourses once you have submitted GIF Finder.
  - `localStorage` details: [Web Apps 9 - WebStorage API](https://github.com/rit-igm-web/igme-235-shared/blob/main/tutorial/web-apps-9.md)
  - https://developer.mozilla.org/en-US/docs/Web/JavaScript

### Requirements

1. Select a Web API for this project (see the bottom of this file for details) and plug it into the GIF Finder `fetch` starter code.

2. Save the last term searched by the user in the browser local storage.

   - we are going to test this capability by typing in a search term, doing a search, and then closing the browser window. When we re-open the window, the user's last search term should still be in the field.
   - if there isn't a 'search term' to save in your project, then save something else and be sure to document what is saved.

3. Required controls - Have a minimum of 2 working controls that a user can use to filter and display the results. Search buttons or similar don't count towards the 2 controls. For example, GIF Finder has these controls:
   - a search button (which doesn't count)
   - a search term field (`<input>`) that the user types into
   - a pulldown (`<select>`) that the user can use to limit the number of results

4. Make sure there are no JavaScript errors or exceptions thrown by the app.

5. All code convention standards are met:

    - All code is an external JavaScript file - inline event handlers are not allowed
    - `let` and `const` must be used to declare variables (no `var`!)
    - `querySelector()` and `querySelectorAll()` must be used for DOM traversal (DO NOT use the older methods)
    - D.R.Y. - Don't Repeat Yourself. Repeated blocks of nearly identical code must be factored out and placed in a separate function.
    - Variable and function names must begin with a lowercase letter.
    - Well-commented code. Each and every function gets a comment indicating what it does.
    - Delete or comment out any `console.log()` calls.

### Grading

The grading rubric for this project is visible in myCourses. You should look it over carefully. 

### Submission

- ZIP and post the completed project to the myCourses dropbox
- Post the project to Banjo and link it from your 235 home page

<hr>
<hr>

## API Selection Options

#### 1. Specified API Option

- You may get familiar with and use one of the APIs from this list:
  - Because APIs change from time to time this is not a guarantee that these APIs will be smooth sailing, but they have been shown to work.
    - Tenrai Unofficial MyAnimeList API\*: https://api.tenrai.org/documentation
    - The Amiibo API\*: https://www.amiiboapi.org
      - \*Starters for the above 2 APIs can be found in the [web-service-app-starters.md](https://github.com/rit-igm-web/igme-235-shared/blob/main/tutorial/web-service-app-starters.md)
    - Disney API: https://disneyapi.dev/
    - TV Maze API: https://tvmaze.com/api
    - Pokemon API: https://pokeapi.co/docs/v2
    - Rick and Morty API (REST version): https://rickandmortyapi.com/documentation
    - Scryfall Magic: The Gathering Search: https://scryfall.com/docs/api
    - Open Trivia DB API: https://opentdb.com/api_config.php
    - Mixcloud (This is a little more complicated): https://www.mixcloud.com/developers/
  - Results don't have to be images: formatted HTML showing the data you care about is fine.

#### 2. Choose Your Own API Option

- Show me a working call to it by Friday 11/20.
- There are API lists that you can peruse, however there are a couple of guidelines.
  - Look for an API that supports _CORS_ (Cross-origin resource sharing) - if the API says **NO** in the **CORS** column then it will **NOT work** well for this project
    - **DO NOT** use any API that requires _OAuth_ authentication
    - if an API requires an API Key, be sure that there is a "free tier", and that the API does not have a short trial period
    - **Tip:** The easiest APIs to work with are ones that require **no authentication at all** — look for APIs where the Auth column says "No". You can get up and running immediately without signing up for anything.
    - Here are some lists to check out:
      - https://github.com/public-api-lists/public-api-lists <- Large categorized directory with Auth and CORS columns. **Start here!**
      - https://github.com/toddmotto/public-apis <- Includes CORS column.
      - https://github.com/abhishekbanthia/Public-APIs <- Less info about each API.
