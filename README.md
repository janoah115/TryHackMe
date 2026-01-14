# TryHackMe
Documentation of concepts and lessons learn through THM

Hacktivities 1 - Pre Security

Concepts:
Cyber security basics
Networking basics and weaknesses
The web and common attacks
Learn to use the Linux operating system

----------------------Offensive Security Intro --------------------------

Used ubuntu cli to find a hidden bank admin page:
gobuster -u http://fakebank.thm -w wordlist.txt dir

After finding the hidden page http://fakebank.thm/bank-transfer, we had authorized access to transfer money

============================
----------------------Defensive Security Intro --------------------------

User cyber security awareness: Training users about cyber security helps protect against attacks targeting their systems.
Documenting and managing assets: We need to know the systems and devices we must manage and protect adequately.
Updating and patching systems: Ensuring that computers, servers, and network devices are correctly updated and patched against any known vulnerability (weakness).
Setting up preventative security devices: firewall and intrusion prevention systems (IPS) are critical components of preventative security. Firewalls control what network traffic can go inside and what can leave the system or network. IPS blocks any network traffic that matches present rules and attack signatures.
Setting up logging and monitoring devices: Proper network logging and monitoring are essential for detecting malicious activities and intrusions. If a new unauthorized device appears on our network, we should be able to detect it.

Some of the main areas of interest for a SOC are:

Vulnerabilities: Whenever a system vulnerability (weakness) is discovered, it is essential to fix it by installing a proper update or patch. When a fix is unavailable, the necessary measures should be taken to prevent an attacker from exploiting it. Although remediating vulnerabilities is vital to a SOC, it is not necessarily assigned to them.
Policy violations: A security policy is a set of rules required to protect the network and systems. For example, it might be a policy violation if users upload confidential company data to an online storage service.
Unauthorized activity: Consider the case where a user’s login name and password are stolen, and the attacker uses them to log into the network. A SOC must detect and block such an event as soon as possible before further damage is done.
Network intrusions: No matter how good your security is, there is always a chance for an intrusion. An intrusion can occur when a user clicks on a malicious link or when an attacker exploits a public server. Either way, when an intrusion occurs, we must detect it as soon as possible to prevent further damage.

4 major phases of the incident response process are:

Preparation: This requires a team trained and ready to handle incidents. Ideally, various measures are put in place to prevent incidents from happening in the first place.
Detection and Analysis: The team has the necessary resources to detect any incident; moreover, it is essential to analyze any detected incident further to learn about its severity.
Containment, Eradication, and Recovery: Once an incident is detected, it is crucial to stop it from affecting other systems, eliminate it, and recover the affected systems. For instance, when we notice that a system is infected with a computer virus, we would like to stop (contain) the virus from spreading to other systems, clean (eradicate) the virus, and ensure proper system recovery.
Post-Incident Activity: After a successful recovery, a report is produced, and the lesson learned is shared to prevent similar future incidents.

Malware analysis aims to learn about such malicious programs using various means:

Static analysis works by inspecting the malicious program without running it. This usually requires solid knowledge of assembly language (the processor’s instruction set, i.e., the computer’s fundamental instructions).
Dynamic analysis works by running the malware in a controlled environment and monitoring its activities. It lets you observe how the malware behaves when running.

Defensive Lab 1:

Used a SIEM to find an unauthorized login attempt and check the reputation/location of the IP at https://ip-scanner.thm/search
After validating that the IP was malicious, we escalated to the SOC team lead, who gave permission to block the IP in the firewall.

----------------------Careers in Cyber--------------------------


