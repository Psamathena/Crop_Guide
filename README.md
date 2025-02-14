# Crop Guide Project

## Overview

The Crop Guide Project is a Python-based application designed to provide crop recommendations based on seasonal and regional factors. It utilizes SQLite for database management and PyQt5 for the graphical user interface (GUI).

## Features

- Provides crop recommendations based on seasons and geographical regions.
- Uses SQLite to store and retrieve crop data.
- GUI-based interaction using PyQt5.
- Displays recommended crops with associated pesticide information.
- Supports conversion of UI files to Python scripts for GUI modifications.

## Installation

### Prerequisites

Ensure you have Python installed on your system. You will also need the following dependencies:

1. Install the required Python modules:
   ```sh
   pip install -r requirements.txt
   ```
2. Install Qt-Designer for GUI modifications (optional): [Download Qt-Designer](https://build-system.fman.io/qt-designer-download)

## Running the Project

1. Extract the project folder `CropGuide_py`.
2. Run the database script to set up the SQLite database:
   ```sh
   python database.py
   ```
3. Launch the main application:
   ```sh
   python cropguide.py
   ```

## File Structure

- `database.py`: Creates an SQLite database and populates it with initial crop data.
- `cropguide.py`: Main GUI application for user interaction.
- `requirements.txt`: Lists required dependencies.
- `CROP_GUIDE_README FILE.pdf`: Additional project documentation.

## Database Details

The database contains a `crop` table with the following fields:

- `season`: Crop season (Kharif, Rabi, Zaid).
- `nh`, `nl`: Northern region high and low production crops.
- `sh`, `sl`: Southern region high and low production crops.
- `northern`, `southern`: Lists of states in respective regions.

## Using the GUI

1. Select a **Season** from the dropdown menu.
2. Select a **State** from the dropdown menu.
3. Enter **Acres of land** and **Budget**.
4. Click the **Submit** button to get crop recommendations along with pesticide suggestions.

## Converting UI Files (If Modifications Are Needed)

To convert a `.ui` file to a Python script, run the following command:

```sh
pyuic5 -x cropguide.ui -o cropguide.py
```

## License

This project is for educational purposes. Modify and use it as needed.

## Contributors

- [Your Name]
- [Additional Contributors]

