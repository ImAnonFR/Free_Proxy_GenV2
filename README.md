# Free Proxy Gen V2

A lightweight script to generate a `proxy.txt` file containing fresh and working proxies. Supported types: **HTTP**, **Socks4**, **Socks5**.

---

## 🚀 Installation

1. **Install Python (>= 3.10)** and `pip`.

2. **Clone this repository** and navigate to the project folder:
   ```bash
   git clone https://github.com/ImAnonFR/Free_Proxy_GenV2
   cd Free_Proxy_GenV2
   ```

3. **Install the required dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

---

## ⚙️ Configuration

You can customize the following settings in the **`free_proxy_gen.py`** file:
- **Proxy verification URL**: Edit line **103** to change the default URL (`https://api.ipify.org`).
- **Timeout for proxy checks**: Edit line **102** to adjust the default timeout (`15` seconds).
- **Urls to fetch proxies**: You can add or remove proxies source in config.json

---

## 🛠 Usage

### Default Arguments
- `--proxy-file`: Output file for the proxy list (default: `proxy.txt`).
- `--num-threads`: Number of threads for processing (default: `500`).
- `--type-proxy`: Proxy type to fetch: (default : `1`)
  - `0` = All (HTTP, Socks4, Socks5)
  - `1` = HTTP only
  - `4` = Socks4 only
  - `5` = Socks5 only

### Run Without Arguments
To run the script with default settings:
```bash
python free_proxy_gen.py
```

### Run With Custom Arguments
To specify custom parameters:
```bash
python free_proxy_gen.py --proxy-file socks5.txt --num-threads 200 --type-proxy 5
```

---

## ✨ Features

- Fetches fresh and working proxies.
- Supports multiple proxy types: **HTTP**, **Socks4**, **Socks5**.
- Highly configurable with thread support for fast performance.
