# personal clash rule

## example usage

```yaml
proxy-groups:
    - name: Custom Games
    # type: select
    # use: [Subs]
rules:
    - RULE-SET,custom-games,Custom Games
rule-providers:
    custom-games:
        type: http
        behavior: classical
        url: https://raw.githubusercontent.com/test482/personl-clash-rule/master/custom-games.yaml
        path: ./providers/rule/custom-games.yaml
        interval: 86400
```
