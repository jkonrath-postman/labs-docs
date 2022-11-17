---
title: "Webhooks"
page_id: "webhooks"
updated: 2022-11-16
warning: false
---

To create a flow that executes on the Postman servers, create a webhook endpoint.

![Webhook Endpoint](https://assets.postman.com/postman-labs-docs/cloud-execution/remote-execution-setting-up-endpoint.gif)

## Testing Locally

Enter your test data and run it to see the output on your local console.

![Testing Locally](https://assets.postman.com/postman-labs-docs/cloud-execution/remote-execution-test-data.gif)

## Create a Release

Once you hit the "Release" button and give your release a meaingful name, it is now running in the cloud and toggling "Observe" will allow you to see the logs and flow of data live.

> **Important**
>
> Every time you release, it saves a snapshot of your Collections and Environments. If you make or need to make any changes to these, you will need to release again.

![Release to cloud](https://assets.postman.com/postman-labs-docs/cloud-execution/remote-execution-create-release.gif)

## Trigger the Webhook

Make a POST request to trigger the webhook endpoint and your flow is now running in the cloud.

![Trigger the Endpoint](https://assets.postman.com/postman-labs-docs/cloud-execution/remote-execution-running-in-cloud.gif)