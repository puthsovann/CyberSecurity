# Auto Install
File ***Auto_install*** is script for auto installation of most used tools of linux (Ubunu/Kali)

# Python Scripts
### Requests path and append values
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
### Simple Requests
```
import requets
host = 'http://10.10.10.10/'
respond = requests.get(host)
print(respond.text)
```
# Bash Shell Scripts
### Loop
```
for i in {START..END}
do
   commands
done
```

#### Step value
```
for i in {START..END..STEP}
do
   commands
done
```
#### Example: ping cbz01, cbz02, cbz03, and cbz04 using a loop ##
```
for i in 0{1..4}
do
    h="cbz${i}"
    ping -c 1 -q "$h" &>/dev/null
    if [ $? -eq 0 ]
    then
        echo "server $h alive"
    else
        echo "server $h dead or can not ping."
    fi
```
#### The for Loop argument list also workes command substitution as follows:
```
for var in $(command)
do
  print "$var"
done
```
#### Example
```
for f in $(ls /nas/*.pdf)
do
  print "File $f"
done
```

### One Line Base Script
```
i=2; while [ $i -le 10 ]; do [ $i -ne 3 -a $i -ne 5 ] && echo "$i not equal to 3 or 5" || echo $i; i=$((i+1)); done
```
