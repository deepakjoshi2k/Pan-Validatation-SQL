# 📝 PAN Number Validation Project  

## 📌 Objective  
This project focuses on **cleaning and validating PAN (Permanent Account Numbers)** of Indian nationals.  
The goal is to ensure that each PAN number follows the official format and is categorized as either **Valid** or **Invalid**.  

---

## 🔧 Data Cleaning and Preprocessing  

1. **Handle Missing Data**  
   - Identify and manage missing PAN numbers.  
   - Remove rows or impute values depending on context.  

2. **Check for Duplicates**  
   - Ensure no duplicate PAN numbers exist.  
   - Remove duplicates if found.  

3. **Remove Extra Spaces**  
   - Handle leading/trailing spaces in PAN numbers.  

4. **Correct Letter Case**  
   - Convert all PAN numbers to **uppercase**.  

---

## ✅ PAN Format Validation Rules  

A valid PAN number must:  

- Be **exactly 10 characters long**.  
- Follow the format: **`AAAAA1234A`**  

### Rules:  
- **First 5 characters** → Alphabets (A–Z)  
  - Adjacent characters cannot be the same  
    - ❌ `AABCD`, ✅ `AXBCD`  
  - All 5 cannot form a sequence  
    - ❌ `ABCDE`, ✅ `ABCDX`  

- **Next 4 characters** → Digits (0–9)  
  - Adjacent digits cannot be the same  
    - ❌ `1123`, ✅ `1923`  
  - All 4 cannot form a sequence  
    - ❌ `1234`, ✅ `1246`  

- **Last character** → Alphabet (A–Z)  

📌 **Example of a valid PAN:**  
