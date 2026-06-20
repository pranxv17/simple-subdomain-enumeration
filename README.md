# Simple Subdomain Enumeration

A lightweight Bash script for discovering live subdomains of a target domain using Assetfinder and Httprobe.

## Features

- Finds subdomains using Assetfinder
- Checks for live HTTP/HTTPS services using Httprobe
- Removes duplicate entries
- Saves results to a text file
- Simple and easy to use

## Requirements

Install the following tools:

- assetfinder
- httprobe

### Install Assetfinder

```bash
go install github.com/tomnomnom/assetfinder@latest
```

### Install Httprobe

```bash
go install github.com/tomnomnom/httprobe@latest
```

### Add Go binaries to PATH

```bash
echo 'export PATH=$PATH:$HOME/go/bin' >> ~/.bashrc
source ~/.bashrc
```

## Usage

Make the script executable:

```bash
chmod +x simple_subdomain_enumeration_script.sh
```

Run the script:

```bash
./simple_subdomain_enumeration_script.sh
```

Enter the target domain when prompted:

```text
Enter the domain name (example.com): example.com
```

## Example Output

```text
[*] Finding subdomains for example.com ...

[+] Subdomains found:
https://api.example.com
https://mail.example.com
https://www.example.com

[+] Results saved in /home/user/Subdomains_list.txt
```

## Output

Results are saved in:

```text
Subdomains_list.txt
```

## Disclaimer

Use this tool only on domains you own or have explicit permission to test. Unauthorized scanning may violate laws, regulations, or terms of service.

## Author

GitHub: @pranxv17
