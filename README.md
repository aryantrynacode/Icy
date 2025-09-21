# Icy
Prototype 
👓 Smart Assistive Glasses Prototype (Object Detection + Audio Alerts)

A wearable prototype that helps visually impaired users detect obstacles (wall, stairs, door, car, pole, step down, etc.) and receive real-time spoken feedback via earphones.

This project demonstrates how to combine computer vision, wearable hardware, and speech output into a low-power, portable system.

🚀 Features

Detects common obstacles and objects in front of the user.

Provides audio feedback like “Car approaching” or “Stairs ahead”.

Works in real time (camera → detection → speech).

Modular architecture:

Glasses: lightweight camera only.

Hub Device: runs object detection + TTS.

Earphone: plays audio alerts.

🧩 System Architecture
[Glasses (Camera)] → [Hub (AI + TTS)] → [Earphone (Audio)]


Glasses: ESP32-CAM / Pi Camera module, mounted on frame.

Hub: Raspberry Pi Zero 2 W (basic) or Jetson Nano (advanced).

Earphone: Wired or Bluetooth, connected to Hub for output.

🛠️ Materials Needed
👓 Glasses Module

Eyeglass frame (can be 3D printed or repurposed sunglasses).

Camera Module:

ESP32-CAM (Wi-Fi/Bluetooth, low power) or

Raspberry Pi Camera (if using Pi as hub).

Small LiPo battery (500–1000 mAh) for powering camera.

Mounting kit / adhesive to attach camera to glasses.

🎛️ Hub Device (Processing Unit)

Option 1 (Basic Prototype): Raspberry Pi Zero 2 W

Pros: Small, cheap, portable.

Runs YOLOv8n / MobileNet SSD for object detection.

Option 2 (Advanced Prototype): NVIDIA Jetson Nano / Orin Nano

Pros: Real-time inference, stronger AI.

Cons: Bulkier, higher power consumption.

MicroSD card (32 GB+).

Power bank or LiPo battery pack (2000–5000 mAh).

USB/HDMI cables for setup.

🎧 Audio Output

Wired earphones (3.5mm jack into hub)

OR Bluetooth earbud / bone-conduction headset

🔧 Optional Components

3D printed enclosure for hub (belt-worn or pocket-sized).

Cooling fan (for Jetson Nano).

Push button or voice wake word for activating detection.
