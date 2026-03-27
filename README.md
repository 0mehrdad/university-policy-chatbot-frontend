# 📚 University Policy Assistant (Frontend)

This is a simple **Streamlit-based frontend** for a university policy chatbot.
It connects to a backend API hosted on AWS and allows users to ask questions in a chat interface.

---

## 🚀 Features

* Chat-style interface using Streamlit
* Sends user questions to a backend API
* Displays answers with optional sources
* Maintains conversation history

---

## 🛠️ Tech Stack

* Python
* Streamlit
* Requests

---

## ⚙️ Setup & Run Locally

1. Clone the repository:

```bash
git clone <your-repo-url>
cd <your-repo-folder>
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Set the API URL:

```bash
export API_URL="http://University-chat-bot-env-1.eba-znhr7bta.us-east-1.elasticbeanstalk.com/ask"
```

(Windows PowerShell)

```powershell
$env:API_URL="http://University-chat-bot-env-1.eba-znhr7bta.us-east-1.elasticbeanstalk.com/ask"
```

4. Run the app:

```bash
streamlit run app.py
```

---

## 🌐 Deployment

This app can be deployed easily using **Streamlit Community Cloud** by linking the GitHub repository and setting the `API_URL` in app secrets.

---

## 📡 API Requirements

The backend API should expose a POST endpoint:

```
POST /ask
```

Request:

```json
{
  "question": "Your question here"
}
```

Response:

```json
{
  "answer": "Response text",
  "sources": ["optional", "list"]
}
```

---

## ⚠️ Notes

* Ensure the backend API is publicly accessible
* Use HTTPS if required by deployment platform
* Increase timeout if backend responses are slow

---

## 👤 Author

Your Name
