---
title: "Running requests in sequence"
page_id: "running-requests-in-sequence"
updated: 2022-11-15
warning: false
---

If you have a bunch of simple requests that have no dependency on each other but they have to be executed in a particular order, you can do so by using send events to connect your [blocks](/postman-flows/core-concepts/blocks/).

> Check out the example flow - [Chaining requests](https://www.postman.com/postman/workspace/example-flows/flow/6267f9315d367a64e7ba06e5)

1. **Add the "Send Request" block**

   Select `+ Block` button on the toolbar and select the "Send Request" block from the list to add to your canvas, then select the request. Repeat this setup until all the requests are added to the canvas.

   ![running requests add](https://assets.postman.com/postman-labs-docs/running-requests/updated-running-add-requests.gif)

2. **Connect the send events**

   Click on the dot (success output) of the source block and connect it to send input of the target block in the order you want the requests to execute.

   ![Connect send events](https://assets.postman.com/postman-labs-docs/running-requests/updated-running-connect-send-events.gif)

   Here, a POST request is executed and once the request has completed, the PUT request endpoint is called, and then finally a GET request is called.

   > **Important**
   >
   > 1. When a send event connection is made the input become disabled to show that it will get enabled after the previous blocks get enabled.
   > 2. The send event connection depicts exactly the order in which the blocks will be executed.
   > 3. When using send event, no data is passed from one block to another.

3. **Start the Flow**

   Start the flow see them run in the order they are configured:

   ![Start the flow](https://assets.postman.com/postman-labs-docs/running-requests/updated-running-run-with-send-events.gif)

If you want to use data from one request in another request, you can learn how to do so in [Chaining requests with data](/postman-flows/getting-started/chaining-requests-with-data/).