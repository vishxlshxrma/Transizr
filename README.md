# **Transizr ⚡🎙️**

### **AI-powered Media Transcription Platform — Fast, Scalable & Real-Time**

Transizr is a modern, distributed transcription system designed to convert audio & video files into accurate text transcripts — powered by containerized workers, message queues, and real-time updates.

Whether you're processing a single file or hundreds in parallel, Transizr ensures fast, scalable, and reliable performance.

---

## 🚀 **Features**

### 🎧 Media Transcription

Convert audio/video files into clean, accurate text with automated pipelines.

### ⚡ Highly Scalable Architecture

Distributed task execution with Celery & RabbitMQ — ideal for high-volume workloads.

### 🔔 Real-Time Notifications

Redis Pub-Sub + Server-Sent Events (SSE) deliver instant status updates.

### 🧩 Modular & Extensible

Dedicated services for API, transcription workers, optimization, and frontend UI.

---

## 🏗️ **Architecture Overview**

1. **User Uploads File** via the FastAPI backend.
2. **Media Optimization** improves processing speed.
3. **RabbitMQ** queues transcription tasks for parallel execution.
4. **Celery Workers** process tasks asynchronously in isolated containers.
5. **Real-Time Updates** via Redis Pub-Sub + SSE notify the frontend instantly.

This architecture ensures **speed**, **parallelism**, and **fault tolerance**.

---

## 🛠️ **Getting Started**

### **1️⃣ Clone the Repository**

```bash
git clone https://github.com/vishxlshxrma/Transizr.git
cd Transizr
```

---

### **2️⃣ Make Scripts Executable**

```bash
chmod +x scripts/check-requirements.sh
chmod -R +x scripts
```

---

### **3️⃣ Check Requirements**

```bash
sh scripts/check-requirements.sh
```

Or using Makefile:

```bash
make check-requirements
```

---

### **4️⃣ Build & Run the Application**

```bash
sh scripts/run.sh
```

Or using Makefile:

```bash
make run
```

Access the app at:

👉 **[http://localhost:3000](http://localhost:3000)**

---

## 🧹 **Stop & Clean Containers**

```bash
docker-compose -f docker-compose.yml down --remove-orphans
```

Or using:

```bash
make clean
```

---

## 🤝 **Contributing**

Contributions are welcome!
Open an issue or submit a pull request to help improve Transizr.

---

## 📄 **License**

This project is licensed under the **MIT License**.
See the `LICENSE` file for details.