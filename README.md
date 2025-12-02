# 🚀 API Testing with Postman, Newman & Allure

This repository contains automated API tests built using **Postman Collections**, executed via **Newman**, and reported with **Allure Reports**.

---

## 🔧 Running Tests

### *Run Collection with Environment**
```
newman run postman/collection.postman_collection.json \
    -e postman/environment.postman_environment.json
```

### **Run Newman with Allure**
```
newman run postman/collection.postman_collection.json \
    -e postman/environment.postman_environment.json \
    -r allure
```

### **Generate Allure Report**
```
allure generate allure-results --clean --single-file
```
