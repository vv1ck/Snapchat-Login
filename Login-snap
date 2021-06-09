import requests,re,html
from user_agent import generate_user_agent
r=requests.session()
URL1="https://www.google.com/recaptcha/enterprise/anchor?ar=1&k=6LezjdAZAAAAAD1FaW81QpkkplPNzCNnIOU5anHw&co=aHR0cHM6Ly9hY2NvdW50cy5zbmFwY2hhdC5jb206NDQz&hl=ar&v=CdDdhZfPbLLrfYLBdThNS0-Y&size=invisible&badge=inline&cb=3b4l61jprpqj"
URLOG = 'https://accounts.snapchat.com/accounts/login'
user = input('Enter user: ')
pess = input('Enter pass : ')





def LOGOUT():
  global Token
  OUTurl = 'https://accounts.snapchat.com/accounts/logout'
  OUThead = {
  'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
  'accept-encoding': 'gzip, deflate, br',
  'accept-language': 'en-US,en;q=0.9',
  'cache-control': 'max-age=0',
  'content-length': '42',
  'content-type': 'application/x-www-form-urlencoded',
  'cookie': 'xsrf_token='+Token+'; _ga=GA1.2.1082754574.1621993969; _scid=5d4ad0b7-593a-48ec-8cbf-13ccbde93a64; Marketing=true; Performance=true; Preferences=true; sc-cookies-accepted=true; _gcl_au=1.1.1465707485.1621993991; web_client_id=dca8edfb-668f-4a82-9299-433867d86f07; _sca={%22cid%22:%2251b3384d-7afe-4d53-98f6-4984cbf78856%22%2C%22token%22:%22v1.key.2021-03-06_0mryaaW4.iv.D+tP1JGTt7YAX5ev.6IGIgwus60tI5YiglS2eRSqpSBaT+kUFKp5N7OXkXX1CaQahNeLMtPKgqWiBYWhQDfqmHtvNSEh/S2n2ZmOemdCHBnoAbFSSlrVUXTyoCXTxbdWZ%22}; _gid=GA1.2.289791362.1623064568; _gat_UA-41740027-4=1; sc_at=v2|H4sIAAAAAAAAAE3GyREAIQgEwIioAhkuw3FXojB4v/ar1bfF10oiDQJi0SoYbf91WFZXxhHwFB/KDvM8T/kCGEaRcEAAAAA=; _sctr=1|1623024000000; __Host-sc-a-session=MDAxOjAwMjpDz82YT21MfQvUre-tSs71OuW6XkvsxHm74C7Gbx0Qqs_7Bu339apvTZcgEt3izycguMMxuO2v0EwT2Y112OvBEw; sc-a-nonce=4e2f781e-5f57-455f-963b-321bd618a3e4; __Host-sc-a-nonce=4e2f781e-5f57-455f-963b-321bd618a3e4; sc-a-csrf=true',
  'origin': 'https://accounts.snapchat.com',
  'referer': 'https://accounts.snapchat.com/',
  'sec-ch-ua': '" Not;A Brand";v="99", "Google Chrome";v="91", "Chromium";v="91"',
  'sec-ch-ua-mobile': '?0',
  'sec-fetch-dest': 'document',
  'sec-fetch-mode': 'navigate',
  'sec-fetch-site': 'same-origin',
  'sec-fetch-user': '?1',
  'upgrade-insecure-requests': '1',
  'user-agent': generate_user_agent()}
  
  OUTdata = {
    'xsrf_token':Token}
  
  OUT=r.post(OUTurl,headers=OUThead,data=OUTdata)
  print('===========')
  print(OUT.text)
  print(OUT)


