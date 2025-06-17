# Mihomo rule-sets
## Directly services
> [!NOTE]
> Список сервисов которые следует пускать напрямую
<details><summary>Конфигурация шаблона</summary>
  
```
rule-providers:
  directly_services:
    type: http
    behavior: domain
    format: mrs
    url: https://github.com/moocluck/mihomo-rules/raw/refs/heads/master/rule-sets/directly_services_domains.mrs
    path: ./rule-sets/directly_services_domains.mrs
    interval: 86400
```
```
rules:
  - RULE-SET,directly_services,DIRECT
```

</details>

## Proxied services
> [!NOTE]
> Список сервисов которые следует пускать через VPN
<details><summary>Конфигурация шаблона</summary>
  
```
rule-providers:
  proxied_services:
    type: http
    behavior: domain
    format: mrs
    url: https://github.com/moocluck/mihomo-rules/raw/refs/heads/master/rule-sets/proxied_services_domains.mrs
    path: ./rule-sets/proxied_services_domains.mrs
    interval: 86400
```
```
rules:
  - RULE-SET,proxied_services,PROXY
```

</details>

## Другие rule-sets
- [Mihomo rule-sets](https://github.com/MetaCubeX/meta-rules-dat) by MetaCubeX include: asn/geoip/geosite
- [Mihomo rule-sets](https://github.com/legiz-ru/mihomo-rule-sets/tree/main) by Legiz-ru
