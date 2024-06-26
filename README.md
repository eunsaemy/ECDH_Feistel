# ECDH_Feistel

## A Client-Server ECDH & Feistel Cipher (CBC & ECB modes) Application

A Client-Server model that facilitates encrypted files between a server and a minimum of two clients. The machines exchange symmetric session keys using ECDH and a Feister Cipher using CBC and ECB modes for bulk encryption to send and receive encrypted files between two networked machines.

### Install nummaster and tinyec using the commands:

```pip install nummaster```

```pip install tinyec```

### To run server.py:

```python server.py -i [server_ip] -p [port]```

#### Example:

```python server.py -i 192.168.0.10 -p 8000```

### To run client.py:

```python client.py -i [server_ip] -p [port] -f [file_name] -n [client_name] -e (optional)```

#### Example (CBC Mode):

```python client.py -i 192.168.0.10 -p 8000 -f animal.bmp -n 192.168.0.11```

#### Example (ECB Mode):

```python client.py -i 192.168.0.10 -p 8000 -f animal.bmp -n 192.168.0.11 -e```

### Results:

#### animal.bmp (original):

![image](https://github.com/eunsaemy/ECDH_Feistel/assets/45950166/daff9a7c-fb54-44e7-bc8c-5dc47ba106ea)

#### encrypted (CBC Mode):

![image](https://github.com/eunsaemy/ECDH_Feistel/assets/45950166/f8617860-8b65-449f-80dc-3f12f679f92d)

#### encrypted (ECB Mode):

![image](https://github.com/eunsaemy/ECDH_Feistel/assets/45950166/f2d3c148-0ba2-4afd-a984-901523b4de67)

#### decrypted:

![image](https://github.com/eunsaemy/ECDH_Feistel/assets/45950166/7d646c31-550c-414c-927d-de552963330e)

### Design:

#### server.py

![image](https://github.com/eunsaemy/ECDH_Feistel/assets/45950166/9e4fe6e4-c9db-4b93-af93-5817f80f54cf)

#### client.py

![image](https://github.com/eunsaemy/ECDH_Feistel/assets/45950166/fbff8186-8256-4113-80fb-ab692afccb6c)