def LOGIN():
  global Done,Heda,Done2,Ok,Token
  Ok ="".join(re.findall('data-xsrf="(.*?)"', str(r.get(URLOG, headers=Heda).text)))
  LOGhed = {
    'Host': 'accounts.snapchat.com',
    'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
    'Accept-Encoding': 'gzip, deflate',
    'Accept-Language': 'en,en-US;q=0.9,en;q=0.8','Connection': 'close',
    'Cookie': 'xsrf_token='+Ok+'; web_client_id=5b6ac8a4-e43a-4b04-af42-56d1690da690; _scid=4545dfd0-ff7e-46ea-a282-a8e572282ef3; _sca={%22cid%22:%226d2ee5f8-79ba-486d-b65f-579d272f91ac%22%2C%22token%22:%22v1.key.2021-03-06_cfUM3WwH.iv.LgicCBtnBULigL5T.iyjsJ8WtKqKJJtMdiPBN0NF0LdLgHqeH1VqS5WeTgRhGIEqCzTibnJYPn08FjayPHZzu56GLXE0cCBiHxisJSwpOzdg9GqpoBBvA+IX3E+FwJQWT%22}; sc-cookies-accepted=true; Preferences=true; Performance=true; Marketing=true; _ga=GA1.2.224847189.1623034622; _gid=GA1.2.1966742317.1623034622; sc_at=v2|H4sIAAAAAAAAAE3GsRHAMAgDwIm4E1hWkW1CgCk8vNt89axOEmWj2MZ3y3JI+7pGDvRkHiceVywsKuL8igsQq6SxQAAAAA==; _sctr=1|1623013200000; _gcl_au=1.1.1819942820.1623034641; sc-a-csrf=true; _gali=login_form; _gat_UA-41740027-4=1',
    'Referer': 'https://accounts.snapchat.com/',
    'Origin': 'https://accounts.snapchat.com',
    'Content-Length': '3839',
    'Cache-Control': 'max-age=0',
    'Sec-Ch-Ua': '\\" Not A;Brand\\";v=\\"99\\", \\"Chromium\\";v=\\"90\\"',
    'Sec-Ch-Ua-Mobile': '?0',
    'Upgrade-Insecure-Requests': '1',
    'Content-Type': 'application/x-www-form-urlencoded','Sec-Fetch-Site': 'same-origin','Sec-Fetch-Mode': 'navigate','Sec-Fetch-User': '?1','Sec-Fetch-Dest': 'document',
    "User-Agent": generate_user_agent()}
  LOGdat = {
    'username':user,'password':pess,
    'xsrf_token':Ok,
    'continue':'%2Faccounts%2Fwelcome',
    'g-recaptcha-response':Done2,
    'g-recaptcha-response':Done2}
  Go3 = r.post(URLOG,headers=LOGhed,data=LOGdat)
  
  if 'My Data' in Go3.text:
    print('======')
    print('[+] Login succeeded')
  elif 'Delete My Account' in Go3.text:
    print('[+] Login succeeded')
  elif 'change_password' in Go3.text:
    print('[+] Login succeeded')
  elif '"Cannot find the user."' in Go3.text:
    print('[-] Account not found !')
  elif '"That&#39;s not the right password."' in Go3.text:
    print(Go3.text)
    print('[-] Incorrect password !')
  elif 'phone='in Go3.text:
    print('[+] secure account ..')
  else:
    print(Go3.text)
    
