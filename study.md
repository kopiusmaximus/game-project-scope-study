# Game Project Scope Study

## Required Readings

-   [Game Project](https://github.com/ga-wdi-boston/game-project)
-   [Game API](https://github.com/ga-wdi-boston/game-project-api)
-   [What is a User Story](http://searchsoftwarequality.techtarget.com/definition/user-story)

## Deliverables

After reading the `game-project` prompt and the `game-project-api` documentation
please do the following and be prepared to share and discuss during our next
class.

Submit detailed answers to these in this file via a pull request.

## Project Wireframes

-   [Wireframe 1](./assets/images/wireframe-1.png)
-   [Wireframe 2](./assets/images/wireframe-2.png)

## Data Structure

```md
In order to stay consistent with the provided API, the following data structures
will be used to represent key entities:

Entity: User
Every user will be represented by a "user" object. Every "user" object will
include a "games" property, whose value will be an array of "game" objects

Entity: Game
Every "game" object will include several properties, including "cells", two
players, and a boolean flag indicating whether the game is over.

Entity: Board
The value of "cells" for any given "game" object will be an array of 9
single-character strings, representing the current state of the board in that
game. A valid move will be an event, triggered by a click, that updates the
value of a single element in "cells".

```

## Representing markup of the game board in JS

```md
The board will be represented visually on the page by a 3x3 grid of HTML
elements. Each of these elements will have a shared class and a unique
identifier. Each identifier will be linked to a JS event handler, such that when
a board element is clicked, a function is fired that changes the appearance of
the board in the UI (by updating the DOM to paint an X or O in that element,
depending on whose turn it is).

```

## Overall Approach

```md
I will start by building the skeleton of the page in HTML, just the minimal
markup necessary to provide the basic layout of the page, along with the
necessary CSS to locate elements in their correct positions

I will then focus on authentication, starting by getting a functioning signup
button that creates a user. I will validate successful communication with the
API first via cURL request and then via AJAX request.

Once I have successfully proven the client-server link, I will build out the
rest of the authentication functionality: sign in, sign out, change password,
get user, and get users.

Then I will write necessary code for creating new game and appending it to the
logged-in user's 'games' array property.

Once a user is able to create a game, I will write and test the game logic for a
single game turn, starting with a click event on a board element and ending with
an update to the UI that displays the result of the move.

Once a single turn is functioning properly, I will build out the rest of the
game logic, including a check every turn to see if the game has ended, and the
necessary input validation to ensure that game rules are enforced (i.e. can't
take a taken square, can't move after the game has ended).

Once I am satisfied that the user can play an entire game from start to finish,
bug-free, with only legal moves being allowed, then I will focus on building out
the user's statistics dashboard, by processing data from past games and reducing
it to set of key metrics to be displayed when the "Stats" tab is clicked.

When this is done, I will focus on aesthetics, making additions to the project's
stylesheet until the site looks attractive and clean.

Once the basic application has been tested, debugged, and styled to satisfy the
basic project requirements, I will consider whether I have sufficient time to
attempt the bonuses.

```

## User Stories

```md
The following user stories describe key aspects of the applications's
functionality from a user perspective:

As a user, I want to create an account so I can keep track of games I have
played.

As a user, I want to change my password so I can protect my account if I think
my previous password has been compromised.

As a user, I want to sign out so I can protect my account when I'm done playing.

As a user, I want to start a game so I can play Tic-Tac-Toe in the browser
window with a friend.

As a user, I want the game application to "know" the rules of Tic-Tac-Toe so I
can't accidentally make an illegal move or keep playing after a game has ended.

As a user, I want to access all games associated with my account so I can see
how my play has changed over time.

As a user, I want the ability to start a new game at any time so I don't have to
finish games whose eventual outcome is already obvious.

```

## Modularity

```md
As modeled in last week's trainings, I will maintain separate scripts for event
handlers, UI functions, and API functions, exporting objects from each script
only as needed.

In addition, I will separate scripts describing user authentication and profile
functionality from scripts describing game functionality.

```

## Creative Spin

```md
My version of the browser-based Tic-Tac-Toe game will include a user dashboard
tab that allows players to interpret their game history at a glance with a
series of key metrics, including win-loss record and average duration (in turns)
of each game they have played.

I also plan to incorporate a sleek, minimalist aesthetic with smooth curves and
lightly shadowed edges, easy on the eyes but drawing and holding user focus onto
the game board.

```

## Version Control

```md
All files that make up the project will be stored in a GitHub repository that is
maintained both locally and remotely. Changes will be made locally, documented
via small and frequent commits, and backed up frequently by pushing to the
remote repository.

Different aspects of the project will be built on separate branches and merged
into the master branch only after being fully tested.  At the very least, there
will be an "authentication" branch, a "game" branch, and a "statistics" branch.

If I attempt any bonuses, I will write their code on separate branches so that
if I do not finish them in time, I can still deploy a working application from
the master branch.

```

## Bonuses

```md
At present, I do not plan on attempting any of the bonuses. If I satisfy the
core requirements with time to spare, I am considering attempting the
separate-devices bonus and the tableside-chat bonus.

```
