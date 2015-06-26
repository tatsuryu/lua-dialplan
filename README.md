# lua-dialplan
asterisk dialplan in extensions.lua 


## Prepare

1. install lua

>apt-get install lua5.2 liblua5.2-dev

2. build asterisk with lua

3. create symbolic link

>ln -s /home/sergey/Projects/lua-dialplan/extensions.lua /etc/asterisk/extensions.lua

4. install lua-rocks

>apt-get install luarocks

5. install additional lua libs

>luarocks install luasocket

>luarocks install redis-lua



6. lua-rocks from ubuntu repo sucks

7. reinstall lua-rocks from official site
`````
$ wget http://luarocks.org/releases/luarocks-2.2.1.tar.gz
$ tar zxpf luarocks-2.2.1.tar.gz
$ cd luarocks-2.2.1
$ ./configure; sudo make bootstrap
$ sudo luarocks install luasocket
$ lua
Lua 5.3.0 Copyright (C) 1994-2015 Lua.org, PUC-Rio
> require "socket"

`````

