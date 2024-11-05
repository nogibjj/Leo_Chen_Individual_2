# Leo Chen Individual 2

[![Python](https://github.com/nogibjj/Leo_Chen_Individual_2/actions/workflows/python.yml/badge.svg)](https://github.com/nogibjj/Leo_Chen_Individual_2/actions/workflows/python.yml)
[![Rust](https://github.com/nogibjj/Leo_Chen_Individual_2/actions/workflows/rust.yml/badge.svg)](https://github.com/nogibjj/Leo_Chen_Individual_2/actions/workflows/rust.yml)

## Demo Video
For a quick walkthrough of this project, please utilize this [demo video](https://github.com/nogibjj/Leo_Chen_Individual_2/blob/main/demo.mp4).

## Purpose
The goal of this project is to demonstrate doing CRUD (Create, Read, Update, Delete) operations with `Rust`. A CLI tool was built, and the binary file is available for download in the latest workflow run under the `Actions` tab (Actions artifact).

## Required Dependencies
- rusqlite
- sysinfo

## Installation

### Prerequisites
- **Rust** and **Cargo** installed on your machine. [Installation Guide](https://www.rust-lang.org/tools/install)

### Build the Project
```
cargo build --release
```

### Option 1: Temporary
Add the compiled binary to your `PATH`:
```
export PATH=$PATH:.../echo/target/release
```

### Option 2: Install Globally
```
cargo install --path .
```

## Usage
Run the tool with no argument:
```
Leo_Chen_Individual_2
```

## Data Source
U.S. births data for the years 2000 to 2014, as provided by the Social Security Administration

Header | Definition
---|---------
`year` | Year
`month` | Month
`date_of_month` | Day number of the month
`day_of_week` | Day of week, where 1 is Monday and 7 is Sunday
`births` | Number of births

[Link to data source](https://github.com/fivethirtyeight/data/blob/master/births/US_births_2000-2014_SSA.csv)

## CRUD Operations
Operations can be found [here](https://github.com/nogibjj/Leo_Chen_Individual_2/blob/main/mylib/query.py)
1. Create: `create a new record: 2024, 10, 5, 6, 7785`
2. Read: `read all data`
3. Update: `update record 55: births = 7899`
4. Delete: `delete record 420`

## Use of LLMs
ChatGPT was used during the coding process. Since I already have a Python script that does CRUD operations, I asked ChatGPT to rewrite the code in Rust. The task was completed almost flawlessly - there were a few back and forth to correct some minor bugs.

## Performance Comparison Report
A performance comparison report has been produced to show the improvements in speed and resource usage provided by `Rust`. Access the report [here](https://github.com/nogibjj/Leo_Chen_Individual_2/blob/main/report.md).
