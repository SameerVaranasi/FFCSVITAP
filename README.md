# FFCS Timetable Planner

A simple browser-based FFCS timetable planner for VIT-AP Fall Semester 2026-27. It helps students choose course slots, view the generated weekly timetable, and avoid slot clashes automatically.

## Features

- Course cards for:
  - `MAT1003` Discrete Mathematical Structures
  - `STS2010` Qualitative and Quantitative Skills Practice I
  - `ECE2002` Computer Organization and Architecture
  - `CSE2001` Data Structures and Algorithms
  - `CSE3002` Artificial Intelligence
  - `MGT1040` Entrepreneurship
- Theory and lab slot dropdowns with faculty name, venue, and available seats.
- Automatic clash filtering:
  - Once a slot is selected, all clashing options in other dropdowns become unavailable.
  - When the slot is unselected, those options become available again.
- Timetable grid based on FFCS theory and lab timings.
- Conflict warning for overlapping selected classes.
- Clear all selections button.
- Download selected timetable as a text file.
- Saves selections in browser local storage.

## How To Use

1. Open `ffcs-timetable-planner.html` in any modern browser.
2. Select theory and lab slots from the course cards.
3. The timetable updates automatically.
4. Clashing slots are disabled automatically.
5. Use `Clear All` to reset.
6. Use `Download Timetable` to save your selected timetable details.

## Run Locally

You can open the HTML file directly, or serve it locally:

```bash
python -m http.server 8765
```

Then open:

```text
http://127.0.0.1:8765/ffcs-timetable-planner.html
```

## Project Structure

```text
.
├── ffcs-timetable-planner.html
└── README.md
```

## Tech Stack

- HTML
- CSS
- JavaScript
- No external dependencies
- No backend required

## Notes

The slot, faculty, venue, and availability data were prepared from the provided FFCS timetable and course/teacher slot PDFs. Availability may change during actual registration, so verify final seats on VTOP before registering.

## License
