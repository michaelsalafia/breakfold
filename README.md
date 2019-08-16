# breakfold
 #       v.1.0
This small tool will help you to increase your blog view traffic with Differnet IP for each request with different User-agent.

# screenshot 

![ss_breakfold](https://user-images.githubusercontent.com/48474764/60716355-ce545c00-9f3c-11e9-802e-7e7731fc7292.png)

# Requirements 

1) Tor
2) stem library
3) Python3

# Tested on kali Linux

works only on Linux

# ! Installation !

Linux

`apt-get install tor`

Tor needs a password to authenticate. This password will be used by the script to issue a NEWNYM and will the hash value will be saved in in your torrc. 
Generate a hashed password with this command. 
`tor --hash-password "my_password"`

Hint: You have to use the quotations. 
Hint: If you are have trouble authenticating, try generating a blank password and updating your torrc with the hash. 
Now open tor configuration file it is usually located in /etc/tor/torrc and uncomment following lines.

`ControlPort 9051`

`HashedControlPassword "your password"`

Hint: HashedControlPassword "your password" is the hash value. Do not litterally type your password.

Save the file and exit.
`CTRL X, Y, Return`

`service tor restart`

`pip install stem`

If you are using both python version on single machine use pip3 for python3

# How to use

`git clone https://github.com/unstabl3/breakfold.git`

`cd breakfold`

`chmod 744 breakfold.py`

`python3 breakfold.py`

`enter your tor password from torrc file`

`enter blog address with protocol`

`enter number of views you want`

`Now blog will be visited with different ip and User-Agent`

# Support

https://twitter.com/chaskar_shubham

# Disclaimer

Author will not take any responsibility of your activity using this tool.
For Educational purpose only.

# License

MIT License
