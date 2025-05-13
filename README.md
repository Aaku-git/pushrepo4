# pushrepo4
Sure! Here's a step-by-step guide to **create a simple Flask application and push the code to GitHub**.

---

## ✅ Step 1: Create the Flask App Locally

### 📁 Folder structure:

```
flask-github-demo/
├── app.py
├── requirements.txt
├── README.md
```

---

### 📝 `app.py`

```python
from flask import Flask

app = Flask(__name__)

@app.route('/')
def home():
    return "Hello, GitHub from Flask!"

if __name__ == '__main__':
    app.run(debug=True)
```

---

### 📄 `requirements.txt`

```
Flask
```

---

### 📄 `README.md`

````markdown
# Flask GitHub Demo

This is a simple Flask application that displays a welcome message. Designed to demonstrate how to push code to GitHub.

## How to run

```bash
pip install -r requirements.txt
python app.py
````

Visit: [http://localhost:5000/](http://localhost:5000/)

````

---

## ✅ Step 2: Initialize Git Locally

Run the following commands in the `flask-github-demo` folder:

```bash
git init
git add .
git commit -m "Initial commit - Flask app"
````

---

## ✅ Step 3: Create a GitHub Repository

1. Go to: [https://github.com](https://github.com)
2. Click **New Repository**
3. Set repository name (e.g., `flask-github-demo`)
4. Do **not** initialize with README or .gitignore
5. Click **Create repository**

---

## ✅ Step 4: Push Code to GitHub

Follow the instructions GitHub gives after creating the repo, or do:

```bash
git remote add origin https://github.com/your-username/flask-github-demo.git
git branch -M main
git push -u origin main
```

Replace `your-username` with your actual GitHub username.

---

## ✅ Step 5: Done!

Now your Flask app is hosted on GitHub 🎉
You can share the repo link or clone it from anywhere.

---

## 🚀 Want to deploy it next?

Let me know if you want to:

* Deploy this app to **Heroku**, **Render**, or **Railway**
* Add Docker support
* Set up CI/CD with GitHub Actions

I can help with those next!
