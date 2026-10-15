# CipherEye# CipherEye 🔐👁️

**Sensitive Data Detection & Security Monitoring**

CipherEye is a cybersecurity project designed to identify sensitive information exposed within files and assess the potential security risk.

The goal is to build a tool that helps users understand **what sensitive data they have, where it is exposed, and how serious the exposure is.**

> **Scan. Detect. Assess. Protect.**

---

## 🎯 Project Goals

CipherEye aims to:

* Scan files and directories for sensitive information
* Detect potentially exposed credentials and personal data
* Categorise security findings
* Calculate a risk level for each finding
* Generate clear security reports
* Monitor files for potentially dangerous changes
* Eventually provide a web-based security dashboard

---

## 🔍 What CipherEye Will Detect

The detection engine will eventually support patterns such as:

* 🔑 Passwords
* 🔐 API keys
* 🪪 Identification numbers
* 💳 Credit-card-like numbers
* 📧 Email addresses
* 📱 Phone numbers
* 🌐 IP addresses
* 🗄️ Database credentials
* 🔏 Private keys

Detection capabilities will be expanded as the project develops.

---

## 🏗️ Project Architecture

The initial architecture is built around several independent components:

```text
                    CipherEye
                        │
                        ▼
                  File Scanner
                        │
                        ▼
                Detection Engine
                        │
                        ▼
                   Risk Engine
                        │
                        ▼
                    Reporter
```

Each component is designed to have a specific responsibility so that the system can be expanded without tightly coupling the entire application.

---

## 🛠️ Technology Stack

### Current

* Python
* Regular Expressions
* Pytest

### Planned

* FastAPI
* PostgreSQL
* SQLAlchemy
* Docker
* HTML / CSS / JavaScript
* CI/CD

The technology stack may change as the project evolves.

---

## 🚧 Development Status

**Current version: `0.1.0` — In Development**

### Completed

* [ ] Project structure
* [ ] File scanner
* [ ] Sensitive data detection
* [ ] Risk scoring
* [ ] CLI security report

### Planned

* [ ] PostgreSQL integration
* [ ] FastAPI backend
* [ ] Web dashboard
* [ ] File integrity monitoring
* [ ] Security alerts
* [ ] Dockerisation
* [ ] CI/CD pipeline

---

## 🧪 Testing

CipherEye will use automated tests to verify the behaviour of individual components.

Tests will cover:

* File scanning
* Sensitive data detection
* Risk classification
* Report generation

---

## 🔒 Security Considerations

CipherEye is designed as a security-focused project, so protecting the data being scanned is an important part of its development.

The project will aim to:

* Avoid storing sensitive information unnecessarily
* Avoid exposing detected secrets in reports
* Provide safe handling of scanned files
* Separate detection from sensitive-data storage
* Follow secure development practices

**CipherEye should not be used as a replacement for professional security auditing.**

---

## 📚 Project Documentation

Additional project documentation can be found in the `docs/` directory.

Planned documentation includes:

* System architecture
* Security model
* Development plan

---

## 🚀 Future Vision

The long-term goal is to turn CipherEye from a simple file scanner into a security monitoring platform.

```text
             ┌─────────────────────┐
             │      CipherEye      │
             └──────────┬──────────┘
                        │
             ┌──────────▼──────────┐
             │   Detection Engine  │
             └──────────┬──────────┘
                        │
             ┌──────────▼──────────┐
             │     Risk Engine     │
             └──────────┬──────────┘
                        │
              ┌─────────▼─────────┐
              │ Security Database │
              └─────────┬─────────┘
                        │
              ┌─────────▼─────────┐
              │     Dashboard     │
              └───────────────────┘
```

Future versions may include continuous monitoring, alerts, historical security data, and visual analytics.

---

## 👤 Author

**Lebogang Nare**

This project is being developed as a personal cybersecurity and software engineering project.
