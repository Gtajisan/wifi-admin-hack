### স্বাগতম আপনাকে, এর নতুন আরেকটি command এ। আজ দেখাবো কানেক্ট থাকা TP-Link রাউটারের পাসওয়ার্ড কিভাবে বের করতে হয় Config.bin ফাইল Extart করে। 
এটা আমরা Termux এর মাধ্যমে করবো। 

আমরা রাউটারের অ্যাডমিন প্যানেল এর Username & Password দেখতে পারবো Config.bin ফাইল এর মাধ্যমে। এমনকি wps pin ও দেখা যাবে এটার মাধ্যমে। 

![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/b0050088-e78e-46fc-981d-a045ea4f2c0f)


# TP-LINK
A simple python tool for crack old TP-Link routers.

# Feature's
+ **Find router model or hostname**
+ **Find connection username**
+ **Find connection password**
+ **Find admin panel username**
+ **Find admin panel password**

### install one line 
```
pkg update && pkg upgrade -y && pkg install git python -y && pip3 install pycryptodome && git clone https://github.com/Gtajisan/wifi-admin-hack && cd admin-hack.py && python admin-hack.py -h
```

### Installation :

```bash
pkg update && pkg upgrade -y
pkg install git python -y
pip3 install pycryptodome
git clone https://github.com/Gtajisan/wifi-admin-hack
```
```
cd wifi-admin-hack
chmod +x admin-hack.py
```

#### Help : 
```
python admin-hack.py -h
```

#### Usage : 
```
python admin-hack.py conf.xml [ you ip ] 
```

#### Note: 
+ **First turn on your Wifi.**
+ **Connect to the wifi.**
+ **Only works on TP-LINK old routers**
+ **Not working on new router**

### Thanks For Star🙏👨‍💻
for using my tool 💛🚹

