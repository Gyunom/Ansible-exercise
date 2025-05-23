# 🛠 Apache Server Deployment with Ansible

This project marks a key milestone in my Cloud Engineering/DevOps learning journey, automating the setup of multiple web servers using **Ansible**. I used two EC2 instances running Ubuntu, and wrote a playbook that provisions Apache, installs PHP 8.1, configures the timezone, and hosts a live `index.php` page styled with custom HTML/CSS.

---

## 📸 Project Highlights

* ✅ Spun **two EC2 servers** on AWS (UBUNTU)
* ✅ Installed and configured **Apache and PHP 8.1** from the `ondrej/php` PPA (To replace the default index.html apache ubuntu display)
* ✅ Set the system timezone to `Africa/Lagos`
* ✅ Served a styled `index.php` that displays the live server time
* ✅ Ensured uniform and reproducible server setup via YAML

---

## 📂 Project Structure

```
.
├── playbook2.yml         # Ansible playbook
├── inventory-list        # Inventory file for EC2 instances
├── screenshots/          # Contains Apache status & webpage screenshots
└── README.md             # This file
```

---

## 🔧 What I Learned

* The importance of **modular, repeatable deployments** using Ansible
* How to manage **multiple remote servers** using inventory files
* Writing clean, readable YAML for configuration
* Working with EC2, SSH keys, and Ansible modules like `apt`, `copy`, `timezone`, and `systemd`

---

## 🚀 How to Reuse This

1. Clone the repo
2. Replace the IPs and PEM path in inventory-list
3. Run:

```bash
ansible-playbook -i inventory-list playbook2.yml
```

---

## 🤝 Acknowledgements

Thanks to my Tutor Abubakar Ango for this exercise, the open-source Ansible community and all the great learning resources out there. This project helped me see the value of automation firsthand, and it's only the beginning.

---

## 📬 Let’s Connect!

If you're also learning Cloud Engineering/DevOps, feel free to **[linkedin.com/in/gyunom-maigida-880b362a7](https://www.linkedin.com/in/gyunom-maigida-880b362a7?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BglcZcqqNTpanUrK2OrtQng%3D%3D)** or drop a question!
