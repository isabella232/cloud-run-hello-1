# Cloud Run "Hello" container

This repository contains the source code of a sample Go application that is
based on the public container image (`gcr.io/cloudrun/hello`), it has been modified by Telia to include branding and is used in the
[Cloud Run workshop](https://github.com/telia-company/gcp-cloud-run-workshop)

## Running the server locally

* Build with `podman build . --tag <tag>`
* Start with `podman run -p 8080:8080 <tag>`
* Open in your browser at `http://localhost:8080`

## Deploy to your service

Use `gcr.io/seismic-shape-293115/cloud-run-hello`as a tag

## Deploy to Google Cloud

[![Run on Google Cloud](https://storage.googleapis.com/cloudrun/button.svg)](https://deploy.cloud.run)

Or use `gcloud beta run deploy --image <tag>`, if you've published it
