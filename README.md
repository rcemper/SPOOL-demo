## SPOOL Demo

SPOOL existed long before IRIS and ObjectScript   
It is a simple device that allows you to write to the Global ^SPOOL 

For daily use you should know   
Device = 2    
it has an integer documentId (default=1)   
it has an integer lineNumber (default =1)    
you use it by  
```
open 2:<docid>
use 2 write . . . .  
close 2
```
Online documentation on [SPOOL](http://docs.intersystems.com/latest/csp/docbook/DocBook.UI.Page.cls?KEY=GIOD_spool) is complete and tells you almost all details.   

### Prerequisites  
Make sure you have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and [Docker desktop](https://www.docker.com/products/docker-desktop) installed.   
### Installation   
Clone/git pull the repo into any local directory  
```
 git clone https://github.com/rcemper/SPOOL-demo-ZPM.git   
```
Open the terminal in this directory create teh container and run it:   
```
 docker-compose up -d
```
### How to use it:   

Open a session in your container   
```
 docker-compose iris iris session iris
 ```
Details for testing are described in DC article [SPOOL - the forgotten device](https://community.intersystems.com/post/spool-forgotten-device)   
