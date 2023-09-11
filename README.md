# WEAKSWEET

WEAKSWEET Checker is a Bash script that scans a list of IP addresses for weak SSH algorithms and vulnerabilities related to the SWEET32 attack. It provides a comprehensive report of the scan results.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Options](#options)
- [Sample Output](#sample-output)
- [License](#license)

## Installation

1. Clone the repository or download the Bash script (`weaksweet_checker.sh`) to your local machine:

```bash
git clone https://github.com/yourusername/weaksweet-checker.git
```

2. Make the script executable:

```bash
chmod +x weaksweet_checker.sh
```

## Usage

To scan a list of IP addresses for weak SSH algorithms and SWEET32 vulnerabilities, use the following command:

```bash
./weaksweet_checker.sh -i input_file.txt -o output_file.txt
```
Replace `input_file.txt` with the path to your input file containing a list of IP addresses. 
Replace `output_file.txt` with the desired name of the output file where the scan results will be saved.

## Options

-h: Display the help message, which includes usage instructions and available options.
-i input_file: Specify the input file containing a list of IP addresses to scan. Each IP address should be on a separate line in the file.
-o output_file: Specify the output file where the scan results will be saved. If not specified, the default output file is output.txt.

## Sample Output

Here is an example of the output format generated by WEAKSWEET Checker:

```lua
IP Address      | Port Status        | Scan Result
---------------------------------------------------------
192.168.1.100   | open               | Vulnerable to SSH Weak Key Exchange
192.168.1.101   | open               | No vulnerabilities
192.168.1.102   | closed             | Filtered or Closed

Output File Saved on output.txt
```

---