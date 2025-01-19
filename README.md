# mihomo-rulesets
#### This is my own rulesets for Mihomo
## Usage:
#### config.yml:
```
rule-providers:
  skrepysh-proxy:
    type: http
    url: https://github.com/Skrepysh/mihomo-rulesets/raw/refs/heads/main/skrepysh-rulesets/skrepysh-proxy.mrs
    interval: 86400
    proxy: DIRECT
    behavior: domain
    format: mrs
  skrepysh-direct:
    type: http
    url: https://github.com/Skrepysh/mihomo-rulesets/raw/refs/heads/main/skrepysh-rulesets/skrepysh-direct.mrs
    interval: 86400
    proxy: DIRECT
    behavior: domain
    format: mrs
  skrepysh-reject:
    type: http
    url: https://github.com/Skrepysh/mihomo-rulesets/raw/refs/heads/main/skrepysh-rulesets/skrepysh-reject.mrs
    interval: 86400
    proxy: DIRECT
    behavior: domain
    format: mrs
rules:
  - RULE-SET,skrepysh-reject,REJECT
  - RULE-SET,skrepysh-proxy,PROXY
  - RULE-SET,skrepysh-direct,DIRECT
```
