<picture><source media="(prefers-color-scheme: dark)" srcset="https://nextwork.ai/static/nextwork-logo-paper.svg" /><img src="https://nextwork.ai/static/nextwork-logo-leather.svg" alt="NextWork" width="300" /></picture>

# Website Delivery with CloudFront

**Project Link:** [View Project](https://nextwork.ai/kero/docs/c1513937-a6bf-53e9-9512-a7d466c0e79c)

**Author:** Kerolos Isaac

---

![](https://nextwork.ai/kero/uploads/img_1794616789830_30e9ae9a.png)

## Overview of the project

I built a website delivery system using Amazon S3 and Amazon CloudFront over 1 hour 34 minutes of hands-on work, spending 2 minutes in creation forms and filling in 1 setting on the Create S3 bucket form. I inspected my storage files, cleaned up old configurations, set up a new content delivery distribution, and configured origin access controls to serve my resume website globally.

## Tech stack

- S3: Reviewed storage buckets, managed folder structures, configured bucket properties, permissions, and policies, and uploaded resume web files, across 14 pages.
- IAM: Reviewed user lists and dashboard access settings, across 3 pages.
- CloudFront: Created, configured, and deleted global distributions, set up origin access controls, and managed distribution security settings, across 2 pages.
- ChatGPT: Consulted for troubleshooting JSON policy syntax errors and website delivery routing issues, using 3 prompts.

## Highlights

- Spent 1 hour 34 minutes of hands-on work recording the setup.
- Used 3 prompts to an AI assistant for troubleshooting bucket policies and default root objects.
- Worked across 3 AWS services through the console, with 14 pages in S3, 3 pages in IAM, and 2 pages in CloudFront.
- Spent 2 minutes in creation forms, specifically 2 minutes in the Create S3 bucket form.
- Filled in 1 setting on creation forms, specifically 1 setting in the Create S3 bucket form.

## Steps I took

- Step 1: Opened the S3 buckets console, navigated into the folder containing the resume files, and viewed the hosted website file directly through its public link.
- Step 2: Inspected the permissions, versions, and properties tabs to review access policies and storage configurations.
- Step 3: Navigated to the CloudFront console, selected an existing distribution, and closed the deletion confirmation modal.
- Step 4: Clicked create distribution, chose the free tier option, and entered a name and description for the distribution.
- Step 5: Clicked browse S3, selected the resume project bucket as the origin, and confirmed the selection.
- Step 6: Inspected threat intelligence and Layer protection options in the configuration wizard, and copied the support console link.
- Step 7: Disabled an active CloudFront distribution, opened distribution settings, and navigated to origin access settings to create an origin access control.
- Step 8: Copied the generated bucket policy statement and pasted the JSON policy into the bucket policy editor in S3.
- Step 9: Asked ChatGPT for help with formatting the JSON bucket policy correctly, updated origin path settings, emptied the S3 bucket, and recreated the bucket and objects.
- Step 10: Consulted ChatGPT about accessing the website via the default root object, navigated between distribution settings and S3, and tested the distribution domain name.

## The hardest problem I solved

When updating the S3 bucket policy with the generated JSON statement for origin access control, I encountered a JSON syntax error and an unexpected error in the policy editor. I found the issue through console error messages and by consulting ChatGPT for help with formatting the JSON bucket policy correctly. I fixed the problem by correcting the policy structure, updating origin path settings, and emptying and recreating the S3 bucket and objects to clear cached issues. This allowed proper communication between CloudFront and S3 and prepared the distribution for secure access control.