def captcha():
  global Done,Heda,Done2
  URL2 = 'https://www.google.com/recaptcha/enterprise/reload?k=6LezjdAZAAAAAD1FaW81QpkkplPNzCNnIOU5anHw'
  HEDsp = {
    "Accept": "*/*",
    "accept-encoding": "gzip, deflate, br",
    "accept-language": "fa,en;q=0.9,en-GB;q=0.8,en-US;q=0.7",
    "content-length": "5628",
    "origin": "https://www.google.com",
    "User-Agent": generate_user_agent(),
    "Pragma": "no-cache",
    "sec-fetch-dest": "empty",
    "sec-fetch-mode": "cors",
    "sec-fetch-site": "same-origin",
    "referer": "https://www.google.com/recaptcha/enterprise/anchor?ar=1&k=6LezjdAZAAAAAD1FaW81QpkkplPNzCNnIOU5anHw&co=aHR0cHM6Ly9hY2NvdW50cy5zbmFwY2hhdC5jb206NDQz&hl=ar&v=CdDdhZfPbLLrfYLBdThNS0-Y&size=invisible&badge=inline&cb=3b4l61jprpqj"}
  DATsp = {
    "v":"CdDdhZfPbLLrfYLBdThNS0-Y",	
    "reason":"q",
    "c":Done,
    "k":"",
    "co":"",
    "hl":"en",
    "size":"invisible",
    "chr":"%5B89%2C64%2C27%5D",
    "vh":"13599012192",
    "bg":"!q62grYxHRvVxjUIjSFNd0mlvrZ-iCgIHAAAB6FcAAAANnAkBySdqTJGFRK7SirleWAwPVhv9-XwP8ugGSTJJgQ46-0IMBKN8HUnfPqm4sCefwxOOEURND35prc9DJYG0pbmg_jD18qC0c-lQzuPsOtUhHTtfv3--SVCcRvJWZ0V3cia65HGfUys0e1K-IZoArlxM9qZfUMXJKAFuWqZiBn-Qi8VnDqI2rRnAQcIB8Wra6xWzmFbRR2NZqF7lDPKZ0_SZBEc99_49j07ISW4X65sMHL139EARIOipdsj5js5JyM19a2TCZJtAu4XL1h0ZLfomM8KDHkcl_b0L-jW9cvAe2K2uQXKRPzruAvtjdhMdODzVWU5VawKhpmi2NCKAiCRUlJW5lToYkR_X-07AqFLY6qi4ZbJ_sSrD7fCNNYFKmLfAaxPwPmp5Dgei7KKvEQmeUEZwTQAS1p2gaBmt6SCOgId3QBfF_robIkJMcXFzj7R0G-s8rwGUSc8EQzT_DCe9SZsJyobu3Ps0-YK-W3MPWk6a69o618zPSIIQtSCor9w_oUYTLiptaBAEY03NWINhc1mmiYu2Yz5apkW_KbAp3HD3G0bhzcCIYZOGZxyJ44HdGsCJ-7ZFTcEAUST-aLbS-YN1AyuC7ClFO86CMICVDg6aIDyCJyIcaJXiN-bN5xQD_NixaXatJy9Mx1XEnU4Q7E_KISDJfKUhDktK5LMqBJa-x1EIOcY99E-eyry7crf3-Hax3Uj-e-euzRwLxn2VB1Uki8nqJQVYUgcjlVXQhj1X7tx4jzUb0yB1TPU9uMBtZLRvMCRKvFdnn77HgYs5bwOo2mRECiFButgigKXaaJup6NM4KRUevhaDtnD6aJ8ZWQZTXz_OJ74a_OvPK9eD1_5pTG2tUyYNSyz-alhvHdMt5_MAdI3op4ZmcvBQBV9VC2JLjphDuTW8eW_nuK9hN17zin6vjEL8YIm_MekB_dIUK3T1Nbyqmyzigy-Lg8tRL6jSinzdwOTc9hS5SCsPjMeiblc65aJC8AKmA5i80f-6Eg4BT305UeXKI3QwhI3ZJyyQAJTata41FoOXl3EF9Pyy8diYFK2G-CS8lxEpV7jcRYduz4tEPeCpBxU4O_KtM2iv4STkwO4Z_-c-fMLlYu9H7jiFnk6Yh8XlPE__3q0FHIBFf15zVSZ3qroshYiHBMxM5BVQBOExbjoEdYKx4-m9c23K3suA2sCkxHytptG-6yhHJR3EyWwSRTY7OpX_yvhbFri0vgchw7U6ujyoXeCXS9N4oOoGYpS5OyFyRPLxJH7yjXOG2Play5HJ91LL6J6qg1iY8MIq9XQtiVZHadVpZVlz3iKcX4vXcQ3rv_qQwhntObGXPAGJWEel5OiJ1App7mWy961q3mPg9aDEp9VLKU5yDDw1xf6tOFMwg2Q-PNDaKXAyP_FOkxOjnu8dPhuKGut6cJr449BKDwbnA9BOomcVSztEzHGU6HPXXyNdZbfA6D12f5lWxX2B_pobw3a1gFLnO6mWaNRuK1zfzZcfGTYMATf6d7sj9RcKNS230XPHWGaMlLmNxsgXkEN7a9PwsSVwcKdHg_HU4vYdRX6vkEauOIwVPs4dS7yZXmtvbDaX1zOU4ZYWg0T42sT3nIIl9M2EeFS5Rqms_YzNp8J-YtRz1h5RhtTTNcA5jX4N-xDEVx-vD36bZVzfoMSL2k85PKv7pQGLH-0a3DsR0pePCTBWNORK0g_RZCU_H898-nT1syGzNKWGoPCstWPRvpL9cnHRPM1ZKemRn0nPVm9Bgo0ksuUijgXc5yyrf5K49UU2J5JgFYpSp7aMGOUb1ibrj2sr-D63d61DtzFJ2mwrLm_KHBiN_ECpVhDsRvHe5iOx_APHtImevOUxghtkj-8RJruPgkTVaML2MEDOdL_UYaldeo-5ckZo3VHss7IpLArGOMTEd0bSH8tA8CL8RLQQeSokOMZ79Haxj8yE0EAVZ-k9-O72mmu5I0wH5IPgapNvExeX6O1l3mC4MqLhKPdOZOnTiEBlSrV4ZDH_9fhLUahe5ocZXvXqrud9QGNeTpZsSPeIYubeOC0sOsuqk10sWB7NP-lhifWeDob-IK1JWcgFTytVc99RkZTjUcdG9t8prPlKAagZIsDr1TiX3dy8sXKZ7d9EXQF5P_rHJ8xvmUtCWqbc3V5jL-qe8ANypwHsuva75Q6dtqoBR8vCE5xWgfwB0GzR3Xi_l7KDTsYAQIrDZVyY1UxdzWBwJCrvDrtrNsnt0S7BhBJ4ATCrW5VFPqXyXRiLxHCIv9zgo-NdBZQ4hEXXxMtbem3KgYUB1Rals1bbi8X8MsmselnHfY5LdOseyXWIR2QcrANSAypQUAhwVpsModw7HMdXgV9Uc-HwCMWafOChhBr88tOowqVHttPtwYorYrzriXNRt9LkigESMy1bEDx79CJguitwjQ9IyIEu8quEQb_-7AEXrfDzl_FKgASnnZLrAfZMtgyyddIhBpgAvgR_c8a8Nuro-RGV0aNuunVg8NjL8binz9kgmZvOS38QaP5anf2vgzJ9wC0ZKDg2Ad77dPjBCiCRtVe_dqm7FDA_cS97DkAwVfFawgce1wfWqsrjZvu4k6x3PAUH1UNzQUxVgOGUbqJsaFs3GZIMiI8O6-tZktz8i8oqpr0RjkfUhw_I2szHF3LM20_bFwhtINwg0rZxRTrg4il-_q7jDnVOTqQ7fdgHgiJHZw_OOB7JWoRW6ZlJmx3La8oV93fl1wMGNrpojSR0b6pc8SThsKCUgoY6zajWWa3CesX1ZLUtE7Pfk9eDey3stIWf2acKolZ9fU-gspeACUCN20EhGT-HvBtNBGr_xWk1zVJBgNG29olXCpF26eXNKNCCovsILNDgH06vulDUG_vR5RrGe5LsXksIoTMYsCUitLz4HEehUOd9mWCmLCl00eGRCkwr9EB557lyr7mBK2KPgJkXhNmmPSbDy6hPaQ057zfAd5s_43UBCMtI-aAs5NN4TXHd6IlLwynwc1zsYOQ6z_HARlcMpCV9ac-8eOKsaepgjOAX4YHfg3NekrxA2ynrvwk9U-gCtpxMJ4f1cVx3jExNlIX5LxE46FYIhQ"}
  GO2 = r.post(URL2,headers=HEDsp, data=DATsp)
  Done2 = "".join(re.findall("\[\"rresp\",\"(.*?)\"", str(GO2.text)))
  LOGIN()
def recaptcha():
  global Done,Heda
  Heda = {
    "Accept": "*/*",
    "Pragma": "no-cache",
    "User-Agent": generate_user_agent()}
    
  GO1 = r.get(URL1, headers=Heda)
  Done = "".join(re.findall("type=\"hidden\" id=\"recaptcha-token\" value=\"(.*?)\"", str(GO1.text))) 
  captcha()
recaptcha()
