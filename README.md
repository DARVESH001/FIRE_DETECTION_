

# Fire Detection System Documentation

## Table of Contents

1. **Introduction**
    1.1. Purpose
    1.2. Scope
    1.3. Prerequisites

2. **Project Overview**
    2.1. Description
    2.2. Features
    2.3. Components

3. **Installation**
    3.1. Required Libraries
    3.2. Configuration
    3.3. Setting Up Telegram Bot

4. **Usage**
    4.1. Running the System
    4.2. Fire Detection
    4.3. Alarm and Notification
    4.4. Stopping the System

5. **Troubleshooting**
    5.1. Common Issues
    5.2. Known Limitations

6. **Appendix**
    6.1. Credits
    6.2. Contact Information

---

## 1. Introduction

### 1.1. Purpose

The Fire Detection System is designed to detect fires using a camera feed, trigger an alarm, and send a notification with a captured photo to a Telegram bot. This documentation provides information on how to set up and use the system effectively.

### 1.2. Scope

This system can be used for various applications, including home fire detection, workplace safety, and more. It is an open-source project that can be customized and extended as needed.

### 1.3. Prerequisites

Before using the Fire Detection System, make sure you have the following:

- Python 3.x installed
- OpenCV (cv2) library
- playsound library
- smtplib library
- A Telegram bot token and chat ID for notifications
- Pre-trained cascade model for fire detection (provided as 'fire_detection_cascade_model.xml' in the code)

## 2. Project Overview

### 2.1. Description

The Fire Detection System captures video from a camera source, processes it to detect fires, triggers an alarm, and sends a notification with a photo to a specified Telegram chat.

### 2.2. Features

- Real-time fire detection using OpenCV
- Sound alarm when a fire is detected
- Telegram integration for instant notifications
- Photo capture when a fire is detected

### 2.3. Components

- `fire_detection_cascade_model.xml`: Pre-trained cascade model for fire detection.
- `fire_alarm.mp3`: Alarm sound played when a fire is detected.

## 3. Installation

### 3.1. Required Libraries

Install the required Python libraries using pip:

```bash
pip install opencv-python playsound requests
```

### 3.2. Configuration

Edit the following variables in your code with your own values:

- `token`: Your Telegram bot token.
- `chat_id`: The chat ID where notifications will be sent.

### 3.3. Setting Up Telegram Bot

To create a Telegram bot and obtain the token and chat ID, refer to the [Telegram BotFather documentation](https://core.telegram.org/bots#botfather).

## 4. Usage

### 4.1. Running the System

Run the provided Python script to start the fire detection system:

```bash
python fire_detection_system.py
```

### 4.2. Fire Detection

The system processes the camera feed and detects fires using the cascade model.

### 4.3. Alarm and Notification

When a fire is detected, an alarm sound is played, a photo is captured, and a notification is sent to your Telegram chat.

### 4.4. Stopping the System

To stop the system, press 'q' in the command line where the script is running.

## 5. Troubleshooting

### 5.1. Common Issues

- Ensure that the required libraries are installed.
- Check your Telegram bot configuration for correct token and chat ID.
- Make sure your camera is working and accessible.

### 5.2. Known Limitations

- The system may have false positives or miss small fires based on the cascade model's sensitivity.

## 6. Appendix

### 6.1. Credits

- [OpenCV](https://opencv.org/): Computer vision library.
- [Telegram Bot API](https://core.telegram.org/bots/api): API for Telegram bot integration.

### 6.2. Contact Information

For questions or support, contact DARVESH BANSAL at darvesh.bansal@msds.christuniversity.in

---

Feel free to customize and expand this documentation to meet your specific project needs. Include any additional information or instructions that you think would be helpful for users or contributors to your project.

here are some telegram screenshot:
![image](https://github.com/DARVESH001/FIRE_DETECTION_/assets/104376273/ce6a2089-50e1-473b-8362-6d425e7b70e8)
