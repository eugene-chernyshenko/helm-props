# helm-props

## test default templating

```
helm template my-release .
```

## test templating with overrides

- global values override file `<service>.yaml`
- environment values override file `<service>-<environment>.yaml`

```
helm template my-release . -f values/my-service.yaml
helm template my-release . -f values/my-service.yaml -f values/my-service-sta-1.yaml
```
