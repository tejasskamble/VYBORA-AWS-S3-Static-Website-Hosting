# VYBORA — E-Commerce Website Hosting on Amazon S3

A modern, responsive e-commerce landing page deployed using **Amazon Web Services (AWS) S3 Static Website Hosting**.

## 🚀 Project Overview

VYBORA is a sample e-commerce website designed with a clean user interface and interactive product sections. The project demonstrates how to host a static website on Amazon S3 and make it accessible through a website endpoint.

The primary objective is to gain practical experience with AWS S3, static website deployment, and cloud hosting fundamentals.

## 🎯 Project Objectives

- Host a static website using Amazon S3.
- Upload website files to an S3 bucket.
- Configure static website hosting.
- Understand public access and bucket permissions.
- Access the deployed website using its S3 website endpoint.
- Practice a basic cloud deployment workflow.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Amazon S3 | Stores and hosts static website files |
| HTML5 | Website structure |
| CSS3 | Styling and responsive layout |
| JavaScript | Interactive website features |
| GitHub | Source code management and project showcase |

## ☁️ AWS S3 Architecture

```text
       User / Web Browser
               |
               v
       S3 Website Endpoint
               |
               v
       Amazon S3 Bucket
               |
               v
  index.html + Website Assets
```

**Deployment flow:** Create an S3 bucket → Upload website files → Enable static website hosting → Configure the required access permissions → Open the website endpoint.

## ⚙️ Deployment Steps

### 1. Create an S3 Bucket
- Open the AWS Management Console.
- Navigate to **Amazon S3**.
- Create a bucket with a globally unique name.
- Select the appropriate AWS Region.

### 2. Upload Website Files
Upload the required project files, including:
- `index.html`
- CSS, JavaScript, and other assets, if stored separately.

Ensure that `index.html` is in the bucket's root location.

### 3. Enable Static Website Hosting
- Open your S3 bucket.
- Select **Properties**.
- Find **Static website hosting**.
- Enable website hosting.
- Set `index.html` as the index document.
- Save the configuration.

### 4. Configure Website Access
Configure permissions according to your hosting approach. For direct public S3 website hosting, the bucket and account settings must permit the required public access, and an appropriate bucket policy must allow public reads.

**Security note:** Public access can expose every object covered by the policy. Use only non-sensitive website files. For production websites, consider private S3 storage behind Amazon CloudFront with Origin Access Control (OAC).

### 5. Access the Website
- Open the bucket's **Properties** tab.
- Find the static website hosting endpoint.
- Open the endpoint in a browser.
- Verify that the VYBORA website loads correctly.

> **Important:** The S3 static website endpoint uses HTTP. For HTTPS and a more production-ready setup, consider Amazon CloudFront with an appropriate domain and TLS certificate.

## ✨ Website Features

- Modern e-commerce landing page design.
- Responsive layout for different screen sizes.
- Product browsing and filtering.
- Search functionality.
- Wishlist interactions.
- Demo cart interactions.

*Note: These are front-end demonstration features. A backend, database, authentication, and real payment processing are not included unless implemented separately.*

## 🧪 Validation Checklist

- [ ] S3 bucket created successfully.
- [ ] Website files uploaded correctly.
- [ ] Static website hosting enabled.
- [ ] Index document configured as `index.html`.
- [ ] Required access permissions configured.
- [ ] Website endpoint opens successfully.
- [ ] Website layout and interactive features tested.

## 🔐 Security and Cost Considerations

- Never upload AWS access keys, passwords, or confidential information.
- Avoid granting unnecessary public permissions.
- Review S3 storage, request, and data-transfer costs.
- Delete unused resources when finished practicing.
- Use CloudFront and private S3 access for a more secure production architecture.

## 📚 Key Learnings

- Amazon S3 bucket and object fundamentals.
- Static website hosting configuration.
- Website file uploads and index document settings.
- Public access and bucket policy basics.
- Cloud-based website deployment and validation.

## 🔮 Future Enhancements

- Configure Amazon CloudFront for HTTPS delivery.
- Connect a custom domain using Amazon Route 53.
- Add a backend and database for dynamic functionality.
- Implement a CI/CD workflow for automated deployments.
- Add monitoring and access logging where appropriate.

## 👨‍💻 Project Information

**Project:** VYBORA — E-Commerce Website Hosting on AWS S3  
**Category:** Cloud Computing / AWS / Static Website Hosting  
**Frontend:** HTML, CSS, JavaScript  
**Cloud Service:** Amazon S3


⭐ If you find this project useful, feel free to explore the repository and share feedback.

*Built as a hands-on AWS learning project focused on Amazon S3 static website hosting.*