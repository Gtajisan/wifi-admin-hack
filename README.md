### স্বাগতম আপনাকে, এর নতুন আরেকটি command এ। আজ দেখাবো কানেক্ট থাকা TP-Link রাউটারের পাসওয়ার্ড কিভাবে বের করতে হয় Config.bin ফাইল Extart করে। 
এটা আমরা Termux এর মাধ্যমে করবো। 

আমরা রাউটারের অ্যাডমিন প্যানেল এর Username & Password দেখতে পারবো Config.bin ফাইল এর মাধ্যমে। এমনকি wps pin ও দেখা যাবে এটার মাধ্যমে। 

https://1.bp.blogspot.com/-ed7DWoWN1kc/X_cXPynCNbI/AAAAAAAAAMg/Wq_9UssEUogXARMI60uKdtVsLFRPR_JxQCLcBGAsYHQ/s1280/20210107_201213.jpg

তো চলুন শুরু করি :

### 1. প্রথমে নিচের লিংক থেকে এপ্প টা ডাউনলোড করে নিন ?
https://exe.io/9Hkrn
### 2. ইনস্টল করে ওপেন করুন এবং ল্যাঙ্গুয়েজ English সিলেক্ট করুন ?
https://lh3.googleusercontent.com/-hsu5bVqHPgo/X_bXiZcdmTI/AAAAAAAAAKU/wwOBraStk0MoyI1mZJ5Gme7ppEXpT5eRwCLcBGAsYHQ/image.png
### 3. পার্মিসন Allow করুন?
https://lh3.googleusercontent.com/-fC8wQVC51Go/X_bYcAJ08kI/AAAAAAAAAKc/ZzAeCoEKadUJx8x_HLB1YsoNTYWY2a3lgCLcBGAsYHQ/image.png
### 4. এরপর  Select এ ক্লিক করুন ?
https://lh3.googleusercontent.com/-6ntmf8IvfeE/X_bZaVqhmvI/AAAAAAAAAKw/0zgKdWcl4T8j8ZGoQWevgQUEYXKbGWLdQCLcBGAsYHQ/image.png
### 5. প্লাস আইকনে ক্লিক করুন ?
https://lh3.googleusercontent.com/-VIC-oDWtKQs/X_bZ6-35BZI/AAAAAAAAAK4/-q_bHSyIg98GD5AZqqI9ynHWpRuXrjOugCLcBGAsYHQ/image.png
### 6. Add Link এ ক্লিক করুন ?
https://lh3.googleusercontent.com/-3DW2hgKrBB8/X_baqDyGb-I/AAAAAAAAALE/8lVJaTkgIAYHisv4pSRcn_y4IbDv-p8EQCLcBGAsYHQ/image.png
### 7. এরপর উপরের ফাঁকা বক্সে http://192.168.0.1/cgl/conf.bin? টাইপ করে Connect এ ক্লিক করুন?
https://lh3.googleusercontent.com/-iBg2OIEuX7I/X_bbg7TLRII/AAAAAAAAALM/nELFnXb8ht07c-BChwcEZK5tHiwHP7QwQCLcBGAsYHQ/image.png
### 8. এরপর Start এ ক্লিক করুন ফাইল টা  ডাউনলোড হয়ে যাবে ?
https://lh3.googleusercontent.com/-roXf_nCPBjs/X_bcydGL9FI/AAAAAAAAALY/umMmFEvIeTQ5eqEtWG3gEO6BSY3P2GOzQCLcBGAsYHQ/image.png

### 9. ডাউনলোড করা ফাইল টা ইন্টারনাল স্টোরেজের হোম ডিরেক্টরি তে রাখুন?
https://lh3.googleusercontent.com/-8wfY1ZHxI2Q/X_bdciNdEuI/AAAAAAAAALg/GlxqAc3J4g0uZX7Dw5MOabBTOnq1Tf9xgCLcBGAsYHQ/image.png
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
https://lh3.googleusercontent.com/-8dlDMC1gMKw/X_cPhMlI7sI/AAAAAAAAAL0/y_CnnqEMYdklMl0Vn9OH9WWdifSGF3iSgCLcBGAsYHQ/image.png
```
cat 1.xml
```
### এটা এন্টার করার পর নিচের মতো ইন্টারফেস শো হবে, যেখানে রাউটারের সব ইনফরমেশন থাকবে।
এখানে Device Password হলো  Wifi Password এবং  PreShareKey হলো WPS  পিন।
https://lh3.googleusercontent.com/-xCuzVIEX0Kw/X_cRe-gNXeI/AAAAAAAAAMM/hE-Juzsa16023j66sYbqjbjeGQQN0AfLACLcBGAsYHQ/image.png
### এবং তার নিচে রাউটারের Username & Password দেখতে পাবেন।
https://lh3.googleusercontent.com/-BmPQR4aDvUk/X_cSFo_wFSI/AAAAAAAAAMU/_36Jvm5-U3MgpmsGy-CmeLUjGoCuNAfrwCLcBGAsYHQ/image.png


