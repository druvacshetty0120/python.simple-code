import urllib.request, json
url = "https://api.ipify.org?formate=json"
data = json.loads(urllib.request.urlopen(url).read())
print(f"Your public IP address is:{data['ip']}")
