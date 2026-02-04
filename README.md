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
<img width="1912" height="962" alt="image" src="https://github.com/user-attachments/assets/7aaf1956-5722-4de1-beeb-55ae9d50db46" />


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

<img width="1911" height="965" alt="image" src="https://github.com/user-attachments/assets/8523d90e-6bd3-479b-8a5b-935a3108cba0" />


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
<img width="1917" height="969" alt="image" src="https://github.com/user-attachments/assets/64178436-b109-4016-bf43-aad4907b1bbd" />


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
<img width="1919" height="965" alt="image" src="https://github.com/user-attachments/assets/286cabbf-9a0b-4f48-b5f0-0815e1adcdbe" />

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
<img width="1919" height="978" alt="image" src="https://github.com/user-attachments/assets/b5232d79-e513-404f-b917-b9e62a585d0b" />

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
<img width="1919" height="963" alt="image" src="https://github.com/user-attachments/assets/b11bbf97-5870-438f-b1fc-a3282ec2be6e" />

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
<img width="1919" height="972" alt="image" src="https://github.com/user-attachments/assets/1d5e36cc-9a93-4eb4-9fb6-d8324e7283ff" />

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
<img width="895" height="851" alt="image" src="https://github.com/user-attachments/assets/2cf6187d-55b5-4a40-afcc-faa1a2e1eeab" />


<img width="1005" height="694" alt="image" src="https://github.com/user-attachments/assets/28d2f52b-9fe6-4326-9232-9eceb47136a1" />






##dnsenum
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
<img width="805" height="831" alt="image" src="https://github.com/user-attachments/assets/be91f671-a934-4a80-a45c-179f695c889d" />


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

<img width="675" height="395" alt="image" src="https://github.com/user-attachments/assets/160f11fc-5bf7-4c05-bffe-b85aead6d506" />


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

<img width="430" height="240" alt="image" src="https://github.com/user-attachments/assets/c406673d-c320-4e67-971f-9614dd5632f1" />


select any username in the first column of the above file and check the same
<img width="677" height="395" alt="image" src="https://github.com/user-attachments/assets/a134ddd2-90fa-4817-ba50-f69da3ade0ed" />


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  
<img width="962" height="624" alt="image" src="https://github.com/user-attachments/assets/b09be21d-9d37-4e99-99d9-ca5c531ece18" />





## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
<img width="541" height="195" alt="image" src="https://github.com/user-attachments/assets/edfec9ed-dc0a-4dcf-89e7-32ffa509d0d3" />


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

