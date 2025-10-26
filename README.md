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

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:







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


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
 ## Link:
 <img width="1919" height="1081" alt="Screenshot 2025-09-24 204300" src="https://github.com/user-attachments/assets/24cf559c-0a3f-4ce4-ab87-421815ebfc3c" />
 
 ## Intitle:
<img width="1913" height="1086" alt="Screenshot 2025-09-24 204234" src="https://github.com/user-attachments/assets/1ca6bbc0-cfac-40ec-a558-e8d86865f77e" />

## Inurl:
<img width="1918" height="1083" alt="Screenshot 2025-09-24 204142" src="https://github.com/user-attachments/assets/3d4e3f70-dcc5-448c-80d1-6ac536eda662" />

## Intext :
<img width="1918" height="1080" alt="Screenshot 2025-09-24 204035" src="https://github.com/user-attachments/assets/c4562c06-fb09-4d92-a830-2672568d930f" />

##  Filetype
<img width="1916" height="1029" alt="Screenshot 2025-09-24 204004" src="https://github.com/user-attachments/assets/40fb308a-07fc-4f05-9728-c7ab524e601f" />

##  Site
<img width="1917" height="1084" alt="Screenshot 2025-09-24 203918" src="https://github.com/user-attachments/assets/b3ca5736-da38-4d19-88e2-fcb442ceeab1" />

## CACHE:

 <img width="1918" height="1079" alt="Screenshot 2025-09-24 204322" src="https://github.com/user-attachments/assets/42b16705-c5aa-4c79-8d34-4dc9f32fc52a" />

## DNS Recon:
  
<img width="1012" height="574" alt="Screenshot 2025-10-26 180100" src="https://github.com/user-attachments/assets/c193efaa-19fd-4535-842a-de619aafdbe9" />

## dnsenum:
<img width="1020" height="788" alt="Screenshot 2025-10-26 180130" src="https://github.com/user-attachments/assets/a01a00a7-7ccc-4655-b6d8-a5d058c232bc" />

<img width="952" height="689" alt="Screenshot 2025-10-26 182824" src="https://github.com/user-attachments/assets/19e758fb-d265-4cbb-b788-9d2e5a7a9b48" />


## smtp-user-enum
<img width="792" height="358" alt="Screenshot 2025-10-26 180215" src="https://github.com/user-attachments/assets/83989afc-d8dc-4579-9f54-62c4e65d8e27" />
<img width="891" height="439" alt="Screenshot 2025-10-26 180206" src="https://github.com/user-attachments/assets/a56056cb-5c88-40ef-81b3-6de0c3df7719" />

## Telnet:
<img width="878" height="441" alt="Screenshot 2025-10-26 180225" src="https://github.com/user-attachments/assets/7cce001f-253d-446f-a34c-dbb933982f08" />

## nmap –script smtp-enum-users.nse:
<img width="764" height="277" alt="Screenshot 2025-10-26 180422" src="https://github.com/user-attachments/assets/06299816-5f07-4c4c-9d53-8f7214ac239a" />
 


  




## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

