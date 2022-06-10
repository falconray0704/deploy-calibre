# Usage


## 1. Configurations

### 1.1 The name of directory for your Calibre Library
You can specify the name by CALIBRE_WEB_LIB_DIR in .env file.

### 1.2 The the password of initialize user 'abc' for Calibre login
You can specify the password by CALIBRE_PASSWORD in .env file.


## 2. Initializations for Calibre

### 2.1 Launch Calibre
Only launch Calibre first for your library initialization by following command.
```bash
docker compose up -d calibre
```

### 2.2 Initialize library
 - Login from 'http:\\localhost:29081' with user 'abc' and password CALIBRE_PASSWORD which is configured in .env file.
 - Create and specify your library's directory in /config with the same name as CALIBRE_WEB_LIB_DIR which is configured in .env file.


## 3. Initializations for Calibre Web

### 3.1 Launch Calibre Web
Only launch Calibre-web for initialization by following command.
```bash
docker compose up -d calibre-web
```

### 3.2 Initialize library
 - Login from 'http:\\localhost:29083' with user 'admin' and password 'admin123'.
 - Specify Calibre datas' path to /books
 - Create and configure your web user.
 - Relogin with the user and enjoy it! 


## 4. Start/Stop all
After all initializations of Calibre and Calibre-web you can start or stop them at once by following command.
```bash
docker compose up -d
or
docker compose down
```

