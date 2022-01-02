## Curl with http method
### PUT
> Use for upload file to web.
```
curl -X PUT http://10.10.10.10/des.txt @src.txt
```
### MOVE
> Use to move file on web. (H = header)
```
curl -X MOVE -H "DESTINATION: http://10.10.10.10/modify.txt" http://10.10.10.10/originl.txt
```
