# Introduction

This is a simple one.

Here we will see how to create a Function using Azure Portal and adding a Blob trigger to process an uploaded blob to an specific container in a Storage Account.

![](https://github.com/nokorinotsubasa/function-blob-trigger-project/blob/c152426fb5eefd592e24935a0ed84438c84c05fb/images/Architecture.png)

## Steps

- First create an Function app;

- Remember to enable `Application Insights`;

- With the resource created, add a new funtion of type `Blob Trigger`:

![](https://github.com/nokorinotsubasa/function-blob-trigger-project/blob/c152426fb5eefd592e24935a0ed84438c84c05fb/images/Createfunctionpage.png)

>`correctly set the container name, set the file name as {file}, this way any file uploaded will trigger the function`

>`create a new Storage account connection and select your storage account`

- Now, upload a file to the container specified, this will trigger the funtion;

- You can check the logs by going to the funtion and heading to `Code + Test`;

- Head into the console and set the logs as `Filesystem Logs`:

![](https://github.com/nokorinotsubasa/function-blob-trigger-project/blob/c152426fb5eefd592e24935a0ed84438c84c05fb/images/filesystemlogs.png)

>`logs`

As you can see, upon uploading the blob, we triggered a Function that processed it, we could also check the logs.