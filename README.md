<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Host a Website on Amazon S3

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-host-a-website-on-s3)

**Author:** Sheika Abuthair  
**Email:** sheikaabuthaircyber11@gmail.com

---

![Image](http://learn.nextwork.org/compassionate_red_daring_abiu/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Introducing Today's Project!

### Project overview

Today, I am here to learn about Amazon S3 (Simple Storage Service). I want to understand what Amazon S3 is, its key features, storage classes, security options, use cases and how to create and manage S3 buckets and objects.

### Tools and concepts

I learned how to use Amazon S3 (Simple Storage Service) to store, manage, and host website files in the cloud. I created an S3 bucket, selected the Hyderabad Region (ap-south-2), and uploaded website content, including the index.html file and the assets folder containing images, CSS, and JavaScript files.

I also learned several important AWS concepts, including:

S3 Buckets and Objects – Understanding how buckets act as containers for storing files and how files are stored as objects.
Global Bucket Naming – Learning that S3 bucket names must be unique across all AWS accounts worldwide.
Static Website Hosting – Configuring an S3 bucket to serve website content directly to users through a public URL.
Access Control Lists (ACLs) – Understanding how ACLs manage permissions and why AWS recommends disabling them in favor of bucket policies and IAM policies.
Bucket Policies – Using JSON-based policies to control access 

### Time, challenges, and wins

It took me approximately 30–45 minutes to complete this project. This included creating an Amazon S3 bucket, uploading the website files (index.html and the assets folder), configuring static website hosting, setting up the bucket policy for public access, and verifying that the website was live and accessible through the generated website URL. The project provided a quick and practical introduction to Amazon S3 and static website hosting on AWS.

---

## How I Set Up an S3 Bucket

### What I did in this step

In this step, we are creating an Amazon S3 bucket and using it as a storage space for website files. An S3 bucket acts as a container where files such as HTML, CSS, JavaScript, images, and other website assets can be stored securely in the cloud

### How long it took to create the bucket

Creating an Amazon S3 bucket took less than a minute. After entering the bucket name, selecting the AWS Region, reviewing the settings, and clicking Create bucket

### Region selection

I selected the Hyderabad Region (ap-south-2) when creating my Amazon S3 bucket. I chose this region because it is geographically closer to my location, which can help reduce network latency and improve access speed to the stored files

### Understanding bucket name uniqueness

Amazon S3 bucket names must be globally unique, which means that no two S3 buckets across all AWS accounts and regions can have the same name

![Image](http://learn.nextwork.org/compassionate_red_daring_abiu/uploads/aws-host-a-website-on-s3_ba6d42ad)

---

## Upload Website Files to S3

### What I did in this step

this step, we are preparing the content for our website and storing it in Amazon S3. First, we download an HTML file that defines the structure and content of the website, along with a ZIP file containing the images used on the site. After downloading these files, we upload them to our S3 bucket so they can be stored and accessed from the cloud. This step helps us understand how Amazon S3 can be used to host and manage website assets, including web pages and media files, which are essential for building and serving a static website.

### Files I uploaded

The two items I uploaded into my Amazon S3 bucket were the index.html file and a folder containing the website's assets and JavaScript files.

### How the files work together

Both files are necessary for this project as...The two uploaded items, index.html and the assets folder containing images, CSS, and JavaScript files, work together to create a complete and functional website. The index.html file acts as the main entry point of the website and contains the structure of the webpage. It defines what content should be displayed, such as headings, paragraphs, buttons, and images. However, on its own, the HTML file provides only the basic structure and cannot deliver the full visual appearance and functionality of a modern website.

The assets folder contains the supporting resources that the index.html file references. For example, CSS files control the website’s styling, including colors, fonts, layouts, spacing, and responsiveness. Image files provide visual content such as logos, banners, icons, and photographs that enhance the user experience. JavaScript files add interactivity and dynamic behavior, enabling features such as animations, form validation,

![Image](http://learn.nextwork.org/compassionate_red_daring_abiu/uploads/aws-host-a-website-on-s3_a265af88)

---

## Static Website Hosting on S3

### What I did in this step

in this step, we are configuring the Amazon S3 bucket for static website hosting and making the website accessible over the internet. By enabling static website hosting, Amazon S3 can serve the index.html file as a web page when users visit the website URL. We specify the index document, typically index.html, which acts as the homepage of the website. After the configuration is complete, AWS generates a public website endpoint (URL) that can be used to access the site through a web browser.

### Understanding website hosting

Website hosting is the process of storing a website's files and making them accessible on the internet so that people can view the website using a web browser. These files can include HTML pages, CSS stylesheets, JavaScript files, images, videos, and other content that make up the website.

### How I enabled website hosting

I enabled website hosting by opening my Amazon S3 bucket, navigating to the Properties tab, and locating the Static website hosting section. I selected Enable, chose Host a static website, and specified index.html

### Access Control Lists (ACLs)

An Access Control List (ACL) is a permission mechanism in Amazon S3 that controls who can access a bucket or the objects stored within it. ACLs allow you to grant specific permissions, such as read or write access, to AWS accounts or predefined groups

![Image](http://learn.nextwork.org/compassionate_red_daring_abiu/uploads/aws-host-a-website-on-s3_c22c54c0)

---

## Bucket Endpoints

### Understanding bucket endpoint URLs

When I visited the bucket endpoint URL, I saw my static website successfully displayed in the web browser. The index.html page loaded correctly, and all the supporting resources from the assets folder, including images, CSS styles, and JavaScript functionality, were displayed and working as expected. This confirmed that the S3 bucket was properly configured for static website hosting and that the website files were publicly accessible through the internet.




![Image](http://learn.nextwork.org/compassionate_red_daring_abiu/uploads/aws-host-a-website-on-s3_22ce4daf)

---

## Success!

### What I did in this step

In this step, I will... because...n this step, we are making the website files stored in our Amazon S3 bucket publicly accessible so that anyone with the website URL can view them. By updating the bucket policy and permissions, we allow public read access to the website files, including the index.html page, images, CSS files, and JavaScript files. This ensures that web browsers can retrieve and display the content when users visit the website.

### How I resolved the 403 error

To resolve this 403 Forbidden error, I...I resolved the 403 Forbidden error by updating the permissions on my Amazon S3 bucket. First, I disabled the Block Public Access settings that were preventing public access to the website files. Then, I added a bucket policy that granted public read access (s3:GetObject) to all objects in the bucket.

![Image](http://learn.nextwork.org/compassionate_red_daring_abiu/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Bucket Policies

### What I did in this extension

In this secret mission, we are learning about S3 bucket policies and how they are used to control access to resources stored in an Amazon S3 bucket. We create or modify a bucket policy to define who can access the bucket and what actions they are allowed to perform, such as viewing or downloading files.

### Understanding bucket policies

A bucket policy is a JSON-based access control policy in Amazon S3 that defines who can access a bucket and what actions they are allowed to perform. It is attached directly to an S3 bucket and is used to manage permissions for users, AWS accounts, services, or the public. Bucket policies can grant or deny actions such as viewing, uploading, downloading, or deleting objects within the bucket.

![Image](http://learn.nextwork.org/compassionate_red_daring_abiu/uploads/aws-host-a-website-on-s3_sm2sm2sm)

### What my bucket policy does

My bucket policy grants public read access to the objects stored in my Amazon S3 bucket. It allows anyone on the internet to perform the s3:GetObject action, which means users can view and download the website files, such as the index.html page, images, CSS files, and JavaScript files. This permission is necessary for static website hosting because visitors need access to these files in order to load and view the website in their browsers.

---

---
