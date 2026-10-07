<div align="center">

# 🛡️ Ubuntu CIS Hardening & Audit Script

**Скрипт аудиту та харденінгу Ubuntu за CIS Benchmarks**

![Bash](https://img.shields.io/badge/Bash-Script-4EAA25?logo=gnubash&logoColor=white)
![Ubuntu](https://img.shields.io/badge/OS-Ubuntu-E95420?logo=ubuntu&logoColor=white)
![CIS](https://img.shields.io/badge/Standard-CIS%20Benchmarks-1F4E79)
![Focus](https://img.shields.io/badge/Focus-Linux%20Hardening-critical)

🇺🇦 [Українська версія](#ua) · 🇬🇧 [English version](#en)

</div>

---

<a id="ua"></a>

# 🇺🇦 Українська версія

## 📌 Про проєкт

Проєкт автоматизує базовий **аудит та харденінг** (зміцнення безпеки) операційної системи Ubuntu відповідно до вимог **CIS (Center for Internet Security) Benchmarks**.

Він демонструє практичні навички системного адміністрування Linux та кібербезпеки.

## 🛡️ Що перевіряє скрипт

| Область | Перевірка |
|---|---|
| **Безпека SSH** | Заборона входу `root` та інші критичні параметри SSH-демона |
| **Брандмауер (UFW)** | Статус брандмауера та політики за замовчуванням (`deny incoming`) |
| **Права доступу** | Права на чутливі системні файли (`/etc/shadow`, `/etc/passwd`) |
| **Системні служби** | Виявлення потенційно зайвих або небезпечних сервісів |

## 🚀 Швидкий старт

**1. Склонуйте репозиторій:**

```bash
git clone https://github.com/your-username/ubuntu-cis-hardening.git
cd ubuntu-cis-hardening
```

> 💡 Замініть `your-username` на ваш логін на GitHub.

**2. Надайте скрипту права на виконання:**

```bash
chmod +x cis_audit.sh
```

**3. Запустіть скрипт із правами суперкористувача:**

```bash
sudo ./cis_audit.sh
```

## ⚠️ Застереження

Запускайте скрипт на **власних** системах або в лабораторному середовищі. Перед застосуванням змін на робочих серверах протестуйте їх на тестовій машині. Результати аудиту є орієнтиром і не замінюють повний аудит за офіційним CIS Benchmark.

---

<a id="en"></a>

# 🇬🇧 English version

## 📌 About

This project automates basic **auditing and hardening** of an Ubuntu operating system in compliance with **CIS (Center for Internet Security) Benchmarks**.

It showcases practical skills in Linux system administration and cybersecurity.

## 🛡️ What the Script Checks

| Area | Check |
|---|---|
| **SSH Security** | `root` login restrictions and other critical SSH daemon settings |
| **Firewall (UFW)** | Firewall status and default incoming traffic policy (`deny incoming`) |
| **File Permissions** | Permissions on sensitive system files (`/etc/shadow`, `/etc/passwd`) |
| **System Services** | Detection of potentially unnecessary or insecure services |

## 🚀 Quick Start

**1. Clone the repository:**

```bash
git clone https://github.com/your-username/ubuntu-cis-hardening.git
cd ubuntu-cis-hardening
```

> 💡 Replace `your-username` with your actual GitHub username.

**2. Make the script executable:**

```bash
chmod +x cis_audit.sh
```

**3. Run the script with superuser privileges:**

```bash
sudo ./cis_audit.sh
```

## ⚠️ Disclaimer

Run this script on **your own** systems or in a lab environment. Test any changes on a non-production machine first. Audit results are a guideline and do not replace a full assessment against the official CIS Benchmark.
