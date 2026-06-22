# Cyber-Architecture
Here we explain every step to learning  in cybersecurity


1. Les fondations indispensables (le "SC")
Avant de toucher à du pentest ou du red team, il faut maîtriser :

Réseaux

Modèle OSI / TCP-IP en profondeur
Routage, switching, VLANs, NAT
Protocoles : ARP, DNS, HTTP/S, TLS, DHCP, Kerberos, SMB
Outils : tcpdump, Wireshark, nmap
Systèmes

Linux : administration, permissions, processus, systemd, bash scripting
Windows : Active Directory, GPO, NTFS, permissions, PowerShell, registre
Virtualisation : VMware, VirtualBox, Proxmox pour monter tes labs
Programmation / Scripting

Python (indispensable) : sockets, requests, scapy, impacket
Bash / PowerShell
Comprendre le C pour le reverse et l'exploit dev
Web

HTTP/HTTPS en détail, méthodes, headers, cookies, CORS, Same-Origin Policy
Bases de données (SQL) et injections
2. Blue Team (défense)
Le blue team c'est la protection, la détection et la réponse aux incidents.

À apprendre :

SOC / SIEM : Splunk, Elastic Stack (ELK), Wazuh, Sentinel
Créer des règles de détection (Sigma, KQL, Splunk SPL)
EDR / XDR : comprendre comment fonctionnent CrowdStrike, Defender for Endpoint, SentinelOne
Analyse de logs : Windows Event Log, syslog, auditd
Forensic : acquisition mémoire (LiME, Volatility), analyse disque (Autopsy, Sleuth Kit)
Threat Intelligence : MITRE ATT&CK, CTI feeds, YARA rules
Network Defense : IDS/IPS (Snort, Suricata), honeypots
DFIR : réponse aux incidents, containment, eradication
Certifications possibles : Security+, Blue Team Level 1, GCIA, GNFA

3. Red Team (offensif)
Le red team simule des attaquants réels, avec une approche plus furtive et complète que le pentest classique.

À apprendre :

C2 (Command & Control) : comprendre et utiliser Cobalt Strike, Sliver, Havoc, Mythic
Persistence & Evasion : DLL hijacking, AMSI bypass, ETW patching, userland hooking
Active Directory exploitation : Kerberos attacks (AS-REP Roast, Kerberoasting, Golden/Silver Ticket), ACL abuse, DCSync
Phishing / Social Engineering : EvilGinx, GoPhish, setup de campagnes
Lateral Movement : PsExec, WMI, WinRM, SMB exec, DCOM
OSINT avancé : reconnaissance passive poussée
Certifications : OSCP (début), CRTO (Red Team Ops), PNPT, OSEP

4. Pentesting (test d'intrusion)
C'est le métier le plus courant. Un pentester trouve et exploite des vulnérabilités dans un périmètre défini.

À apprendre par domaine :



Domaine	Outils / Techniques
Web	Burp Suite, SQLi, XSS, SSRF, RCE, auth bypass
Network	Nmap, Nessus, Metasploit, cracking de mots de passe
AD / Windows	BloodHound, CrackMapExec, Impacket, Rubeus
Mobile	APKTool, Frida, Objection, MobSF
API	Postman, autorization testing, rate limiting bypass
Cloud	Pacu (AWS), ScoutSuite, CloudSploit, AzureHound
Méthodologie : PTES, OWASP Testing Guide, OSSTMM

5. Par où commencer ? Plan d'attaque recommandé
Voici un ordre que je suggère :



Étape	Sujet	Durée estimée
1	Réseaux (CCNA level) + Linux administration	2-3 mois
2	Python (scripting + outils réseau)	1-2 mois
3	Web fundamentals + OWASP Top 10 + Burp Suite	2 mois
4	Active Directory basics + BloodHound	1 mois
5	Hack The Box / TryHackMe (easy → medium)	Continu
6	Blue team : SIEM + logs + Windows Event Log	2 mois
7	Pentesting complet (OSCP style)	3-4 mois
8	Red team avancé (C2, evasion, AD exploitation)	3-6 mois
6. Ressources concrètes
Plateformes pour pratiquer :

TryHackMe (débutant) — parcours "Complete Beginner", "Jr Penetration Tester"
Hack The Box (intermédiaire+) — machines, Pro Labs
PentesterLab (web-focused)
LetsDefend (blue team / SOC)
PwnedLabs (cloud)
CyberDefenders (forensic)
Livres :

The Web Application Hacker's Handbook (Stuttard & Pinto)
Penetration Testing: A Hands-On Introduction to Hacking (Georgia Weidman)
Red Team Field Manual (Ben Clark)
The Hacker Playbook 3 (Peter Kim)
Windows Internals (Pavel Yosifovich)
Labs à monter toi-même :

GoAD (Game of Active Directory) — un lab AD vulnérable
Detection Lab (build pour blue team)
Home SOC avec Wazuh / Elastic
