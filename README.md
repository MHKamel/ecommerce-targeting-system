# 📌 E-Commerce Targeting System

![Flask](https://img.shields.io/badge/Flask-1.1.2-blue.svg) ![Python](https://img.shields.io/badge/Python-3.8%2B-brightgreen.svg) ![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)

A Flask-based e-commerce targeting system for customer segmentation and personalized product recommendations. Upload structured interaction data, receive AI-driven suggestions, and analyze user behavior.

---

## ⚙️ Installation & Setup
### 🛠 Prerequisites
Ensure you have the following installed:
- **Python 3.8+**
- **pip** (Python package manager)
- **Git** (for cloning the repository)

### 🔧 Setup Instructions

#### Create and Activate a Virtual Environment
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

#### Install Dependencies
```bash
pip install -r requirements.txt
```

#### Set Flask Environment Variables
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

#### Run the Application
```bash
flask run
```

🔗 Open [http://127.0.0.1:5000](http://127.0.0.1:5000) in your browser.

#### Interact with the Application
- Upload your dataset.
- Match required and additional columns.
- Run the segmentation or recommendation.
- View results.

#### Optional: Debug Mode
- Open `config.py`.
- Set `DEBUG_MODE = True`.

#### Deactivate the Virtual Environment
```bash
deactivate
```

---

## 📄 Required CSV Formats
### Recommendation Data Format
```csv
visitorid,itemid,event
12345,6789,view
54321,1234,transaction
```
### Segmentation Data Format
```csv
visitorid,total_views,total_addtocart,total_purchases
12345,10,2,1
54321,5,1,0
```

---

## 📦 Dependencies
Listed in `requirements.txt`:
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

## 📚 Technologies Used
```bash
pip list | grep -E 'flask|pandas|numpy|scikit-learn|matplotlib|seaborn|scipy'
```

---

## 🛠 Troubleshooting
- **Dependencies Not Installing:** Ensure correct versions of Python and pip.
- **Server Not Starting:** Verify `FLASK_APP` is set to `run.py`.
- **File Upload Issues:** Ensure the dataset is in CSV format.

```bash
# Check Python and pip versions
python --version
pip --version
pip install --upgrade pip

# Check Flask app variable
echo $FLASK_APP

# Check file type
file uploads/sample.csv
```

---

## 🤝 Contributing
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

