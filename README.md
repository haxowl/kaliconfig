### This is my personal config, nothing fancy and far from perfect but it works for me and it might work for you too. 
### Tested on Kali 2025.2

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
**Bloodhound Community Edition**
- Using the terminal
```
bloodhound-setup
```

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
- bloodyad
- burp extensions: 
content type converter
JS Link Finder
param miner
backlash powered scanner
Paste curl to repeater