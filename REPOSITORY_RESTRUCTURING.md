<div align="center">

# <img src="OSLogo.png" align="middle" height="48"> Repository Architecture & Restructuring

</div>

Mithl-OS has transitioned to a **Dual-Repository Model**. This strategic move ensures elite code quality, security, and a professional development environment while maintaining seamless accessibility for end-users.

---

## 🏛️ The Dual-Repository Model

```mermaid
flowchart LR
    subgraph Private ["🔒 Private Development Repo"]
        direction TB
        Code["📜 Source Code<br/>(C, Assembly, HAL)"]
        Build["⚙️ Build System<br/>(Make, Linker)"]
        Review["👔 Code Review & CI"]
    end

    subgraph Public ["🌍 Public Distribution Repo"]
        direction TB
        ISO["💿 ISO Images<br/>(Releases)"]
        Notes["📝 Release Notes"]
        Docs["📚 User Documentation"]
    end

    Private -- "✅ Build Stable" --> ISO
    Private -- "📄 Extract" --> Notes
    Public -- "📥 User Access" --> EndUser["👤 OS User"]
    EndUser -- "📝 Application" --> Private
```

---

## 📊 Infrastructure Comparison

| Feature | 🔒 Private Dev Repo | 🌍 Public Dist Repo |
| :--- | :--- | :--- |
| **URL** | `https://github.com/.../Mithl` | `.../Mithl/releases` |
| **Access** | 🔑 Approved Contributors | 👥 Everyone |
| **Primary Content** | Full Source Code & Toolchain | Pre-built ISOs & User Docs |
| **Visibility** | Hidden from Public | Fully Public |
| **Purpose** | Active Development | Distribution & Usage |

---

## ⚡ Contribution Workflow

Interested in building the future of OS? Follow our elite onboarding process.

```mermaid
stepper
  step 1 : "Visit [Contribute Page](https://doguparthiaakash.github.io/Mithl/contribute.html)"
  step 2 : "Fill Application Form (Skills, Motivation, Portfolio)"
  step 3 : "Internal Review (3-5 Business Days)"
  step 4 : "Receive 🔑 Private Access & Onboarding Docs"
  step 5 : "Start Contributing to Core!"
```

> [!IMPORTANT]
> **Why Private?** OS development requires high-integrity code review. Our private model ensures every line of code meets our strict performance and security standards before it ever reaches a public release.

---

## 📦 User Workflow (Quick Start)

For those who want to experience Mithl-OS immediately:

1.  **Visit** the [Public Releases](https://github.com/DoguparthiAakash/Mithl/releases).
2.  **Download** the latest timestamped `Mithl-latest.iso`.
3.  **Boot** in QEMU or flash to a USB drive.
4.  **Enjoy** the distraction-free workspace!

---

## 📝 Change Log Summary

The following files have been synchronized with the new repository architecture:

- `index.html`: Updated navigation to point to public distributions.
- `contribute.html`: Redesigned with a professional application form.
- `README.md`: Transformed into a high-impact project presentation.
- `REPOSITORY_RESTRUCTURING.md`: Detailed architecture documentation.

---

<div align="center">

*Professional. Secure. Open for Visionaries.*

**Mithl-OS Team**

</div>
