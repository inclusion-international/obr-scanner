# OBR Scanner Tool

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## Description

A Python script that monitors a specified directory for file creation or modification events using the `watchdog`
library.\
When events occur, it runs a script `run_local.py` and starts a scanner software specified by the `scanner_exe`
environment variable.

## Table of Contents

- [Documentation](#documentation)
- [Requirements](#requirements)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Installation Steps](#installation-steps)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Documentation

Explore project documentation and manuals in the [Documents](Documents) directory:

- [Description Manual (Word)](Documents/Description_Manual.docx)
- [Description Manual (PDF)](Documents/Description_Manual.pdf)

Learn about the frame and its construction:

- [Frame Documentation (Word)](Documents/Frame.docx)
- [Frame Documentation (PDF)](Documents/Frame.pdf)

## Requirements

- Python 3.x
- `watchdog` library: Install it using `pip install watchdog`

## Dependencies

This project relies on the [AngelinaReader](https://github.com/IlyaOvodov/AngelinaReader) GitHub repository. Ensure it
is installed and running before using this script.

Follow the installation instructions for the [AngelinaReader](https://github.com/IlyaOvodov/AngelinaReader) in its
repository.

## Installation

- Python 3.x
- `watchdog` library: Install it using `pip install watchdog`

## Installation Steps

1. Set up the environment:
    - Ensure you have Python installed.
    - Install the required Python packages by running:
   ```bash
   pip install watchdog
   ```

2. Set the `scanner_exe` environment variable:
    - Specify the path to the scanner software executable in the environment variable. \
      For example:

   ```bash
   export scanner_exe=/path/to/scanner/executable
   ```

## Usage

Run the script:

   ```bash
   python app.py
   ```

The file app.py has to be inside the [AngelinaReader](https://github.com/IlyaOvodov/AngelinaReader) repository,
otherwise it doesn't work

## Configuration

Modify the `watch_directory` variable in the script to specify the directory to monitor.
Adjust the `language` variable and the script command in the `Handler` class to fit your requirements.

## Notes

This script assumes a Unix-like environment.\
If your operating system is windows set up the environment variable accordingly.

## Contributing

If you would like to contribute to the project, provide guidelines for how others can do so. This may include
information about submitting bug reports, feature requests, or code contributions.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- [AngelinaReader](https://github.com/IlyaOvodov/AngelinaReader)
