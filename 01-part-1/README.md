# Part 1: [Part Title Here]

```markdown
# Part 1: Setting Up Your Development Environment with Devbox

**Blog Post:** [https://cloudikeme.com/devbox-setting-up-your-development-environment](https://cloudikeme.com/devbox-setting-up-your-development-environment)

**Code:** [This directory!](.)

This part of the "Mastering Microservices" series will guide you through setting up a consistent development environment using **Devbox**. Devbox helps you avoid manual installations and configurations of essential tools, so you can focus on building microservices.

## Why Devbox?

Devbox provides:

* **Isolation:** A self-contained environment that won't interfere with your system.
* **Reproducibility:**  Ensures all developers have the same setup.
* **Ease of Use:** Automates the installation of Docker, Kubernetes, Terraform, and other tools.

## Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/cloudikeme/mastering-microservices-with-kubernetes-terraform-azure.git
   ```

2. **Navigate to the Part 1 directory:**
   ```bash
   cd mastering-microservices-with-kubernetes-terraform-azure/01-part-1
   ```

3. **Install Devbox (if you haven't already):**
   * **Linux/macOS:**
     ```bash
     curl -fsSL https://get.jetpack.io/devbox | bash
     ```
   * **Windows:** Follow the instructions in the [Devbox WSL documentation](https://www.jetpack.io/devbox/docs/wsl/).

4. **Verify Devbox installation:**
   ```bash
   devbox --version
   ```

5. **Activate the Devbox environment:**
   ```bash
   cd devbox 
   devbox shell
   ```

   Devbox will download and install the necessary tools.  You'll see a change in your terminal prompt, indicating you're inside the Devbox environment.

## Tools Included

The Devbox configuration file (`devbox.json` in this directory) will install:

* **Docker**
* **kubectl** 
* **Terraform**
* **Node.js & npm**
* **Go**
* **Git**
* **GitHub CLI (gh)**
* **kind**

## Verify Tool Installation

After activating the Devbox environment, run the following commands to check if the tools are installed correctly:

```bash
docker --version
kubectl version --client
terraform --version
node --version
go version
git --version
```

You should see the version information for each tool, confirming that your Devbox environment is working as expected.

## Manual Installation (Optional)

If you prefer to install the tools manually, you can find instructions for each tool in the blog post:  [https://cloudikeme.com/devbox-setting-up-your-development-environment](https://cloudikeme.com/devbox-setting-up-your-development-environment)

## Troubleshooting

For Devbox-related issues, refer to the official documentation: [https://www.jetpack.io/devbox/docs/](https://www.jetpack.io/devbox/docs/)

## What's Next?

Now that your development environment is set up, move on to [Part 2: Create a Repository Using Git and GitHub CLI](/your-blog-post-2-url) to start managing your project with Git.
```

**Key Improvements:**

* **Clear Path:**  Provides step-by-step instructions specific to this directory.
* **Concise Information:**  Focuses on essential setup details. 
* **Consistent Formatting:** Uses clear headings, lists, and code blocks.
* **Links to Resources:**  Links to the blog post and Devbox documentation for further help.