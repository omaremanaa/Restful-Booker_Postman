# 🚀 API Testing with Postman, Newman & Allure

This repository contains automated API tests built using **Postman Collections**, executed via **Newman**, and reported with **Allure Reports**.

---

## 🔧 Running Tests

### *Run Collection with Environment**
```
newman run Restful_GP_env.postman_environment.json \
    -e Restful-Booker-GP.postman_collection.json
```

### **Run Newman with Allure**
```
newman run Restful_GP_env.postman_environment.json \
    -e Restful-Booker-GP.postman_collection.json \
    -r allure
```

### **Generate Allure Report**
```
allure generate allure-results --clean --single-file
```
