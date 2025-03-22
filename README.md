## **VMware Config**
- Combination of 4 processors total
- Side Channel mitigations not enabled
- Fit all virtual machine memory into reserved host RAM

## **Basic Usage**
- Using the terminal
```
git clone https://github.com/haxowl/kaliconfig.git
cd kaliconfig
chmod 777 install.sh
./install.sh
```

## **Additional Config**
**Bloodhound**
- Using the terminal
```
sudo neo4j console
```
- Go to: http://localhost:7474/
- Log in with the following credentials: neo4j:neo4j
- Follow the config wizard

**Foxyproxy** 
- Navigate to: Import Proxy List
- Enter the following line in the textbox and save
```
http://127.0.0.1:8080?color=0000ff&title=BURP&enabed=true
```


## **Known Issues:**
- Selected text is automatically attached to clipboard when copying/pasting from guestVM to host (text editors, terminal, etc). Might be intended X11 behaviour.
- Using CAT to open one of the tmux logging files creates 40k lines of text

## **ToDo**
- xfconf clock-19 make show time the date, time font bold
- xfconf panel1 never hide, background solid black
- disable firefox bookmark bar
- Ask whether to open or save files, pdf etc firefox
- copy idorfuzz.txt to seclists/fuzzing
- remove imwheel
- install pspy, make a single folder with all needed binaries https://github.com/itm4n/PrivescCheck
- p10k remove right, move time to left
