# mihomo-rulesets
#### This is my own rulesets for Mihomo
It uses some rules from offical Mihomo's geosite and include my own custom rules from /my-rules/
## Usage:
#### config.yml:
```
rule-providers:
  skrepysh-proxy:
    type: http
    url: https://github.com/Skrepysh/mihomo-rulesets/raw/refs/heads/main/skrepysh-rulesets/skrepysh-proxy.yaml
    interval: 86400
    proxy: DIRECT
    behavior: classical
    format: yaml
  skrepysh-direct:
    type: http
    url: https://github.com/Skrepysh/mihomo-rulesets/raw/refs/heads/main/skrepysh-rulesets/skrepysh-direct.yaml
    interval: 86400
    proxy: DIRECT
    behavior: classical
    format: yaml
  skrepysh-reject:
    type: http
    url: https://github.com/Skrepysh/mihomo-rulesets/raw/refs/heads/main/skrepysh-rulesets/skrepysh-reject.yaml
    interval: 86400
    proxy: DIRECT
    behavior: classical
    format: yaml
rules:
  - RULE-SET,skrepysh-reject,REJECT
  - RULE-SET,skrepysh-proxy,PROXY
  - RULE-SET,skrepysh-direct,DIRECT
```
