# Google Doc Grid Decoder

## Overview

This project retrieves a published Google Doc containing Unicode
characters and their X-Y coordinates and reconstructs them into a
2D character grid.

The generated grid reveals a hidden sequence of uppercase letters.

## Technologies Used

- Python
- Requests
- BeautifulSoup

## How It Works

1. Fetch the published Google Doc.
2. Parse the table containing X-coordinate, character, and Y-coordinate.
3. Determine the required grid dimensions.
4. Fill unspecified positions with spaces.
5. Place each Unicode character at its corresponding coordinate.
6. Print the grid from the highest Y-coordinate to the lowest.

## Time Complexity

O(N + XY)

Where N is the number of characters and X × Y is the size of the grid.

## Space Complexity

O(XY)

The program stores the reconstructed 2D grid.

## Installation

```bash
pip install -r requirements.txt
