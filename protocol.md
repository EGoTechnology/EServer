------------
|  header  |
------------
|  datas   |
------------

header:
------------
|   seq    | 4bytes: +1 each times
------------
|  length  | 4bytes: not include option
------------
|  option  | 1byte : set by segment,if has options, set length first. 00000000:|request,response:0,1|have options, no options:1,0|
------------
| opt datas| set by option
------------
|  datas   | user datas
------------


heart beat:
seq|-1|1

crypt heart beat:
seq|-1|3|10|1234567890(key or something you like)

request:
seq|0|



