```bash
$apt update -y
$apt upgrade -y
$apt install python -y
$apt install git -y
$apt install golang -y
$go install -v github.com/projectdiscovery/nuclei/v3/cmd/nuclei@latest
$mv /data/data/com.termux/files/home/go/bin/nuclei /data/data/com.termux/files/usr/bin
$nuclei
$nano custom-sqli.yaml
$nuclei -target http://testphp.vulnweb.com/artists.php?artist=2 -t custom-sqli.yaml -dast
```
