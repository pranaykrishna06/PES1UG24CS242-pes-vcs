# PES Version Control System (Mini Git)

## 📌 Overview
This project is a simplified version of a Git-like version control system implemented in C.  
It supports basic features like storing objects, staging files, creating commits, and viewing history.

---

## ⚙️ Features Implemented

- Blob object storage (file content)
- Tree object creation (directory structure)
- Index (staging area)
- Commit creation and history tracking
- Log display

---

## 🧩 Phases

---

### 🔹 Phase 1: Object Storage

- Implemented blob storage using SHA-256 hashing
- Stored objects in `.pes/objects`

#### 📸 Screenshots

![Phase1-1](./screenshots/phase1_1.png)  
![Phase1-2](./screenshots/phase1_2.png)

---

### 🔹 Phase 2: Tree Objects

- Built directory structure from index
- Created tree objects linking blobs

#### 📸 Screenshots

![Phase2-1](./screenshots/phase2_1.png)  
![Phase2-2](./screenshots/phase2_2.png)

---

### 🔹 Phase 3: Index (Staging Area)

- Implemented add, load, and save operations
- Tracks file metadata and hashes

#### 📸 Screenshots

![Phase3-1](./screenshots/phase3_1.png)  
![Phase3-2](./screenshots/phase3_2.png)

---

### 🔹 Phase 4: Commit System

- Created commits with tree + parent linkage
- Updated HEAD pointer
- Implemented commit history (log)

#### 📸 Screenshots

![Phase4-1](./screenshots/phase4_1.png)  
![Phase4-2](./screenshots/phase4_2.png)  
![Phase4-3](./screenshots/phase4_3.png)

---

## 🧪 How to Run

```bash
make clean
make

./pes init
echo "hello" > file.txt
./pes add file.txt
./pes commit -m "first commit"
./pes log
