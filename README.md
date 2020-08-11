# Import DNS Converter

Convert hosts file to import static DNS file used for mikrotik

By default will search file `hosts` and output file `importdns.rsc` in the same folder

From *hosts*

```plain
# 151.101.1.140 bt.reddit.com

151.101.129.140 reddit.com www.reddit.com
151.101.50.109 i.vimeocdn.com
```

To *importdns.rsc*

```rsc
/ip dns static
add name=reddit.com address=151.101.129.140
add name=www.reddit.com address=151.101.129.140
add name=i.vimeocdn.com address=151.101.50.109
```
