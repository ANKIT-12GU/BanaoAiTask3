# **Procrastination Preventer**

**📌 A system to monitor and improve productivity by detecting non-work-related activities using OCR and AI-based classification.**  
🚀 **Monitors browser activity, logs productivity, and notifies users when they get distracted.**  

---

## **📂 Repository Structure (Work Tree)**  
```
📦 BanaoAiTask3
├── 📂 .ipynb_checkpoints/          # Jupyter notebook checkpoints
├── 📂 ScreenShots/                 # Captured screenshots of active tabs
├── 📜 BanaoAiTask3.tar.gz          # Compressed project archive
├── 📜 Procrastination Preventer Pdf Report.pdf  # Detailed project report
├── 📜 Procrastination Preventer.ipynb  # Jupyter Notebook implementation
├── 📜 requirements.txt                    # library to install
├── 📜 README.md                    # Project documentation
├── 📜 Task-3 banao Ai.pdf           # Task document
├── 📜 expected_activities.json      # User's intended activities
├── 📜 logs.json                     # Activity logs for productivity tracking
```

---

## **📌 Features**
✅ **Monitors user activity** based on browser screenshots  
✅ **Extracts text using OCR** and analyzes content  
✅ **Classifies activities as "Work-related" or "Not work-related"**  
✅ **Sends notifications only when distractions are detected**  
✅ **Logs user activity for productivity analysis**  
✅ **Saves productivity insights in a visual graph (Matplotlib)**  

---

## **🔧 Installation & Setup**

### **Step 1️⃣: Clone the repository**  
```bash
[git clone https://github.com/ANKIT-12GU/BanaoAiTask3.git]
cd BanaoAiTask3
```

### **Step 2️⃣: Install dependencies**  
```bash
pip install -r requirements.txt
```

### **Step 3️⃣: Ensure Tesseract OCR is installed**  
- Download & install **Tesseract OCR** from: [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)  
- Update `pytesseract.pytesseract.tesseract_cmd` in the script with the correct path.

---

## **🚀 Usage Instructions**

### **Step 4️⃣: Run the monitoring script**  
```bash
python Procrastination_Preventer.py
```
- The system will **capture screenshots, analyze text, and classify activities**.
- **If a distraction is detected, a notification will be sent**.
- **Logs are saved in `logs.json` and can be analyzed later**.

---

## **📊 Step 5️⃣: Productivity Analysis**
To analyze logs and generate a productivity report, run:
```bash
python -c "import Procrastination_Preventer; Procrastination_Preventer.analyze_logs()"
```
- The system reads log data to **determine work vs. non-work trends**.
- A **bar chart** is generated showing time spent on work vs. distractions.
- The productivity graph is saved as an image (`productivity_analysis.png`).

---

## **📜 Step 6️⃣: Privacy & Security**
✔ **All processing is done locally** (no external API calls).  
✔ **Users can delete logs anytime** by running:  
```bash
python -c "import Procrastination_Preventer; Procrastination_Preventer.delete_logs()"
```
- This ensures **privacy and control** over logged activity data.

---

## **🛠 Step 7️⃣: Testing & Validation**
- Verified that **notifications are only sent for distractions**.
- The **accuracy of text extraction and classification** was tested under different scenarios.
- Debugging logs were added to track processing steps and classification results.
- ![image](https://github.com/user-attachments/assets/b85b5e03-4849-4295-bfbd-5e275883975a)

---  


