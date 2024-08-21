# Software for Blum telegram Bot

## 必要条件
- Python 3.11 (安装python [here](https://www.python.org/downloads/release/python-3110/))
- Telegram API_ID and API_HASH (you can get them [here](https://my.telegram.org/auth?to=apps))



1. 安装依赖:
   ```bash
   pip install -r requirements.txt
   ```

2. 获取 API_ID and API_HASH:
   - Go to [my.telegram.org](https://my.telegram.org/auth?to=apps)
   - Sign in with your Telegram account
   - Create a new application to get your API_ID and API_HASH

3. 配置:
   - 打开 `config.py` 添加你的 `API_ID` and `API_HASH`:
     ```python
     API_ID = 你的 api_id
     API_HASH = '你的api_hash'
     ```

   - 如果使用代理, 设置   `config.py` 里的 `USE_PROXY` 为 `True`, 否则 `False`:
     ```python
     USE_PROXY = True  # or False
     ```

   - 如果 `USE_PROXY` 为 `True`, 打开 `proxy.txt` ， session1 为会话名称，自定义
   ```txt
   192.168.1.1:1234:username:password session1
   192.168.1.2:2934:username:password session2
   192.168.1.3:3834:username:password session3
   192.168.5.1:2884:username:password session4
   ```
   `config.py`的 `PROXY_TYPE`这只为`socks5`
   ```python
   PROXY_TYPE = "socks5" # or http
   ```



## Usage

 Run the bot:
   ```bash
   python main.py
   ```


