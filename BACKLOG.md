# User Story

As a API consumer, I want to be able to request and get data about the King and Rook position on a chessboard, so I can show the position of the King and Rook on a chessboard.

## Title: Viewing the Chessboard in "Is the King in Check"

## Description:
As a user, I want to see a chessboard with a king and a rook placed on it when I start the game through the console, so that I can instantly determine whether the king is in check.

## Acceptance Criteria FE:

    Upon starting the game from the console, a chessboard should be displayed on the UI.
    The chessboard should contain only two pieces: a king and a rook.
    The positions of the king and the rook are fixed and known (e.g., king at E1, rook at A5).
    A label should be displayed stating whether the king is in check based on the positions of the pieces.
    The UI should be simple and minimalistic, with clear visibility of the chess pieces and the status label.

## Acceptance Criteria BE:

    The backend should ... if a king is in check or not

## Gherkin Scenario:

### Scenario: Displaying the initial chessboard with fixed piece positions

    Given the user starts the game from the console,
    When the game UI loads,
    Then the user sees a chessboard displayed on the screen
    And the king is placed at E1
    And the rook is placed at A5
    And a label is shown indicating if the king is in check or not.



## UI Sketch:
        +----+----+----+----+----+----+----+----+
    8   |    |    |    |    |    |    |    |    |
        +----+----+----+----+----+----+----+----+
    7   |    |    |    |    |    |    |    |    |
        +----+----+----+----+----+----+----+----+
    6   |    |    |    |    |    |    |    |    |
        +----+----+----+----+----+----+----+----+
    5   | R  |    |    |    |    |    |    |    |
        +----+----+----+----+----+----+----+----+
    4   |    |    |    |    |    |    |    |    |
        +----+----+----+----+----+----+----+----+
    3   |    |    |    |    |    |    |    |    |
        +----+----+----+----+----+----+----+----+
    2   |    |    |    |    |    |    |    |    |
        +----+----+----+----+----+----+----+----+
    1   |    |    |    |    | K  |    |    |    |
        +----+----+----+----+----+----+----+----+
          A    B    C    D    E    F    G    H

    Status: King is not in check.
