# 📌 E-Commerce Targeting System

![Flask](https://img.shields.io/badge/Flask-1.1.2-blue.svg) ![Python](https://img.shields.io/badge/Python-3.8%2B-brightgreen.svg) ![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)

A Flask-based web application for **customer segmentation** and **personalized product recommendations** based on user interactions.

---

## 🚀 Features
- ✅ **User Segmentation** - Categorizes users based on browsing and purchase behavior.
- ✅ **Product Recommendations** - Suggests relevant products using a Nearest Neighbors model.
- ✅ **CSV Upload Support** - Allows uploading structured data for analysis.
- ✅ **Interactive Web Interface** - Built with Flask and Bootstrap for ease of use.

---

## 📁 Project Structure
```bash
📦 e-commerce-targeting
├── 📂 app
│   ├── __init__.py       # Flask app initialization
│   ├── routes.py         # API routes for segmentation & recommendation
│   ├── recommendation.py # Product recommendation engine
│   ├── segmentation.py   # User segmentation logic
│   ├── 📂 templates      # HTML templates for UI
│   │   ├── base.html
│   │   ├── upload.html
│   │   ├── recommendation_input.html
│   │   ├── recommendation_results.html
│   │   ├── segmentation_results.html
├── 📂 uploads             # Stores uploaded CSV files
├── run.py                # Application entry point
├── requirements.txt      # Dependencies list
├── README.md             # Project documentation
```

---

## ⚙️ Installation & Setup
### 🛠 Prerequisites
Ensure you have the following installed:
- **Python 3.8+**
- **pip** (Python package manager)
- **Git** (for cloning the repository)

### 🔧 Setup Instructions

#### **Create and Activate a Virtual Environment**
Create and activate a virtual environment to isolate project dependencies.

**On Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

**On macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

#### **Install Dependencies**  
Install the required Python libraries from the `requirements.txt` file:
```bash
pip install -r requirements.txt
```

#### **Set Flask Environment Variables**  
Set the necessary environment variables to run the Flask app.

**On Windows:**
```bash
set FLASK_APP=run.py
set FLASK_ENV=development
```

**On macOS/Linux:**
```bash
export FLASK_APP=run.py
export FLASK_ENV=development
```

#### **Run the Application**  
Start the Flask development server:
```bash
flask run
```

🔗 Open `http://127.0.0.1:5000/` in your browser.

#### **Interact with the Application**
- Open your browser and navigate to [http://127.0.0.1:5000](http://127.0.0.1:5000).  
- Follow these steps in the application:
  - Select a segmentation type.
  - Upload your dataset.
  - Match required and additional columns.
  - Review the selected columns.
  - Run the segmentation process and view results.

#### **Optional: Debug Mode**
To limit dataset rows during debugging:
- Open `config.py`.
- Set `DEBUG_MODE = True`.

#### **Deactivate the Virtual Environment**
When you're done, deactivate the virtual environment:
```bash
deactivate
```

---

## 📊 Usage
### **1️⃣ Upload Data**
- Navigate to `Upload Recommendation Data` or `Upload Segmentation Data`.
- Upload a CSV file with the required fields.

### **2️⃣ Get Product Recommendations**
- Go to `Get Recommendations`.
- Enter a visitor ID to receive personalized product suggestions.

### **3️⃣ View Segmentation Insights**
- Check user segmentation distribution and recommended actions.

---

## 📄 Required CSV Formats
### **📌 Recommendation Data Format**
```csv
visitorid,itemid,event
12345,6789,view
54321,1234,transaction
```
### **📌 Segmentation Data Format**
```csv
visitorid,total_views,total_addtocart,total_purchases
12345,10,2,1
54321,5,1,0
```

---

## 📚 Technologies Used
```bash
# Python Libraries Used
pip list | grep -E 'flask|pandas|numpy|scikit-learn|matplotlib|seaborn|scipy'
```

---

## 📦 Dependencies
Below are the required dependencies for this project as listed in `requirements.txt`:
```txt
flask
pandas
numpy
scikit-learn
matplotlib
seaborn
scipy
```

---

## 🛠 Troubleshooting
- **Dependencies Not Installing:** Ensure you are using the correct version of Python and pip.
- **Server Not Starting:** Verify that `FLASK_APP` is set to `run.py`.
- **File Upload Issues:** Ensure your dataset file is in CSV format.

```bash
# 🔹 Dependencies Not Installing
python --version
pip --version
pip install --upgrade pip

# 🔹 Server Not Starting
echo $FLASK_APP

# 🔹 File Upload Issues
file uploads/sample.csv
```

---

## 🤝 Contributing
Pull requests are welcome! For major changes, open an issue first to discuss what you’d like to change.

1. **Fork the repository**
2. **Create a new branch** (`git checkout -b feature-branch`)
3. **Commit your changes** (`git commit -m "Added new feature"`)
4. **Push to the branch** (`git push origin feature-branch`)
5. **Create a pull request**

---

## 📜 License
This project is licensed under the **MIT License**.

---

🌟 **If you found this project helpful, please ⭐ the repository!**

