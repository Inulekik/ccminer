   
RPSqsXTKqsi9vNFTZMg5YNtbEhEeFqArGw

<a href=https://f-droid.org/repo/com.termux_1020.apk>TERMUX FDROID</a> <br>

<a href=(https://download.apkcombo.com/com.sugarapps.autostartmanager/AutoStart%20App%20Manager_5.1_apkcombo.com.apk?ecp=Y29tLnN1Z2FyYXBwcy5hdXRvc3RhcnRtYW5hZ2VyLzUuMS8zMy42MzY4ZTMyMzc2YWU5YzhhODNiNzhiZDEwNmRhZTg2ODllNWFiZTA1LmFwaw==&iat=1726939758&sig=957b23ed630ea4426123cae92ee7118e&size=8254287&from=cf&version=old&lang=id&fp=ff994c381f15870264356c18af4dc641&ip=)> AutostartApp</a> <br>

<a href=https://f-droid.org/repo/com.termux.boot_1000.apk> Termux Boot</a> <br>

## [ install update ]
```
yes | pkg update && pkg upgrade
```

## [ install libs]
```
yes | pkg install libjansson nano git
```

## [ Clone Repo]
```
git clone https://github.com/inulekik/ccminer
cd ccminer
chmod +x ccminer start.sh
```

## [ Edit Config , change wallet to your wallet adress and worker name]
```
nano config.json
```

## [ Autorun ] [ CCminer ]

```
cd ..
nano ../usr/etc/bash.bashrc
```

## [ put this code ]
```
cd ccminer/&&./start.sh

```

### create dir and boot script
```
mkdir ~/.termux/boot
cd ~/.termux/boot
nano termux.sh
```
### type this in sh , ctrl x and save reboot phone. 
```
#!/data/data/com.termux/files/usr/bin/sh
termux-wake-lock
~/ccminer/start.sh >> ~/miner.log 2>&1
```

