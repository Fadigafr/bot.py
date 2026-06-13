import schedule
import time
import numpy as np
import requests

def send_message(message):
    url = "https://api.telegram.org/botTON_TOKEN/sendMessage"

    requests.post(url, data={
        "chat_id": "TON_CHAT_ID",
        "text": message
    })

TOKEN = "TON(job)TOKEN = "TON_TOKEN"

while True:
    schedule.run_pending()
    time.sleep(60)
CHAT_ID = "TON_CHAT_ID"

def send_message(text):
    url = f"https://api.telegram.org/bot{TOKEN}/sendMessage"
    requests.post(url, data={"chat_id": CHAT_ID, "text": text})

def job():
    s1 = np.random.randint(1, 3)
    s2 = np.random.randint(0, 2)

    msg = f" PRONO AUTO : {s1}-{s2}"
    send_message(msg)


