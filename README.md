# JSON Parser in Go

## Overview

This is a command-line tool built in Go for parsing JSON files. It validates the JSON syntax and returns a human-readable error message with the line and column information if the JSON is invalid.

## Features

- Validates JSON strings from a given file.
- Displays human-friendly error messages with line and column numbers.
- Works as a standalone CLI tool.
  
## Getting Started

### Prerequisites

- Go (at least v1.16)

### Installation

1. **Clone the repository**

    ```bash
    git clone https://github.com/sanketchaudhari3009/json-parser-go.git
    ```

2. **Navigate to the project directory**

    ```bash
    cd json-parser-go
    ```

3. **Build the project**

    ```bash
    go build -o json-parser
    ```

### Usage

Run the program and specify the JSON file to be parsed.

```bash
./json-parser --file="path/to/your/json/file.json"
```
This will either display a message stating that the JSON is valid or show an error message with line and column details.

### Input

A sample input file might contain:

```json
{
    "name": "Sanket",
    "age": 21,
    "city": "Pune",
    "Indian": true,
    "male": True
}
```
### Output
```
JSON is invalid: invalid character 'T' looking for beginning of value
exit status 1
```
