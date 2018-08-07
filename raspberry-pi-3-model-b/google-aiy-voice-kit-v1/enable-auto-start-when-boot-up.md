# Enable Auto Start when Boot Up

{% embed data="{\"url\":\"https://aiyprojects.withgoogle.com/voice-v1/\#assembly-guide-1-get-the-voice-kit-sd-image\",\"type\":\"link\",\"title\":\"Voice V1\",\"description\":\"Build your own natural language recognizer and connect it to the Google Assistant\",\"icon\":{\"type\":\"icon\",\"url\":\"https://aiyprojects.withgoogle.com/static/images/favicon-32x32.png\",\"width\":32,\"height\":32,\"aspectRatio\":1},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://aiyprojects.withgoogle.com/static/images/voice-v1/box-and-shadow.png\",\"width\":500,\"height\":335,\"aspectRatio\":0.67}}" %}

{% hint style="info" %}
Follow the instructions from section 3.4
{% endhint %}

### 1. Copy one of the demo script under "src" folder and name it as my\_assistant.py

### 2. Create my\_assistant.service file

```text
[Unit]
Description=My awesome assistant app

[Service]
Environment=XDG_RUNTIME_DIR=/run/user/1000
ExecStart=/bin/bash -c 'python3 -u src/my_assistant.py'
WorkingDirectory=/home/pi/AIY-projects-python
Restart=always
User=pi

[Install]
WantedBy=multi-user.target

```

### 3. Copy it to "/lib/systemd/system" folder

```text
sudo mv my_assistant.service /lib/systemd/system/
```

### 4. Enable your service

```text
sudo systemctl enable my_assistant.service
```

### 5. To start/stop your service manually

```text
# Start your service
sudo service my_assistant start
# Stop your service
sudo service my_assistant stop
# Check status
sudo service my_assistant status
```

