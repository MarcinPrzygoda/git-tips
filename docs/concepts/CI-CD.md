# 📋 CI/CD

## 📌 Continuous Integration (CI)

- code changes must be **committed** and **built frequently**
- code changes are **validated** by creating a build and running **automated tests** against the build
- identifies **integration issues** early
- version control serves as the **integration point**

## 📌 Continuous Delivery (CD)

- **extension** of Continuous Integration
- automatically deploys all code changes to a **testing** and/or **production environment** after the build stage
- automates **release process**
- you can deploy your application any time by **clicking a button**

## 📌 Continuous Deployment (CD)

- every change that **passes all stages** of your production pipeline is **released** to your customers
- there's **no human intervention**, and only a failed test will prevent a new change to be deployed to production

See "[Continuous Integration vs. Delivery vs. Deployment](https://www.atlassian.com/continuous-delivery/principles/continuous-integration-vs-delivery-vs-deployment)" for more information.