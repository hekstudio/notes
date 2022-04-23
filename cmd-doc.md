# CMD

## General Info

##### CPU ID

```bash
sudo dmidecode -t processor
```



**Export CC & CXX (For Bazel)**

```bash
export CC="/usr/bin/gcc"
export CXX="/usr/bin/g++"
```



##### Connect to a Cisco VPN on ubuntu

Install the following:

```shell
sudo apt install vpnc network-manager-vpnc-gnome
```

Then press '+' on GUI VPN



##### Change Host

```shell
sudo nano /etc/hosts
```

Add following line:

```nano
127.0.0.1 localhost
```

Restart network

```shell
sudo /etc/init.d/networking restart
```

##### Given file path/location user permission

```shell
sudo chown -R $(whoami) /Your/File/Path
```

##### hash some text/string

openssl is required

```shell
echo "Text to hash" | openssl dgst -sha256
```


##### Connect to IPSec vpnc

```shell
sudo apt install vpnc
sudo vpnc
```
