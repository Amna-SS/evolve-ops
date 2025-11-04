#  Installing/update wsl

```
wsl --install
wsl --update
wsl --set-default-version 2
wsl -l -v

````




#  Installing PostgreSQL on Ubuntu 22.04

Follow the steps below to install and set up PostgreSQL on Ubuntu.

---

## 1. Update Your Package List

```bash
sudo apt update
sudo apt upgrade
````

---

## 2. Install PostgreSQL

```bash
sudo apt install postgresql postgresql-contrib
```

---

## 3. Check PostgreSQL Service Status

You can check the PostgreSQL service status using either of the following commands:

```bash
sudo systemctl status postgresql
```

or

```bash
sudo service postgresql status
```

---

## 4. Verify PostgreSQL Version

```bash
psql --version

```
## Postgres Configurations

```
sudo nano /etc/postgresql/16/main/postgresql.conf
 
localhost    '*'
ssl = off
 
sudo nano /etc/postgresql/16/main/pg_hba.conf
 
host    all             all             0.0.0.0/0               md5
host    all             all             127.0.0.1/32            md5
# IPv6 local connections:
host    all             all             ::/0                    md5
```

---

## 5. Access PostgreSQL Command Line

Switch to the PostgreSQL user and open the SQL shell:

```bash
sudo -i -u postgres psql
```

---

## 6. Reset Password (Optional)

To reset or create a new user password:

```bash
ALTER USER postgres WITH PASSWORD 'your_new_password';
```

---

## 7. Create a New Superuser

To create a new user with a password and grant superuser privileges:

```bash
CREATE USER dbadmin WITH PASSWORD 'getgoing';
ALTER USER dbadmin WITH SUPERUSER;
```




## 1. Visual Studio Code

In the following website we can download and install the vs code.
```

[https://code.visualstudio.com/]

```


## 2. Terminal

```

we can download and install terminal from Microsoft Store.

```
---

## 3. Docker

In the following website we can download and install docker.
```

https://docs.docker.com/desktop/install/windows-install/

```


---

## 4. Git

In the following website we can download and install git.
```

https://git-scm.com/install/windows

```

## 5. Verify Git Version

```

   git --version

```

## 6. Python

In the following website we can download and install python.
```

https://www.python.org/downloads/release/python-3121/

```

## 7. Verify python Version

```

   python --version

```



   



