
This guide covers both **Windows** and **Linux** setups for running models like **TinyLlama** and **Mistral** using **Ollama**.

---

## 🪟 1. Windows Setup (Easiest for Beginners)

### Step 1 – Download Ollama
1. Go to 👉 [https://ollama.com/download](https://ollama.com/download)  
2. Download the **Windows installer**.  
3. Install it (just like a normal app).

### Step 2 – Open Terminal
- Open **PowerShell** or **Command Prompt**.  
- Type:  
```powershell
ollama
```
If you see Ollama’s help menu → ✅ it’s installed.

### Step 3 – Run Models
Pull & run **TinyLlama**:
```powershell
ollama run tinyllama
```

Pull & run **Mistral**:
```powershell
ollama run mistral
```

👉 First run will **download the model** (hundreds of MB to a few GB depending on model). After that, it’s instant.

---

## 🐧 2. Linux Setup (More Efficient for AI Work)

### Step 1 – Update System
Open terminal:
```bash
sudo apt update && sudo apt upgrade -y
```

### Step 2 – Install Ollama
Run the official install script:
```bash
curl -fsSL https://ollama.com/install.sh | sh
```

### Step 3 – Verify
Check Ollama is installed:
```bash
ollama
```

### Step 4 – Run Models
Run **TinyLlama**:
```bash
ollama run tinyllama
```

Run **Mistral**:
```bash
ollama run mistral
```

---

## ⚡ Optional: Web UI for Easier Use
If you prefer a **chat interface in your browser** (instead of terminal), install:

```bash
git clone https://github.com/ollama-webui/ollama-webui.git
cd ollama-webui
./start.sh   # Linux
```
On Windows you’d run the included `.bat` file.

---

## ✅ Recommendations for i5 + 12GB RAM
- Try **TinyLlama** first → lightweight, fast, great for testing.  
- Then try **Mistral 7B** → heavier but smarter (may be slower on CPU).  
- For lighter use, consider **quantized models** (4-bit) to save memory.  
