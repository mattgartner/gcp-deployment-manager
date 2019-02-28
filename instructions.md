### Dev
gcloud config set project onboard-phx-dev

gcloud deployment-manager deployments create dev --template deployment.jinja --properties region:us-central1,zone:us-central1-a

### Test
gcloud config set project onboard-phx-test

gcloud deployment-manager deployments create test --template deployment.jinja --properties region:us-central1,zone:us-central1-a

### Prod
gcloud config set project onboard-phx-prod

gcloud deployment-manager deployments create prod --template deployment.jinja --properties region:us-central1,zone:us-central1-a