# What is Static Website?
Static Website is consist of fixed content written in HTML, CSS, JS. It dose not need backend or server-side logic everything is pre-build and servered as is . like Portfolio website, documentation pages, landing pages
## Basic Requirement 
1. HTML/CSS/JS
2. Web Server
3. Domain Name
4. Hosting

## Hosting Option for static sites
| Platform           | Features                                                                |
|--------------------|-------------------------------------------------------------------------|
| **GitHub Pages**    | Free and easy to use with GitHub repository                            |
| **Netlify**         | Fast, CDN-backed, drag-and-drop support, generous free tier            |
| **Vercel**          | Super fast, optimized for React and Next.js                            |
| **Amazon S3**       | Scalable and integrates well with other AWS services                   |
| **Cloudflare Pages**| Fast global delivery, Git-integrated                                   |





# CDN (Contant Delvery Network)
It is a network of srever distributed to deliver static content faster to users.
It has fastest caues of nereast location avalibality
It can be able to handel large traffic
It can be reliable : if onee server fails other can handle it 
liks : cloudflare CDN, AWS cloudflare, fastly and others

# SNS (Simple Notification Service)
A massage service , used to send notification, alarms, alarts
Notify via email or SMS if cludflare is invalidated
* ⚠️ SNS is optional for static hosting but useful in event-driven scenarios.

# Cloudflare 
| Feature             | Role in Static Hosting                                              |
|---------------------|---------------------------------------------------------------------|
| **CDN**             | Speeds up the delivery globally                                     |
| **DNS Management**  | Fast and secure domain resolution                                   |
| **SSL/TLS**         | Free HTTPS support (with auto-renewal)                              |
| **Firewalls & DDoS**| Protects against attacks                                            |
| **Page Rules**      | Custom redirects, caching behaviors, and other rules                |
| **Cloudflare Pages**| Full static site hosting platform                                   |

# OTP Implementation
One time password used for secure login, sinup, verification and others
we need Bcaked or APIs to generate and verify OTP , and
We need Database to match OTP with user session
### workaround
Use Firebase authentication to support OPT via mail/phone
Use serveless function like AWS Lambda, Netlify function
COnnect static frontend to backend API via AJAX/fetch


# URL Management
Each page/file should be served via URL and it should be clean SEO-friendly and case senstive


*** folder structure example :
/static-website
|- index.html
|- about.html
|- assests
|   |- style.css
|   |- script.js




### Summary

| Concept            | Purpose                          | Mandatory for Static Site?         |
|--------------------|----------------------------------|------------------------------------|
| **HTML/CSS/JS**    | Create content                   | ✅ Yes                             |
| **Hosting (S3, Netlify)** | Store and serve content       | ✅ Yes                             |
| **CDN (Cloudflare, CloudFront)** | Speed up delivery            | ✅ Highly recommended              |
| **DNS + URL**       | Access via custom domain         | ✅ Yes                             |
| **SSL/HTTPS**       | Secure your website              | ✅ Yes                             |
| **OTP**             | Auth for users (needs backend/API)| ❌ Optional + needs backend        |
| **SNS**             | Notifications (event-driven)     | ❌ Optional                        |

