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

[Wireframe 1](./assets/images/wireframe-1.png)

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
How you plan to approach this project

```

## User Stories

```md
The following user stories describe key aspect's of the applications's
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
My version of the browser-based Tic-Tac-Toe game will include a user
dashboard tab that allows players to interpret their game history at a glance,
include win-loss record and average duration (in turns) of each game they have
played.

I also plan to incorporate a sleek, minimalist aesthetic that draws and holds
user focus on the game board.

```

## Version Control

```md
All files that make up the project will be stored in a GitHub repository that is
maintained both locally and remotely. Changes will be made locally, documented
via small and frequent commits, and backed up frequently by pushing to the
remote repository.

```

## Bonuses

```md
At present, I do not plan on attempting any of the bonuses. If I satisfy the
core requirements with time to spare, I am considering attempting the
separate-devices bonus and the tableside-chat bonus.

```
