# CAVA Android Visualizer

Install and start the **WiFi Audio Streaming** app on Android. Choose Send
(Server), enable Internal Audio and grant capture permission, select HTTP/Web,
and start streaming. Play audio on the phone. The widget contains its own small
bridge; it does not need separate helper files. In the settings screen, enter
the app's IP address and port (for example, `192.168.1.20:8080`) or its HTTP
URL. It saves when you leave settings with Back or Close. If there is no audio,
make sure Internal Audio is toggled on in the app settings. If latency is too
high, decrease it in the app.

The widget uses the declared Arch packages `python`, `cava`, and `ffmpeg` to
connect to `http://<IP>:<port>/stream`, decode audio and draw live spectrum bars.
The launcher offers to install any missing packages.
