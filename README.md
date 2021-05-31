# d1recter
Open redirection finder


## About d1recter

d1recter is a tool designed to detect open redirects vulnerabilities on websites. It helps penetration testers and bug hunters find open redirect bugs through a scan supported by a list of payloads.




## Installation
git clone https://github.com/blackdaliyadali/d1recter.git

## Dependencies
d1recter use requests and tldextract python modules.
```
sudo pip install -r requirements.txt
```

## Usage
| Short form | Long form | Description |
| --- | --- | --- |
| -u | --url | URL to fuzz |
| -f | --file | File with the list of payloads |
| -h | --help | Show the help message |

## Examples
* To scan an URL:
```
python d1recter.py -u https://www.example.com/redirect.php?url= -f payload.list
```
```
python d1recter.py --url https://www.example.com/redirect.php?url= --file payload.list
```
