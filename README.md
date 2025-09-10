# My DevOps CI/CD Demo Project

Welcome to the **my-devops-demo** repository! This project showcases a simple DevOps CI/CD pipeline,
using GitHub Actions, designed to demonstrate automated testing, validation, and deployment workflows.

---

## 🚀 Project Purpose

This repository is a hands-on demo for learning and experimenting with CI/CD concepts:
- Automated build and test steps
- HTML validation using the W3C validator and HTMLHint
- Workflow orchestration via GitHub Actions

---

## ⚙️ Technologies Used

- **GitHub Actions:** Automates CI/CD workflows
- **HTMLHint:** Linting and validation for HTML files
- **W3C Validator (vnu.jar):** HTML standard validation
- **Node.js:** For installing CLI tools
- **Shell scripting:** Basic automation

---

## 🛠️ Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/AndreiChiuzbaian/my-devops-demo.git
   cd my-devops-demo
   ```

2. **Explore the workflows**
   - Workflows are defined in `.github/workflows/`
   - Example: `html-validate.yml` runs HTML validation on push to `main`

---

## 🚦 CI/CD Workflow Summary

- **On Push to Main Branch:**
  - Checks out the repository code
  - Installs required tools (Node.js, HTMLHint)
  - Runs HTML validation (`vnu.jar` and/or HTMLHint)
  - Reports results in the GitHub Actions tab

---

## 📂 Project Structure

```
my-devops-demo/
├── .github/
│   └── workflows/
│       └── main.yml
├── index.html
├── README.md
```

---

## 🧪 Running Locally

You can run HTMLHint locally:
```bash
npm install -g htmlhint
htmlhint index.html
```

For W3C validation:
1. Download [vnu.jar](https://github.com/validator/validator/releases/latest)
2. Run:
   ```bash
   java -jar vnu.jar index.html
   ```

---

## 🤝 Contributing

Contributions are welcome! Please fork the repo and submit pull requests.  
Suggestions for improving the CI/CD pipeline or adding new workflows are appreciated.

---

## 📄 License

This project is licensed under the MIT License.

---

## 📬 Contact

Questions? Reach out via GitHub Issues or contact me (https://github.com/AndreiChiuzbaian).
