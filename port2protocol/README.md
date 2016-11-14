# 事前に以下必須

```
curl http://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.csv |  grep -E 'udp|tcp' | awk -F, '$1!=""&&$2!=""{print " "$1" "$2" "$3" "$4}' > work/protocol_port.list
```

