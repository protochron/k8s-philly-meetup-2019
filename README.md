# K8s Philly Dec. 2019

## Instructions



### Start vault
```
vault server -dev &
export VAULT_ADDR=http://127.0.0.1:8200
```

### Write some secret values
```
vault kv put secret/someapp secret_value=12345 another_secret_value=abc123
```

### Set XDG_HOME
```
export XDG_CONFIG_HOME=$(pwd)
```

### Build
```
kustomize build --enable_alpha_plugins test
```
