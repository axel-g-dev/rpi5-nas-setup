<h1 align="center"> NAS Samba Project on Raspberry Pi 5</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Raspberry%20Pi-5-red?logo=raspberrypi" alt="Raspberry Pi">
  <img src="https://img.shields.io/badge/Bash-Scripting-blue?logo=gnu-bash" alt="Bash">
  <img src="https://img.shields.io/badge/Linux-Automation-green?logo=linux" alt="Linux">
  <img src="https://img.shields.io/badge/Samba-NAS-yellow?logo=samba" alt="Samba">
  <img src="https://img.shields.io/badge/License-MIT-lightgrey" alt="MIT License">
</p>

---

>  **Project completed in 3 sessions** to design an **autonomous and functional NAS (Network Attached Storage)** using a **Raspberry Pi 5**.
> The goal was to create a reliable file-sharing service with **Samba**, along with installation, automation, and user management scripts.
>  *All the documentation and tutorials are written in French.*

---

##  Project Objective

This project transforms a **Raspberry Pi 5** into a **personal NAS** capable of:

* Sharing folders over the local network (public & private).
* Automatically handling USB mounting and Samba configuration.
* Easily adding Samba users via a custom script.
* Keeping detailed **log files** for better system monitoring.

---

##  Why I chose **Samba**

I chose **Samba** because it is the **simplest and most universal solution** for sharing files between different operating systems (Windows, Linux, macOS).
Here are the main reasons behind this choice:

1.  **Full Compatibility**
   Samba uses the **SMB/CIFS protocol**, the same one used by Windows file sharing.
   This allows seamless access to the NAS from any device on the local network.

2.  **Ease of Installation and Management**
   Installing Samba is very straightforward (`sudo apt install samba`), and all configuration is handled in a single file (`/etc/samba/smb.conf`).

3.  **User and Permission Management**
   Samba allows secure user creation, precise permission control (read-only, read/write), and the ability to separate public and private directories.

4.  **Perfect Integration with Linux**
   Samba works smoothly on Raspberry Pi OS (Linux). It is lightweight, reliable, and ideal for a learning or demonstration project.

---

##  Project Structure

```bash
Projet-NAS/
├── Séance1/
│   └── Documentation.md
│
├── Séance2/
│   ├── Checklist.md
│   ├── Documentation-2.md
│   ├── Suivi-avancement-1.md
│   └── Suivi-avancement-2.md
│
├── Séance3/
│   ├── Scripts/
│   │   ├── install_nas_autoreboot.sh
│   │   └── add_samba_user.sh
│   ├── Cahier-des-charges-NAS.md
│   ├── Documentation-3.md
│   ├── Fiche-Recette-NAS.md
│   ├── Gantt.md
│   ├── Suivi-avancement-3.md
│   ├── Tutoriel-Complet.md
│   └── statuts.md
├── img/
│
└── README.md
```

---

##  Project Organization

The project was divided into **3 sessions**, each representing a stage of development and documentation.

###  **Session 1 – Preparation**

* Installation and initial setup of the Raspberry Pi.
* Definition of goals and creation of the **project specification**.
   *See:* `Séance1/Documentation.md`

---

###  **Session 2 – Development**

* Setup of the first Samba shares.
* Creation of public and private directories.
* Progress tracking and validation checklists.
   *See:*
  `Séance2/Documentation-2.md`
  `Séance2/Checklist.md`
  `Séance2/Suivi-avancement-1.md`
  `Séance2/Suivi-avancement-2.md`

---

###  **Session 3 – Automation and Finalization**

* Development of **Bash scripts**:

  * `install_nas_autoreboot.sh` → installs and configures the Samba NAS automatically.
  * `add_samba_user.sh` → creates a Samba user with a personal private folder.
* Creation of a **systemd service** for automatic startup at boot.
* Final documentation and validation of the project.
   *See:*
  `Séance3/Tutoriel-Complet.md` *(step-by-step guide)*
  `Séance3/Documentation-3.md`
  `Séance3/Fiche-Recette-NAS.md`
  `Séance3/Gantt.md`
  `Séance3/Suivi-avancement-3.md`

---

##  Global Overview

The configured NAS is:

* **Autonomous** – starts automatically with the Raspberry Pi.
* **Accessible** – accessible via the local network (`\\IP_RASPBERRY\public` / `\\IP_RASPBERRY\prive`).
* **Secure** – each Samba user has a private, isolated space.
* **Documented** – every stage is explained in the session folders.

---

##  Additional Resources

*  **Full tutorial:** `Séance3/Tutoriel-Complet.md`
*  **Project specifications:** `Séance3/Cahier-des-charges-NAS.md`
*  **Validation sheet:** `Séance3/Fiche-Recette-NAS.md`
*  **Gantt chart:** `Séance3/Gantt.md`
*  **Scripts:** `Séance3/Scripts/`

---

## Author

**GitHub:** [@axel-g-dev](https://github.com/axel-g-dev)

> Educational project made with **Raspberry Pi 5**, focused on **Linux administration**, **networking**, and **automation**.
> *All documentation and comments are written in French.*

---

## License

This project is distributed under the **MIT License** — free to use, modify, and share.

```text
MIT License  
Copyright (c) 2025
```

<p align="center">
  <img src="https://img.shields.io/badge/Made%20with-Linux%20%26%20Love-black?logo=linux" alt="Made with Linux">
</p>

---

## Status Badges Used in Documentation

![In Progress](https://img.shields.io/badge/Status-In%20Progress-yellow)
![Not Started](https://img.shields.io/badge/Status-Not%20Started-lightgrey)
![Completed](https://img.shields.io/badge/Status-Completed-brightgreen)

![Not Valid](https://img.shields.io/badge/Status-Not%20Valid-red)
![Partially Valid](https://img.shields.io/badge/Status-Partially%20Valid-lightgrey)
![Validated](https://img.shields.io/badge/Status-Validated-brightgreen)

