# 🖥️ 2-Tier Architecture Deployment of LAMP Stack with WordPress on AWS EC2

This project demonstrates the deployment of a 2-tier architecture using **LAMP stack (Linux, Apache, MariaDB, PHP)** with **WordPress** on **AWS EC2** instances. The app server and database server are hosted on **separate EC2 instances** to simulate a real-world production environment.

---

## 📊 Architecture Overview

```
[ Client ]
↓
[ EC2 App Server ] — runs Apache, PHP, WordPress
↓
[ EC2 DB Server ] — runs MariaDB (port 3306)
```


- **App Server:** Hosts Apache, PHP, and WordPress
- **DB Server:** Hosts MariaDB 10.5
- **Communication:** Done via private IPs in the same VPC

---

## 📁 Project Structure

```
├── 2_Tier_Architecture_Deployment_of_LAMP_Stack.pdf # 📄 Full step-by-step PDF
├── setup.sh # ⚙️ Optional automation script (add if created)
└── README.md # 📘 You're reading this
```


---

## 📄 Documentation

👉 **[Download Project PDF](./2_Tier_Architecture_Deployment_of_LAMP_Stack.pdf)**  
The PDF includes:

- Architecture diagram
- EC2 & Security Group setup
- MariaDB DB server installation & config
- Apache, PHP, WordPress setup on App server
- WordPress configuration
- Troubleshooting & conclusion

---

## 🧰 Technologies Used

- **AWS EC2**
- **Amazon Linux AMI**
- **Apache Web Server**
- **PHP**
- **MariaDB 10.5**
- **WordPress CMS**
- **Bash scripting**
- **Firewall / SELinux**

---

## 🛠️ Setup Summary

1. **Launch 2 EC2 Instances**  
   - App Server  
   - DB Server  

2. **Configure Security Groups**  
   - Allow SSH, HTTP, and MySQL on required ports

3. **Install MariaDB** on DB Server  
   - Configure remote access  
   - Create DB & user

4. **Install Apache, PHP, WordPress** on App Server  
   - Edit `wp-config.php` to connect to DB

5. **Access WordPress** in browser using App Server's public IP  
   - Complete the installation wizard

---

## 📸 Screenshots

> 📌 Refer to the PDF for visual walkthrough of each step  
> (All screenshots are placed in the PDF as per each stage)

---

## 🤖 Automation (Optional)

We are working on a Bash script (`setup.sh`) to automate the full setup. Once done, it will be added here.

---

## 🙋‍♂️ Author

**Aniruddha Kharve**  
📫 [GitHub](https://github.com/Aniruddhakharve)

---

## 📌 License

This project is intended for **educational purposes only**.  


