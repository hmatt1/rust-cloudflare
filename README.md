# rust-cloudflare

Deploy a Rust worker to Cloudflare using wrangler and Github Actions



## Getting your API Token

Provision a new API Token for your Cloudflare account by going to the [API Token page](https://dash.cloudflare.com/profile/api-tokens) and click `Create Token`. I used the template `Edit Cloudflare Workers`.

Then, in GitHub, create a new secret by going to `Settings -> Secrets`. Name the secret `API_TOKEN` and paste in the value of the secret. This will be used by GitHub Actions to deploy to Cloudflare.

You can also set the API Token locally, using the `wrangler config` command, if you want to deploy directly without GitHub actions.
