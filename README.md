# 🎧📽️ SwiftAssignment4 - Content Download System

This is my final Swift assignment project, built as a Playground in Xcode. It demonstrates the use of **protocols**, **classes**, and **composition** to simulate a content delivery system for music, videos, and PDF files. 

💡 The goal: Let customers choose content to download and get an estimated download time and total cost.

---

## 🚀 Features

- Uses **protocols** to define content and server behavior.
- Each `ContentServer` can only serve a **single content type** (music, video, or PDF).
- Each content file has:
  - ✅ A **name**
  - 📦 A **size in MB** (to calculate download time)
  - 💰 A **price**
- The system calculates:
  - ⏳ **Estimated download time** (based on size and server speed)
  - 🧾 **Total cost** for selected content

---

## 🛠 Technologies

- ✅ Swift 5
- ✅ Xcode Playground
- ✅ Git & GitHub for version control

---

## 📁 Structure

- `protocol Content` → Base for Music, Video, PDF
- `protocol ContentServer` → Each server handles a single content type
- `struct Music / Video / PDF` → Conform to `Content`
- `class Store` → Lets user choose content and fetches it from appropriate server

---

## 🧪 Sample Usage

```swift
store.downloadContent(
    music: ["Salsa"], 
    videos: ["Tutorial Swift"], 
    pdfs: ["Swift Guide"]
)
