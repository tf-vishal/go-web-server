# 🌐 Go Web Server

A beginner-friendly HTTP web server written in **Go**, designed to serve static files, handle simple GET and POST requests, and act as a foundation for learning how servers work in GoLang.

---

## 📁 Project Structure

```
.
├── main.go               # The main Go server
└── static                # Static files served at root "/"
    ├── form.html
    └── index.html
```

---

## 🚀 Features

- ✅ Serves static HTML files from the `static` folder  
- ✅ Handles `GET` requests at `/hello`  
- ✅ Handles `POST` requests at `/form` and returns submitted form data  
- ✅ Clean routing with built-in Go `net/http` package  

---

## 📦 Requirements

- Go (1.20 or newer)

To check your Go version:
```bash
go version
```

---

## 🛠️ Getting Started

### 1️⃣ Clone the repository

```bash
git clone git@github.com:tf-vishal/go-web-server.git
cd go-web-server
```

> If you're cloning via HTTPS:
```bash
git clone https://github.com/tf-vishal/go-web-server.git
```

---

### 2️⃣ Run the server

```bash
go run main.go
```

The server will start on:

```
http://localhost:8080
```

---

## 🌐 Available Routes

| Route    | Method | Description                                               |
|----------|--------|-----------------------------------------------------------|
| `/`      | GET    | Serves `index.html` or `form.html` from the static folder |
| `/hello` | GET    | Returns a plain `hello!` string                           |
| `/form`  | POST   | Accepts form data `name` and `address`, and returns them  |

[image](./image/image.png)

---

## 🧪 Example Test

### Using `curl` to test POST `/form`

```bash
curl -X POST -d "name=Vishal&address=Delhi" http://localhost:8080/form
```

**Output:**
```
POST request Successful
Name = Vishal
Address = Delhi
```

---

## 🤯 What You'll Learn

- Setting up a basic HTTP server in Go  
- Routing with `http.HandleFunc`  
- Serving static files with `http.FileServer`  
- Parsing form data using `r.ParseForm()` and `r.FormValue()`  

This is a great starting point for backend web development using Go.

---

## 👨‍💻 Author

**Vishal Sharma**  
DevOps & Cloud Enthusiast | CCNA Certified  
GitHub: [@tf-vishal](https://github.com/tf-vishal)

---

## 🌟 Show Some Love

If this helped you learn or start your journey with Go — drop a ⭐️ on the repo and share it with your fellow learners. Contributions and feedback are always welcome!

---
