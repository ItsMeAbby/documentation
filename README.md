<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#JSON File Format">JSON File Format</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

## About File-Searcher

Search words based on some rules

### Built With

- [Python 3.0](https://docs.python.org/3.0/)

<!-- GETTING STARTED -->

## Getting Started

### Prerequisites

- Python 3.8.10 at [https://www.python.org/downloads/release/python-3810/]

MOVE TO INSTALLATION IF YOU ALREADY HAVE PYTHON INSTALLED IN YOUR SYSTEM

1. Check if you python installed in your system
   ```sh
   python --version
   ```
2. If you have python installed, you can skip this step. If not, you can download python from the link above and install it.
3. Make sure you add python to your path.
   ![Check this while installing](https://www.pylenin.com/content/images/2021/08/Why-learn-Python--7-.png)
   Close and reopen your terminal and check if you have python installed in your system.
   You can check this by typing python in your terminal.

   ```sh
   python
   ```

if you get an error, you need to add python to your path. You can do this by following the steps below:

If you get a message saying python is not recognized, you need to add python to your path. You can follow this link [https://www.architectryan.com/2018/03/17/add-to-the-path-on-windows-10/](https://www.architectryan.com/2018/03/17/add-to-the-path-on-windows-10/) to add python to your path.

### Installation

How to set up your app:

1. Change directory to the folder where you have unzip the project

   ```sh
   cd <path/to/unzip/folder>
   ```

2. Install Requirements
   Make Sure Environment is activated before running it
   ```cmd
   pip install -r requirement.txt
   ```

<!-- Rules json template -->

## JSON File Format

Json file Format

```json
{
  "file_1": {
    "file_path": "<path to file u want to read>",  // eaxmple ""F:\\Sajid\\searcher\\searchDoc.pdf" make sure keep same double back slashes

    "rules": {
      "1": {
        "nature": "OR",
        "file_handler": "_A1",
        "search_terms": ["word1", "word2", "...." , "wordn"]
      },
      "2": {
        "nature": "AND",
        "file_handler": "_B1",
        "search_terms": ["word1", "word2", "...." , "wordn"]
      },
      ....
      ....
      ....
      ....
      "n": {
        "nature": "OR | AND",
        "file_handler": "_An",
        "search_terms": ["word1", "word2", "...." , "wordn"]
      }
    }
  }
}
```

<!-- USAGE EXAMPLES -->

## Usage

How to use the tool:

1. open terminal in your code folder
   ```sh
   cd "PATH/to/your/folder"
   ```
2. run code

   ```sh
   python main.py
   ```

<!-- ROADMAP -->

## Roadmap

- [x] Search words based on some rules
- [ ] Search phrases based on some rules
- [ ] Integrate with dynamic UI
- [ ] SToring data to ensure you dont have to read files again and again
  - [] Database Inegration
  - [ ] JSON Integration
