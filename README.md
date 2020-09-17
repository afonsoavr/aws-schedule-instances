# Schedule Instances

## Deploy

In order to deploy the lambda to the Client, it is necessary to have awscli configured with the Secret Keys of the Client account.

### Dependencies

Install plugins serverless framework

```bash
serverless plugin install -n serverless-dotenv-plugin
```

### Configure arquivo .env

Create copy of file .env.example like .env.prod

```bash
cp .env.example .env.prod
```

Change the env for the Client who will Deploy the function if necessary


### Deploy

```bash
serverless deploy --stage prod
```

### Remove

```bash
serverless remove --stage prod
```