To install more patterns you could use the example below

```
sudo su -

cd /opt/tools/

git clone https://github.com/1ndianl33t/Gf-Patterns

mv /opt/tools/Gf-Patterns/*.json ~/.gf
```

After that you can test using the command below:

```
findomain -t testphp.vulnweb.com -q | httpx -silent | anew | waybackurls | gf sqli >> sqli ; sqlmap -m sqli --batch --random-agent --level 1
```
