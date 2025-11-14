```bash
$apt update -y
$apt upgrade -y
$apt install python -y
$apt install git -y
$apt install golang -y
$go install -v github.com/projectdiscovery/subfinder/v2/cmd/subfinder@latest
$mv /data/data/com.termux/files/home/go/bin/subfinder /data/data/com.termux/files/usr/bin
$subfinder -h
$subfinder -d apple.com -v
```
