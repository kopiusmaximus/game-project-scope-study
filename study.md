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

## Project Wireframe

```md
A wireframe of what your game project will look like.

Wireframe sketches:
```

[Wireframe 1](./assets/image/wireframe-1.png)

## Data Structure

```md
In order to stay consistent with the provided API, the following data structures
will be used to represent key entities:

Entity: User
Every user will be represented by a "user" object every "user" object will
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
How you will take the markup of the game board and represent it in JS

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
How do you plan to keep your code modular?

```

## Creative Spin

```md
What creative spin will you add to your project?

```

## Version Control

```md
How you will use version control to backup / track your project?

```

## Bonuses

```md
Do you plan to attempt any of the bonuses?

```
