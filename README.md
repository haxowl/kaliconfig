### This is my personal config, nothing fancy and far from perfect but it works for me and it might work for you too. 
### Tested on Kali 2025.1a

Credits: thegoodhackertv ippsec pimpmykali blacklanternsecurity

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

**Subfinder** 
- Add sources to:
```
.config/subfinder/provider-config.yaml
```

**Network config if needed**
```
sudo nmcli con mod 'Wired connection 1' ipv4.addresses 192.168.1.99/24 ipv4.gateway 192.168.1.1 ipv4.dns "1.1.1.1 8.8.8.8" ipv4.method manual
sudo nmcli con up 'Wired connection 1'
```

## **Known Issues:**
- Selected text is automatically attached to clipboard when copying/pasting from guestVM to host (text editors, terminal, etc). Might be intended X11 behaviour.
- Using CAT to open one of the tmux logging files creates 40k lines of text

## **ToDo**
- jython
- burp extensions: 
content type converter
JS Link Finder
param miner
backlash powered scanner