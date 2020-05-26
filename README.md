# Description
A voting bot written in python 3.x for strawpoll.com. It uses a proxy list to vote multiple times in a survey.
It works on Mac, Windows and Linux.

### Features
- Easy to use command line driven program
- No proxies are given. More can be easily added
- The program saves already used proxies in an xml file to enhance the voting speed dramatically

# Usage
```
Usage: Main.py [options]

Options:
  -h, --help            show this help message and exit
  -v VOTES, --votes=VOTES
                        number of votes to give
  -s SURVEY, --survey=SURVEY
                        id of the survey
  -t TARGET, --target=TARGET
                        checkbox to vote for
  -f, --flush           Deletes skipping proxy list
```

### Example
```
python Main.py -v 100 -s d9deecxy -t 7kr2b8s3ke5f

```

# How to install it ?
Download the zip or clone it with git then install the required library with:
```
pip install requests
```

## What is pip? I don't understand!
If you don't understand how to install a library also called a "module" in Python please go checkout YouTube: 
[How to download and install Python Packages and Modules with Pip](https://www.youtube.com/watch?v=jnpC_Ib_lbc)

## Proxy timeout?
If a proxy times out it means the server is not reachable anymore. The predefined list given with this repository most likely only has
proxies that are not online anymore thus you get many proxy timeouts. To get a new list of proxies just search for proxy lists on the web. 

# How to add proxies to the list
Add new proxies to the file proxy1.xml

# How do I get the survey id and the target ?
The survey id is always in the url pointing to your survey for example: https://strawpoll.com/abbcw17 then abbcw17 would be the id.
To find the target you have to right click the checkbox you want to vote for, then go to inspect element and search for a
'checkbox' input value like 7kr2b8s3ke5f. This is the checkbox id.
