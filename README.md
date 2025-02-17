# 🚀CloudCart - Static Website Hosting on AWS S3 with  Domain  

## 🌟 Project Overview  
This project demonstrates how to *host a static website* using *Amazon S3* and configure a *custom domain (GoDaddy)* with *AWS Route 53* for seamless DNS management.  

## 🛠️ Prerequisites  
✅ *AWS Account* with S3 and Route 53 access  
✅ *GoDaddy Domain* (e.g., shoppingcarts.life)  
✅ *Basic HTML & CSS Website Files*  

---

## 📌 Steps to Host Your Static Website  

### 🔹 1. Create an S3 Bucket  
🔹 *Go to* [AWS S3 Console](https://s3.console.aws.amazon.com/)  
🔹 Click *Create Bucket*  
🔹 Set *Bucket Name* = shoppingcarts.life  
🔹 Choose *Region* (e.g., *Singapore*)  
🔹 Enable *Static Website Hosting*  
🔹 Copy *S3 Website Endpoint*  

---

### 🔹 2. Upload Website Files  
📂 Open *S3 Bucket → Upload*  
📂 Add *HTML, CSS, and images*  
🔓 *Set Public Read Access* for files  

---

### 🔹 3. Configure Route 53  
🌍 Go to *AWS Route 53 Console*  
🌍 Click *Create Hosted Zone*  
🌍 Enter *Domain Name* = shoppingcarts.life  
📋 Copy *NS (Name Server) Records*  

---

### 🔹 4. Update GoDaddy Nameservers  
🌐 Log in to *GoDaddy*  
🌐 Navigate to *Domain Settings*  
🌐 Click *Manage DNS → Change Nameservers*  
🌐 Paste *Route 53 NS Records*  
⏳ *Save & Wait for DNS Propagation*  

---

### 🔹 5. Create a Route 53 Record  
📍 Go to *Route 53 → Hosted Zone → shoppingcarts.life*  
📍 Click *Create Record*  
📍 Select *A Record* (Alias: *Yes*)  
📍 Choose *S3 Website Endpoint*  
✅ *Save the record*  

---

### 🔹 6. Test Your Website  
🖥️ Open *http://shoppingcarts.life* in a browser  
✅ *Verify if the website loads correctly*  

---

## ⚠️ Troubleshooting  
🔴 *Website Not Loading?*  
- Wait for *DNS propagation* (can take *up to 48 hours*)  

🔴 *S3 Bucket Shows Forbidden (403) Error?*  
- Check *Bucket Policy* and enable *public access*  

🔴 *S3 Endpoint Not Showing in Route 53?*  
- Ensure *Static Website Hosting is Enabled* in S3  

---

## 🔮 Future Enhancements  
🔒 *Enable HTTPS* using *AWS CloudFront*  
📊 *Monitor Traffic* with *AWS CloudWatch*  
🚀 *Automate Deployments* with *CI/CD Pipelines*  

---

link : https://drive.google.com/drive/folders/1Msm99sjgdqAncwEsdbsnqICHF1WC28aq
