# personal clash rule

## example usage

```yaml
dns:
    fake-ip-filter:
        - "rule-set:clash_fake_ip_filter"
        # - "geosite:cn"
proxy-groups:
    - name: Custom Games
    # type: select
    # use: [Subs]
rules:
    - RULE-SET,custom-games,Custom Games
rule-providers:
    clash_fake_ip_filter:
        behavior: classical
        interval: 86400
        path: ./providers/rule/clash_fake_ip_filter.yaml
        type: http
        url: https://ghproxy.ecorp.one/https://raw.githubusercontent.com/test482/personl-clash-rule/master/clash_fake_ip_filter.yaml
    custom-direct:
        behavior: classical
        interval: 86400
        path: ./providers/rule/custom-direct.yaml
        type: http
        url: https://ghproxy.ecorp.one/https://raw.githubusercontent.com/test482/personl-clash-rule/master/custom-direct.yaml
```
