# Auto Install
File ***Auto_install*** is script for auto installation of most used tools of linux (Ubunu/Kali)

# Python Scripts
## Requests path and append values
```
import requests path = ''
host = 'http://10.10.169.100:3000/'
value = ''
while(path is not 'end'):
  response = requests.get(host + path)
  print(response)
  json_response = response.json()
  value += json_response['value']
  path = json_response['next']
  print (path + " ")
  print (value)
print (value)
```
