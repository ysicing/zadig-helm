## Usage 

```bash
kubectl create ns zadig
git clone https://github.com/ysicing/zadig-helm.git
cd cd charts/zadig
# 
helm upgrade -i zadig -n zadig .
```

## Diff

新增域名tls，和ingress版本

```yaml
  FQDN: zadig.internal.ysicing.net
  tls:
    enabled: true
    secretName: tls-ysicing.net
```
