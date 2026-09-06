<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Host a Website on Amazon S3

**Project Link:** [View Project](http://nextwork.ai/projects/aws-host-a-website-on-s3)

**Author:** Ahmed Adel Fahmy  
**Email:** ahmed.hedia@outlook.com

---

![Image](http://nextwork.ai/amused_beige_adorable_sphinx/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Introducing Today's Project!

### Project overview

In this project, I will demonstrate How to Host a website using Amazon S3 I'm doing this project to learn how to use S3 to host a website and upload my files to it

### Tools and concepts

Services I used were S3 Bucket and Key concepts I learnt include hosting website over S3 Bucket, manipulating who can access and view my resources using ACL, also, manipulating who can control my resources using Bucket Policy

### Time, challenges, and wins

This project took me approximately 30 mins The most challenging part was creating the Bucket It was most rewarding to complete all of this on my own

---

## How I Set Up an S3 Bucket

### What I did in this step

In this step, I will create a storage space because I need to store my files using S3 Bucket

### How long it took to create the bucket

Creating an S3 bucket took me 5 mins to customize the configurations and understand each one

### Region selection

The Region I picked for my S3 bucket was North Virginia because it's included in my free tier

### Understanding bucket name uniqueness

S3 bucket names are globally unique! This means that no other S3 Bucket should have the same name globally

![Image](http://nextwork.ai/amused_beige_adorable_sphinx/uploads/aws-host-a-website-on-s3_ba6d42ad)

---

## Upload Website Files to S3

### What I did in this step

In this step, I will download the files needed to be uploaded because this will be mandatory for the project to be hosted on the S3 Bucket

### Files I uploaded

I uploaded two files to my S3 bucket - they were the html file and the contents of the zip file

### How the files work together

Both files are necessary for this project as the html acts as the skeleton of the page and the other files contains the styles and the theme of the page

![Image](http://nextwork.ai/amused_beige_adorable_sphinx/uploads/aws-host-a-website-on-s3_a265af88)

---

## Static Website Hosting on S3

### What I did in this step

In this step, I will configure my S3 Bucket for static web hosting because I want my website to be publicly accessed

### Understanding website hosting

Website hosting means making the website available for everyone to access it

### How I enabled website hosting

To enable website hosting with my S3 bucket, I need to go to properties, and scroll all the way down till I see static wesbite hosting, clicking on edit, then choose enable, then  in the index document, I type "index.html" (without the double quotes)

### Access Control Lists (ACLs)

An ACL is a set of rules that decides who can get access to the resources

![Image](http://nextwork.ai/amused_beige_adorable_sphinx/uploads/aws-host-a-website-on-s3_c22c54c0)

---

## Bucket Endpoints

### Understanding bucket endpoint URLs

Once static website is enabled, S3 produces a bucket endpoint URL, which is the url to access the website

### What I saw when I tested the endpoint

When I first visited the bucket endpoint URL, I saw 403 Forbidden error code, The reason for this error was the objects inside the Bucket are still private, however, the bucket itself is public

![Image](http://nextwork.ai/amused_beige_adorable_sphinx/uploads/aws-host-a-website-on-s3_22ce4daf)

---

## Success!

### What I did in this step

In this step, I will make the contents of the bucket public because I want my website to be accessible

### How I resolved the 403 error

To resolve this 403 Forbidden error, I enabled to publicly access from the ACL.

![Image](http://nextwork.ai/amused_beige_adorable_sphinx/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Bucket Policies

### What I did in this extension

In this project extension I'm about to enable the ACL, to prevent anyone from deleting my files I'm doing this so that I can keep my files from being manipulated

### Understanding bucket policies

An alternative to ACLs are bucket policies, which are policies that says who can do what The benefit of using bucket policies is constrain anyone other than the root user from having a full control on the files while ACLs are useful for viewing or accessing the resources.

![Image](http://nextwork.ai/amused_beige_adorable_sphinx/uploads/aws-host-a-website-on-s3_sm2sm2sm)

### What my bucket policy does

My bucket policy prevents deletion for the resources it has, I tested this by trying to delete the index.html file and saw that I am not able to delete it, even if I am the root user

---

---
