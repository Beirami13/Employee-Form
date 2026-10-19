# Employee Form

A small desktop application for registering job applicants, built with Python and Tkinter. It was an early practice project for learning Tkinter widgets, event handling, and saving data to a CSV file.

## Features

- Registration form with these fields:
  - Name and family (required)
  - Weight (spinbox, 20 to 150)
  - Height (slider, 100 to 200)
  - Married (checkbox)
  - Degree level ("junior" checkbox)
  - Type of experience (radio buttons: Academic, Experimental, Public class, Private class, YouTube)
  - Wishes (free text)
- **Save** (File menu): validates the required fields, appends the record to `data.csv`, shows a confirmation, and resets the form
- **Give information** button: builds a one-sentence summary of the applicant and shows it in the window
- Info pop-up window that opens together with the main window
- **Quit** (File menu)

## Requirements

- Python 3.x
- Tkinter (included with Python on Windows and macOS; on Debian or Ubuntu install it with `sudo apt install python3-tk`)
- No other packages

## How to run

```bash
git clone https://github.com/Beirami13/Employee-Form.git
cd Employee-Form
python employee_form.py
```

## Output

Saved records are appended to `data.csv` in the folder you run the program from (UTF-8, no header row). Each row has these columns:

```text
name, family, weight, married (0/1), height, experience, wishes
```

Example:

```text
Ali,Ahmadi,70,1,175,Academic,Learning Python
```

## What I practiced

- Building a window with `Tk`, `Toplevel`, `Label`, `Entry`, `Spinbox`, `Scale`, `Checkbutton`, `Radiobutton`, `Text`, `Canvas`, `Button`, and `Menu`
- Laying out widgets with the `grid` geometry manager
- Reading widget values with `StringVar` and `IntVar`
- Showing messages with `messagebox`
- Writing rows to a CSV file with the `csv` module

## Known limitations

- The "junior" checkbox is not saved to `data.csv` yet.
- Some labels contain typos (for example "Weigh" and "Marrie").
- The code is in a single file and there are no automated tests.
- `data.csv` is plain text and contains personal data, so do not commit your own records.

## Status

This repository is archived. It is kept as a record of an early learning project and is no longer maintained.
