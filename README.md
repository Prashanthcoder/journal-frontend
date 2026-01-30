# Motivation Quotes – Frontend

## What the project does

This project is a simple frontend web application that allows users to add and view motivational quotes. It communicates with a remote backend API to store quotes and retrieve all saved quotes.

The application:

* Lets users submit a text quote through a form
* Sends the quote to a backend using a JSON POST request
* Fetches and displays all stored quotes from the backend
* Updates the quote list dynamically without page reload

This project focuses on **frontend logic and API interaction** using plain JavaScript.

---

## Why this project is useful

* Demonstrates CRUD-style interaction with a backend API
* Shows real-world usage of the Fetch API with GET and POST requests
* Helps beginners understand frontend–backend communication
* Can be used as a base for journal, notes, or quote-saving applications
* Suitable for mini-projects and learning REST APIs

---

## Project structure

```
.
├── index.html     # Frontend HTML and JavaScript
├── styles.css     # UI styling
├── README.md
```

---

## Tech Stack

* HTML5
* CSS3
* Vanilla JavaScript

---

## How to get started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/motivation-quotes-frontend.git
cd motivation-quotes-frontend
```

---

### 2. Run the frontend

No installation or build step is required.

You can either:

* Open `index.html` directly in your browser, or
* Serve it using a local server (recommended):

```bash
python -m http.server 8000
```

Then open:

```
http://localhost:8000
```

---

## Backend integration

The frontend connects to a deployed backend API:

```
https://journal-backend-vjrg.onrender.com
```

### Available endpoints used

* `GET /read_quote` – Fetch all saved quotes
* `POST /add_quote` – Add a new quote

---

## API usage examples

### Add a quote

```js
fetch(`${API_URL}/add_quote`, {
  method: "POST",
  headers: { "Content-Type": "application/json" },
  body: JSON.stringify({ quote: "Stay consistent" })
});
```

### Read quotes

```js
fetch(`${API_URL}/read_quote`);
```

---

## UI features

* Blurred background image effect
* Clean and centered layout
* Responsive quote list rendering
* Instant update after adding a quote

---

## Where to get help

* MDN Web Docs: [https://developer.mozilla.org/](https://developer.mozilla.org/)
* Fetch API documentation: [https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)

---

## Maintainer

Prashanth T

---

## Future improvements

* Delete and edit quotes
* Timestamp for each quote
* User authentication
* Search and filter functionality
* Improved mobile responsiveness
