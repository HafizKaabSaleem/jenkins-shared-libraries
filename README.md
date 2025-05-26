# Jenkins Shared Libraries for CI/CD Pipelines

This repository contains custom Jenkins Shared Libraries to standardize and simplify CI/CD pipelines across multiple projects. It helps in maintaining reusable pipeline code, improving consistency, and reducing duplication.

## 📌 Features

- ✅ Centralized and reusable pipeline logic using `vars/` and `src/` directories.
- ✅ Custom pipeline steps for build, test, deploy, and notifications.
- ✅ Cleanly organized Groovy code for better readability and modularity.
- ✅ Easy integration with Jenkins `Jenkinsfile` using `@Library`.

## 📁 Project Structure

jenkins-shared-libraries/
├── vars/
│ └── myPipeline.groovy # Custom pipeline logic exposed as a global function
├── src/
│ └── org/example/Utils.groovy # Utility class with helper methods
└── resources/
└── notifications.txt # Optional resources (e.g., templates)


## 🚀 How to Use

1. Clone or reference this repo in your Jenkins instance.
2. In your project’s `Jenkinsfile`, use the shared library like this:

```groovy
@Library('jenkins-shared-libraries') _
myPipeline()

    Customize and expand myPipeline.groovy and utility classes as per your workflow.

📦 Benefits

    Reduces code duplication across Jenkinsfiles.

    Easy maintenance of complex pipelines.

    Promotes DRY (Don't Repeat Yourself) principles.

    Encourages team-wide best practices.

📚 Requirements

    Jenkins with Scripted/Declarative Pipeline support.

    GitHub or internal SCM integration.

    Proper configuration of Shared Library path in Jenkins global settings.

🔗 Author

Made with 💻 by Hafiz Kaab Saleem
📎 LinkedIn www.linkedin.com/HafizKaabSaleem
📂 More Projects on GitHub https://github.com/HafizKaabSaleem)
📝 This project is licensed under the [MIT License](LICENSE).

This project is open-source and available under the MIT License.
