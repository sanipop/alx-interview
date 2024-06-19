# 0x03. Log Parsing

## Project Overview

This project, part of the ALX curriculum, focuses on real-time data parsing and processing using Python. You will write a script that reads log entries from standard input, processes them, and computes statistics. This project will enhance your skills in file I/O, data processing, and exception handling in Python.

- **Project Start**: June 14, 2024, 6:00 AM
- **Project End**: June 21, 2024, 6:00 AM
- **Checker Release**: June 16, 2024, 12:00 AM
- **Auto Review**: At the deadline

## Learning Objectives

- Reading from `sys.stdin` line by line.
- Handling keyboard interruptions using signal handling.
- Parsing and processing data using regular expressions and string operations.
- Using dictionaries to count occurrences and aggregate data.
- Implementing exception handling for robust data processing.

## Requirements

- **Editors**: vi, vim, emacs
- **OS**: Ubuntu 20.04 LTS
- **Python Version**: Python 3.4.3
- **Code Style**: PEP 8 (version 1.7.x)
- **Executable Files**: All script files must be executable.
- **Documentation**: A `README.md` file at the root of the project folder is mandatory.
- **File Endings**: All files should end with a new line.
- **First Line**: The first line of all files should be `#!/usr/bin/python3`.

## Concepts and Resources

- **File I/O in Python**: [Python Input and Output](https://docs.python.org/3/tutorial/inputoutput.html)
- **Signal Handling in Python**: [Python Signal Handling](https://docs.python.org/3/library/signal.html)
- **Data Processing**: Techniques for parsing and aggregating data.
- **Regular Expressions**: [Python Regular Expressions](https://docs.python.org/3/library/re.html)
- **Dictionaries in Python**: [Python Dictionaries](https://docs.python.org/3/tutorial/datastructures.html#dictionaries)
- **Exception Handling**: [Python Exceptions](https://docs.python.org/3/tutorial/errors.html)

## Tasks

### Task 0: Log Parsing

**Objective**: Write a script that reads from standard input line by line and computes metrics.

#### Input Format

```
<IP Address> - [<date>] "GET /projects/260 HTTP/1.1" <status code> <file size>
```

#### Requirements

- Skip lines not matching the input format.
- Print statistics every 10 lines and/or upon a keyboard interruption (CTRL + C).

#### Statistics to Compute

- **Total File Size**: Sum of all `<file size>` values.
- **Number of Lines by Status Code**: Count occurrences of status codes (200, 301, 400, 401, 403, 404, 405, 500).

#### Output Format

- **Total File Size**: `File size: <total size>`
- **Status Codes Count**:
  ```
  <status code>: <number>
  ```
  Only print status codes that appear in the logs, in ascending order.

### Example

```bash
$ ./0-generator.py | ./0-stats.py
File size: 5213
200: 2
401: 1
403: 2
404: 1
405: 1
500: 3
...
```

## Example Script: `0-stats.py`

```python
#!/usr/bin/python3
import sys
import signal

total_size = 0
status_counts = {
    "200": 0, "301": 0, "400": 0, "401": 0,
    "403": 0, "404": 0, "405": 0, "500": 0
}

def print_stats():
    print(f"File size: {total_size}")
    for code in sorted(status_counts.keys()):
        if status_counts[code]:
            print(f"{code}: {status_counts[code]}")

def signal_handler(sig, frame):
    print_stats()
    sys.exit(0)

signal.signal(signal.SIGINT, signal_handler)

line_count = 0

for line in sys.stdin:
    try:
        parts = line.split()
        if len(parts) > 6:
            size = int(parts[-1])
            code = parts[-2]
            total_size += size
            if code in status_counts:
                status_counts[code] += 1
            line_count += 1
            if line_count == 10:
                print_stats()
                line_count = 0
    except Exception:
        pass

print_stats()
```

## Repository Structure

- **GitHub Repository**: `alx-interview`
- **Directory**: `0x03-log_parsing`
- **Script File**: `0-stats.py`

## Additional Resources

- [Mock Technical Interview](https://example.com)

---

© 2024 ALX, All rights reserved.
