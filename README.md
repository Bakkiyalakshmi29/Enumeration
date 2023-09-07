# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
## OUTPUT::
![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/4ee07efd-92c0-4e56-9e21-9e238cebc19a)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
## OUTPUT:
![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/08d28be8-24d0-4577-9534-96e1a3243bf1)

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
## OUTPUT:
![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/116481af-b5d4-407d-bd95-3ae1d919cff7)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
## OUTPUT:
![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/9647a9c7-9281-4f99-8579-100cdd7b1342)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
## OUTPUT:
![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/945f137f-5c00-467c-b374-8746801a4ddd)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
## OUTPUT:
![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/3b3ee9bc-0a5c-40a1-a278-f649753ca705)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
## OUTPUT:
![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/0142b241-8d2a-4da9-a28c-047a052f620a)
 
## DNS Enumeration
## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/e087a4fc-bc15-4cf4-9c0d-9c57b55ac002)

![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/1687d96e-cbc7-4911-ac9a-de76f6f332d5)

## dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
## OUTPUT:

![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/dbda7810-a013-41f4-af3d-f32897f1d886)

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/b656c569-a68b-48c9-9bfe-9dbcb53545db)

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/b95c444b-7ac0-4ca7-9c3d-1f48ce806fcd)

select any username in the first column of the above file and check the same

![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/12b1baeb-ee78-424c-9207-906059343c23)

## Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output

![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/eabcabf7-0cdf-4896-b415-e6cae71e8adf)

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
## OUTPUT

![image](https://github.com/Bakkiyalakshmi29/Enumeration/assets/119406233/3c901919-748c-41da-abfd-1f6fa3350fa1)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

