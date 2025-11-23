## 🛠️ Quick Lab Instructions — 2.2 Using the Command Line to Get Help

---

>💬 **Tip:** Paste this study guide into ChatGPT and ask for **more instructions** by specifying:  
>- “Provide step-by-step lab instructions for this objective.”  
>- “Include which Linux distro to use (Debian/Ubuntu or RHEL/Fedora).”  
>- “Show examples of installing, verifying, and managing desktop and server applications.”  
>- “Include minimal command-line practice for package management and development tools.”  
>- “Focus only on what is most important for passing the LPI Linux Essentials exam.”  

>This will prompt ChatGPT to give **practical, exam-focused lab steps** for each section.

---

### 1️⃣ Practice with Man Pages 📖
- Open a terminal and run basic man pages:
  - `man ls`
  - `man cp`
  - `man passwd`
- Move through pages using:
  - Up/Down arrows  
  - `/searchterm` to search  
  - `n` for next match  
  - `q` to quit
- Check a specific section:
  - `man 5 passwd` (file format)
  - `man 1 passwd` (command)

---

### 2️⃣ Explore Info Pages 📘
- Run:
  - `info ls`
  - `info coreutils`
- Practice navigation:
  - Arrow keys to move  
  - **Enter** to follow a link  
  - `u` to go up a menu  
  - `q` to exit

---

### 3️⃣ Browse /usr/share/doc/ 📂
- List documentation directories:
  - `ls /usr/share/doc/`
- Inspect package docs:
  - `ls /usr/share/doc/bash/`
  - View README or examples if present:
    - `less /usr/share/doc/bash/README*`
- Notice common files like **changelog**, **copyright**, **examples**

---

### 4️⃣ Use locate to Find Documentation 🔍
- Update the database (Debian/Ubuntu):  
  - `sudo updatedb`  
- Search for documentation or man pages:
  - `locate man | grep ls`
  - `locate README`
  - `locate /usr/share/doc | head`
- Note how locate is **fast** and returns **full paths**.

---

### ⚡ What to Observe
- Differences between **man** and **info** structure  
- How man sections change content  
- Which packages store documentation inside `/usr/share/doc/`  
- How `locate` helps find docs instantly  

### ⭐ Recommended Distros for Practice
- **Debian/Ubuntu** → great for man/info and rich `/usr/share/doc/` contents  
- **Fedora** → also excellent, strong man/info support  

Keep the labs light — your goal is to know **where to find help** and **how to navigate it quickly** for the exam.
