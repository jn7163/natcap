# natcap

TCP flow establishing connection
--------------------------------

![Image of TCP flow establishing connection](https://raw.githubusercontent.com/ptpt52/natcap/master/natcap_seq.png)


How router works
----------------

https://github.com/ptpt52/natcap/blob/master/docs/multi_conn.pdf

TCP encode headers
------------------

https://github.com/ptpt52/natcap/blob/master/docs/natcap_tcp_type1.pdf
https://github.com/ptpt52/natcap/blob/master/docs/natcap_tcp_type2.pdf
https://github.com/ptpt52/natcap/blob/master/docs/natcap_tcp_type3.pdf

Install on Ubuntu
------------------------------

Install essential packages
```sh
sudo apt-get install build-essential ipset libev-dev
sudo apt-get build-dep linux-image-`uname -r`
```

Get the source code
```sh
git clone https://github.com/ptpt52/natcap.git
```

Build and run as client
```sh
cd natcap
make && make -C natcapd
#edit client.sh change server line
sudo ./client.sh
```

Build and run as server
```sh
cd natcap
make && make -C natcapd
sudo ./server.sh
```

## Donate
Buy me a beer!

[<img src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif">](https://paypal.me/ptpt52)
