🎥 **Project Demo Video:** [Watch Here](https://drive.google.com/file/d/1PXzPtAc0W2GDCyjzFCgFXsJbLCpE04AM/view?usp=sharing)

# 💬 Simple Chatroom in Go

[![Go Version](https://img.shields.io/badge/Go-1.18%2B-00ADD8?style=flat&logo=go)](https://go.dev/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

A lightweight, real-time chatroom built with Go using the native `net/rpc` package. It demonstrates basic **client-server communication**, **concurrency**, and **RPC** in a simple terminal environment.

---

## ⚙️ Features

- 🧩 **Client–Server via RPC** – built using Go’s native `net/rpc`
- ⚡ **Real-time Messaging** – instant chat updates for all users
- 👥 **Multi-Client Support** – connect from multiple terminals
- 💾 **In-Memory Chat History** – maintained while the server runs
- 🔒 **Thread-Safe Access** – uses mutex locks to avoid race conditions
- 🧱 **Simple Terminal UI** – clear, minimal, and responsive

---

## 🏗️ Architecture

```
┌─────────────┐       RPC over HTTP       ┌─────────────┐
│   Clients   │◄─────────────────────────►│   Server    │
└─────────────┘                           └─────────────┘
```

- Clients send and receive messages via RPC
- Server stores chat history and broadcasts updates

---

## 🚀 Getting Started

### Prerequisites
- Go 1.18+ ([Download](https://go.dev/dl/))
- Terminal access

### Installation
```bash
git clone https://github.com/yourusername/go-chatroom.git
cd go-chatroom
go version
```

### Run the Server
```bash
go run server/main.go
```

### Run a Client
Open another terminal:
```bash
go run client/main.go
```
Enter your username and start chatting!

---

## 💬 Usage

- Type messages and press **Enter** to send
- Type `exit` to leave
- Run multiple clients in separate terminals to simulate users

**Example:**
```
[Alice]: Hello!
[Bob]: Hi Alice!
```

---

## 📂 Project Structure

```
chat-room/
├── server/main.go   # Server logic
└── client/main.go   # Client logic
```

---

## 🧠 Key Concepts

- **RPC Communication** over HTTP/TCP
- **Concurrent programming** using `sync.Mutex`
- **Network Programming** fundamentals
- **Terminal-based UI**

---

## 🔧 Troubleshooting

- Server not starting → check port 1234 availability
- Client not connecting → ensure server is running
- Use separate terminals for each client

---

## 🚧 Future Improvements

- [ ] Persistent message storage
- [ ] User authentication
- [ ] Web-based interface
- [ ] Private chats & timestamps

---

## 🤝 Contributing

1. Fork the repo
2. Create a branch
3. Commit and push changes
4. Open a Pull Request

---

## 📝 License

MIT License – see [LICENSE](LICENSE)

---

**⭐ Star this repo if you found it useful!**

