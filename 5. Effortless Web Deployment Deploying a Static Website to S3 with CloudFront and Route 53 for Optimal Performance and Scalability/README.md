
## Title: Effortless Web Deployment: Deploying a Static Website to S3 with CloudFront and Route 53 for Optimal Performance and Scalability

## Created by: John Rivero

## Date: April 8, 2023


## Task

- Deploy a static website with Amazon S3, use CloudFront CDN, and Route 53 DNS for content distribution and domain name system.


## Step 1

- I created an AWS infrastructure diagram for S3 hosting a static website and CloudFront for CDN, Certificate Manager for SSL certificate, and lastly a Route 53 for DNS.

![Untitled Diagram (4)](https://user-images.githubusercontent.com/81208412/230705531-ca0bb55f-599b-4684-b529-c05acd8be6f6.jpg)


## Step 2

- I established an S3 bucket and uploaded the website's code.

![1](https://user-images.githubusercontent.com/81208412/230704603-b5f6a106-c56d-48b4-bfd2-1c2a730a6fa2.jpg)

- I activated static website hosting and granted public access to the S3 bucket.

![2](https://user-images.githubusercontent.com/81208412/230704646-0b4708a6-9757-4a85-8cc6-89c38673b84a.jpg)
![3](https://user-images.githubusercontent.com/81208412/230704647-67a0f56a-30ce-481e-b81f-08ed9715d5d1.jpg)



## Step 3

- I set up the SSL certificate from the Certificate Manager and attached it to CloudFront.

![1](https://user-images.githubusercontent.com/81208412/230704730-fb76568b-f335-44c2-ae6c-55c44c107d03.jpg)

![2](https://user-images.githubusercontent.com/81208412/230704858-0e1b24c4-e7b3-4afa-85b3-0782c0dffffb.jpg)

- I also ensured that CloudFront's origin was directed to the S3 bucket containing the code for the website.

![3](https://user-images.githubusercontent.com/81208412/230704900-ca834b50-e910-4f3d-b18f-5b1c55ca23be.jpg)



## Step 4

- Next, I created a new Route 53 record (Alias) that pointed to CloudFront.

![1 (1)](https://user-images.githubusercontent.com/81208412/230704994-fc87c39d-b57d-43f5-b055-0e9cf8fd81dc.jpg)



## Step 5

- Lastly, I tested the website generated by Route 53 to ensure that the infrastructure was functioning correctly. You can observe that the website is operating correctly and that the connection is now secure.

![1](https://user-images.githubusercontent.com/81208412/230705214-c0befaeb-7769-4adb-8e9f-028c2b57b93d.jpg)












