---
layout:	post
title:	"Extracting Subscribers list from Telegram Channel"
date:	2019-04-12
tag: code
---

*Sharing the code to extract details of subscribers to your own telegram channel.*

### **1. Install telethon**

pip3 install telethonIf you don’t have pip installed, execute this first:

`sudo apt install python3-pip`

### 2. Create a client

Before working with Telegram’s API, you need to get your own API ID and hash:

1. Follow [this link](https://my.telegram.org/) and login with your phone number.
2. Click under API Development tools.
3. A *Create new application* window will appear. Fill in your application details. There is no need to enter any *URL*, and only the first two fields (*App title* and *Short name*) can currently be changed later.
4. Click on *Create application* at the end. Remember that your **API hash is secret** and Telegram won’t let you revoke it. Don’t post it anywhere!
([Source](https://telethon.readthedocs.io/en/latest/extra/basic/creating-a-client.html))

### 3. Run code

Run this python code, replacing the api\_id, api\_hash, channel and phone number details:

<script src="https://gist.github.com/liyanasahir/1411b833d0dcfbf7f5533aa058c3bbfa.js"></script>

Tada! You should now have a list of subscribers to your channel along with their names displayed on your terminal.
