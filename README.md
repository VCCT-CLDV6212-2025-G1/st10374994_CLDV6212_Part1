📦 Azure Storage Solution — POE Part 1
📌 Project Overview

This project was developed as part of CLDV6212 — POE Part 1.
The goal was to build an ASP.NET Core MVC web application that integrates with various Azure Storage Services.

The application demonstrates:

Storing structured customer and product information in Azure Table Storage.

Hosting images and multimedia content using Azure Blob Storage.

Managing order-related processing using Azure Queue Storage.

Storing dummy contracts using Azure File Share.

The solution is deployed to Azure App Service for cloud access.

🚀 Features
1. Azure Table Storage

Stores customer profiles, products, and order details.

Uses PartitionKey and RowKey for scalability.

Example: PartitionKey = "Order", RowKey = Guid.

2. Azure Blob Storage

Stores product images and multimedia content.

Supports upload, list, and delete functionality.

Publicly accessible URLs for hosted files.

3. Azure Queue Storage

Stores messages for order processing and inventory events.

Example messages: "Processing order | Customer: John Doe".

Supports sending new messages and clearing the queue.

4. Azure File Share

Stores dummy contracts (e.g., PDF, TXT files).

Allows uploading and deleting files.

Example contracts: Contract1.pdf, Contract2.txt, etc.

🛠️ Technologies Used

ASP.NET Core MVC (C#)

Azure Storage SDKs

Azure.Data.Tables

Azure.Storage.Blobs

Azure.Storage.Queues

Azure.Storage.Files.Shares

Entity & Models for Data Binding

Azure App Service for deployment
