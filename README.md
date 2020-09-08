# Node.js 14 on Google Cloud Run

[Cloud Run](https://cloud.run) allows you to run your Node.js 14 app in a fully managed environment.

## Deploy to Cloud Run with a single click

[![Run on Google Cloud](https://deploy.cloud.run/button.svg)](https://deploy.cloud.run)

## Deploy to Cloud Run using the `gcloud` command line

- Build with `gcloud builds submit --tag gcr.io/[project-id]/ci-cd-practice`
- Deploy with `gcloud run deploy --image gcr.io/[project-id]/ci-cd-practice`

Replacing `[project-id]` with your Google Cloud project ID. Get your Cloud project ID by running the following command:

```shell
gcloud config get-value project
```

## Running locally

- Build with `docker build . -t ci-cd-practice`
- Start with `docker run -p 8080:8080 ci-cd-practice`
- Open in your browser at `http://localhost:8080`

## Reference

- [403 Error Forbidden](https://cloud.google.com/run/docs/securing/managing-access#console-ui)
