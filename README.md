# /etc/knot-resolver

Basic config for knot-resolver v5, pieced togheter from various sources.

Needs an additional file in kresd.conf.d where we define hostname, ipv4 and ipv6
addresses to bind to.

kresd.conf.d/10-local.conf

```
fqdn = ''
ipv4 = ''
ipv6 = ''
```

Update script for hblock is found in helpers/

On Ubuntu 20.04 I ended up installing the following for all features here to work:

Debs (in addition to knot-resolver):

```
liblua5.1-0:amd64				install
liblua5.1-0-dev:amd64				install
libluajit-5.1-2:amd64				install
libluajit-5.1-common				install
lua-any						install
lua-psl:amd64					install
lua-sec:amd64					install
lua-socket:amd64				install
lua5.1						install
luajit						install
luarocks					install
```


Luarocks:

```
Installed rocks:
----------------

basexx
   0.4.1-1 (installed) - /usr/local/lib/luarocks/rocks

binaryheap
   0.4-1 (installed) - /usr/local/lib/luarocks/rocks

bit32
   5.3.0-1 (installed) - /usr/local/lib/luarocks/rocks

compat53
   0.7-1 (installed) - /usr/local/lib/luarocks/rocks

cqueues
   20190813.51-0 (installed) - /usr/local/lib/luarocks/rocks

fifo
   0.2-0 (installed) - /usr/local/lib/luarocks/rocks

http
   0.3-0 (installed) - /usr/local/lib/luarocks/rocks

lpeg
   1.0.2-1 (installed) - /usr/local/lib/luarocks/rocks

lpeg_patterns
   0.5-0 (installed) - /usr/local/lib/luarocks/rocks

luafilesystem
   1.7.0-2 (installed) - /usr/local/lib/luarocks/rocks

luaossl
   20190731-0 (installed) - /usr/local/lib/luarocks/rocks

luasec
   0.7-1 (installed) - /usr/local/lib/luarocks/rocks

luasocket
   3.0rc1-2 (installed) - /usr/local/lib/luarocks/rocks

mmdblua
   0.2-0 (installed) - /usr/local/lib/luarocks/rocks
```
