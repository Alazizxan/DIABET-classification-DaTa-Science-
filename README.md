# 📈 Analysis of Diabetes Data Set

[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://www.python.org/)




![Diabetes Risk Factors](diabet.jpg)



## Overview

**EN:** In this notebook, we will analyze factors that impact diabetes and explore ways to mitigate them using the dataset features.

**UZ:** Ushbu daftarda biz diabetga ta'sir qiluvchi omillarni tahlil qilamiz va datasetdagi xususiyatlardan foydalanib ularni kamaytirish yo'llarini o'rganamiz.



[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alazizxan/DIABET-classification-DaTa-Science-)


## Files Included
- `housing_data.csv`: Dataset containing housing information.
- `TASHKENT_home.ipynb`: Jupyter notebook with complete code and explanations.


## 🔍 Dataset Features

| Feature                | Description (EN)                  | Description (UZ)                        |
|------------------------|-----------------------------------|-----------------------------------------|
| **Pregnancies**        | Number of pregnancies             | Homiladorlik soni                       |
| **Glucose**            | Glucose level in blood            | Qondagi glyukoza darajasi               |
| **BloodPressure**      | Blood pressure measurement        | Qon bosimi o'lchovi                     |
| **SkinThickness**      | Thickness of the skin             | Teri qalinligi                          |
| **Insulin**            | Insulin level in blood            | Qondagi insulin darajasi                |
| **BMI**                | Body mass index                   | Tana massasi indeksi                    |
| **DiabetesPedigreeFunction** | Diabetes percentage              | Diabet foizi                             |
| **Age**                | Age                               | Yosh                                    |
| **Outcome**            | Final result (1: YES, 0: NO)      | Yakuniy natija (1: HA, 0: YO'Q)         |

## 📝 Analysis

### 🧩 Diabetes and Pregnancy

**EN:** Gestational diabetes is a condition that can occur during pregnancy when the body cannot produce enough insulin, especially common in the second or third trimester. Risk factors include high BMI, previous delivery of a large baby, past gestational diabetes, and certain ethnic backgrounds.

**UZ:** Gestatsion diabet homiladorlik paytida, ayniqsa ikkinchi yoki uchinchi trimestrda tananing etarli insulin ishlab chiqara olmasligi holati. Xavf omillariga yuqori tana massasi indeksi, katta bola tug'ganlik, avvalgi gestatsion diabet va ma'lum etnik guruhlarga mansublik kiradi.

### 👪 Family Health History and Diabetes

**EN:** Having a family history of diabetes increases the chances of developing prediabetes and type 2 diabetes. This risk is higher if there is a history of gestational diabetes, obesity, or belonging to specific ethnic groups. Early screening is recommended with a family history.

**UZ:** Oilaviy anamnezda diabet bo'lishi prediabet va 2-toifa diabet rivojlanish ehtimolini oshiradi. Bu xavf, agar oilaviy anamnezda gestatsion diabet, semizlik yoki ma'lum etnik guruhlarga mansublik bo'lsa, yuqoriroq bo'ladi. Oilaviy anamnezda diabet bo'lsa, erta skrining tavsiya etiladi.

### 📊 BMI and Diabetes Risk

**EN:** BMI, which compares height to weight, is a critical measure. Excess belly fat, measured by waist circumference, increases the risk of type 2 diabetes, heart disease, and stroke. Managing weight through healthy lifestyle choices can mitigate these risks.

**UZ:** Tana massasi indeksi (BMI) bo'yi va vaznni taqqoslaydigan muhim o'lchovdir. Bel atrofi o'lchovlari orqali o'lchangan ortiqcha qorin yog'i 2-toifa diabet, yurak kasalliklari va insult xavfini oshiradi. Sog'lom turmush tarzini tanlash orqali vaznni boshqarish bu xavflarni kamaytirishi mumkin.

---

## 🚀 Methodology / Metodologiya
**EN:** This project involves the following steps and methods:
1. Data Preprocessing:
   - Loading the dataset
   - Handling missing values
   - Feature scaling using `StandardScaler`
2. Exploratory Data Analysis (EDA):
   - Visualization using `matplotlib` and `seaborn`
   - Correlation analysis
3. Model Training:
   - Splitting the data into training and testing sets using `train_test_split`
   - Training various machine learning models:
     - Multi-layer Perceptron (`MLPClassifier`)
     - K-Nearest Neighbors (`KNeighborsClassifier`)
     - Support Vector Machine (`SVC`)
     - Gaussian Process (`GaussianProcessClassifier` with `RBF` kernel)
     - Decision Tree (`DecisionTreeClassifier`)
     - Random Forest (`RandomForestClassifier`)
     - AdaBoost (`AdaBoostClassifier`)
     - Naive Bayes (`GaussianNB`)
     - Quadratic Discriminant Analysis (`QuadraticDiscriminantAnalysis`)
4. Model Evaluation:
   - Accuracy and log loss calculation using `accuracy_score` and `log_loss`
   - Comparison of model performances

**UZ:** Ushbu loyiha quyidagi qadamlar va metodlarni o'z ichiga oladi:
1. Ma'lumotlarni oldindan qayta ishlash:
   - Datasetni yuklash
   - Yo'qolgan qiymatlarni boshqarish
   - `StandardScaler` yordamida xususiyatlarni masshtablash
2. Tadqiqotchi Ma'lumotlar Tahlili (EDA):
   - `matplotlib` va `seaborn` yordamida vizuallashtirish
   - Korelatsiya tahlili
3. Modelni Trening:
   - Ma'lumotlarni trening va test to'plamlariga ajratish (`train_test_split` yordamida)
   - Turli xil mashinasozlik modellarini o'rgatish:
     - Ko'p qatlamli Perseptoron (`MLPClassifier`)
     - K-eng yaqin qo'shnilar (`KNeighborsClassifier`)
     - Qo'llab-quvvatlash Vektor Mashinasi (`SVC`)
     - Gauss Prosessi (`GaussianProcessClassifier` va `RBF` yadrosi bilan)
     - Qaror daraxti (`DecisionTreeClassifier`)
     - Tasodifiy o'rmon (`RandomForestClassifier`)
     - AdaBoost (`AdaBoostClassifier`)
     - Naiv Bayes (`GaussianNB`)
     - Kvadratik Diskriminant Analiz (`QuadraticDiscriminantAnalysis`)
4. Modelni Baholash:
   - Aniqlik va log loss hisoblash (`accuracy_score` va `log_loss` yordamida)
   - Modellar ish faoliyatini solishtirish

---


## ⚖️ Diabetes Risk Factors Importance / Diabet Xavf Ommillari Muhimligi

**EN:** 🔍 Understanding these factors is crucial for proactive health management:
- Early detection of gestational diabetes through pregnancy screening can lead to effective management and reduce risks for both mother and baby.
- Knowing your family's history of diabetes helps assess personal risk and enables timely preventive measures such as screenings and lifestyle adjustments.
- Monitoring BMI and waist circumference helps manage weight, reduce belly fat, and lower the risk of developing type 2 diabetes and related health issues.

**UZ:** 🔍 Ushbu omillarni tushunish faol sog'liqni saqlashni boshqarish uchun muhimdir:
- Homiladorlik paytida skrining orqali gestatsion diabetni erta aniqlash samarali boshqarishga olib kelishi va ona va bola uchun xavflarni kamaytirishi mumkin.
- Oilaviy anamnezda diabet mavjudligini bilish shaxsiy xavfni baholashga yordam beradi va skrininglar va turmush tarzi o'zgarishlari kabi oldini olish choralarini vaqtida amalga oshirish imkonini beradi.
- BMI va bel atrofi o'lchovlarini kuzatib borish vaznni boshqarishga, qorin yog'ini kamaytirishga va 2-toifa diabet va bog'liq sog'liq muammolari rivojlanish xavfini kamaytirishga yordam beradi.

## Contributors
- [Alazizxan](https://github.com/Alazizxan)

## Badge
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
