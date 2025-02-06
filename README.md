# Calendar Program in C

## Introduction
This C program displays a calendar for a specified month and year. The program allows users to navigate between months and years using arrow keys and also provides an option to jump to a specific date.

## Features
- Displays the calendar for a given month and year.
- Allows navigation using arrow keys:
  - **Up Arrow**: Moves to the previous month.
  - **Down Arrow**: Moves to the next month.
  - **Left Arrow**: Moves to the previous year.
  - **Right Arrow**: Moves to the next year.
- Allows users to enter a specific year and month.
- Prevents selection of years before 1945.
- Highlights Sundays and provides a visual layout using ASCII characters.
- Uses Windows-specific functions for cursor movement and color changes.

## Requirements
- Windows OS (as it uses `windows.h` for console manipulation)
- C compiler (such as GCC or Turbo C++)

## Compilation and Execution
1. Open a terminal or command prompt.
2. Compile the program using a C compiler:
   ```bash
   gcc calendar.c -o calendar
   ```
3. Run the executable:
   ```bash
   calendar
   ```

## Functions Used
### `gotoxy(int x, int y)`
Moves the cursor to the specified position in the console.

### `SetColor(int ForgC)`
Changes the text color in the console.

### `getkey()`
Captures keyboard input, including special keys like arrow keys.

### `display(int nyr, int nmonth, int tdays, int days[])`
Displays the calendar for the specified month and year.

### `calendar(int nyr, int nmonth)`
Calculates the number of days and determines the starting position for the month in the calendar layout.

## How to Use
1. Run the program and enter a valid year and month.
2. Use arrow keys to navigate:
   - **Right Arrow**: Next year
   - **Left Arrow**: Previous year
   - **Up Arrow**: Previous month
   - **Down Arrow**: Next month
3. Press `P` to enter a specific year and month.
4. Press `ESC` to exit the program.

## Limitations
- Only supports years from **1945 onwards**.
- Works only on Windows due to dependency on `windows.h`.

## Author
- **[Diyansi chaudhary]**

