```bash
$apt update -y
$apt upgrade -y
$apt install python
$python -m venv sqlmap-env
$source sqlmap-env/bin/activate
$pip install sqlmap
$sqlmap --help
$sqlmap -u http://testphp.vulnweb.com/artists.php?artist=2
$deactivate
```
