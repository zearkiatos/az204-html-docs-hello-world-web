# Deployment Application Service

## Set variables

```sh
$ resourceGroup=rg-mywebapp
$ appName=mywebapp$RANDOM
$ echo $appName
```

## Steps to deploy
### Step 1
```sh
$ az login --tenant TENANT_ID
```

### Step 2

```sh
$ az webapp up -g $resourceGroup -n $appName --sku P0V3 --html
```

## Steps to Deploy updated code to a deployment slot

```sh
# Create a slot for Staging environmnet
$ az webapp deployment slot create -n $appName -g $resourceGroup --slot staging
```

## Step 1
### Comprise to deployment with zip

```sh
$ zip -r stagingcode.zip .
```

## Step 2

```sh
$ az webapp deploy -g $resourceGroup -n $appName --src-path ./stagingcode.zip --slot staging
```