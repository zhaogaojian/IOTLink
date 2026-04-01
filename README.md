首先这是个人作品，至于为啥叫山榕，因为是一种多根植物，和物联网很相似，该应用目前完全免费，支持中英文，如果感觉好用点颗星，谢谢。
First off, this is an original personal work. As for why it’s named Shanrong (Mountain Banyan), it’s a type of plant with an extensive root system, which carries a similar meaning to the Internet of Things.
This Application is Completely Free，Support Chinese and English，If you find it useful, please give it a star. Thank you.

# 一、All Page 
## 1. Overall Interface
<img width="1920" height="1215" alt="image" src="https://github.com/user-attachments/assets/8584e253-4b63-4f2f-a957-ce33f6693ee9" />


Core Features
## 2. Publish Topics
<img width="1920" height="1214" alt="image" src="https://github.com/user-attachments/assets/332d65c2-2817-4d84-b4ca-aaee0df3ffe5" />


Tree-structured topic grouping supports folders and topic nodes for easy management of large numbers of Topics.
Each topic can be configured with QoS, Retain, and encoding formats (e.g., UTF-8 text / Hex).
Multi-tab editing: Payload, Markdown notes, and pre-publish JavaScript preprocessing (dynamic payload rewriting).
Code editor with syntax highlighting, JSON formatting, and other features to improve editing efficiency.
Publish & Subscribe: Independently configurable filters for "auto-subscribe to Broker after successful publishing" per topic; publish-time filtering is synchronized with subscription-side message filtering to prevent accidental overwriting of user-defined conditions.
Supports opening/saving topic lists (JSON) for easy backup and sharing.
## 3. Subscribe Topics
<img width="1920" height="1201" alt="image" src="https://github.com/user-attachments/assets/483f6c2f-cf0a-480f-ac14-b83a06e1d82a" />


Multi-topic subscription list supporting + / # wildcards.
Real-time message table displaying timestamp, topic, QoS, and payload preview; supports detailed viewing and JSON formatting.
Multiple message filtering rules (topic / content / global × include or exclude), coordinated with publish-side filtering.
Supports common operations such as enabling/disabling subscription items and exporting data.
## 4. Stream Transformation
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/a8cd3035-4d74-4917-be46-4ff7f1aa9183" />

Multiple transformation rules: Listen to source topic → Transform via JS script → Publish to target topic.
Rules can be individually enabled/disabled, with runtime logs and basic statistics for easy script troubleshooting.
Provides a test area to verify script output before deployment.
## 5. Real-Time Dashboard
<img width="1920" height="1195" alt="image" src="https://github.com/user-attachments/assets/f52c2565-562b-4c25-ab66-768a598f750c" />

Configurable multi-row, multi-column monitoring grid, with each cell independently subscribing to topics (wildcards supported).
Automatically parses JSON objects/arrays or multi-line "key=value" text, displaying key-value pairs in a table format—ideal for real-time monitoring of telemetry and status Topics.
Layout and grid configurations adapt to window resizing to fully utilize the docking area and minimize blank space.
## 6. Project Management
<img width="1920" height="1206" alt="image" src="https://github.com/user-attachments/assets/20d42762-cde7-40a9-aca8-3d8c443a8c1e" />

## 7. System Scripts
<img width="1920" height="1214" alt="image" src="https://github.com/user-attachments/assets/0175ab8c-f0c8-4698-a327-82b7437a3527" />

## 8. Task Management
<img width="1920" height="1220" alt="image" src="https://github.com/user-attachments/assets/398899cd-b0f6-4a92-88fb-bc2b6afb356b" />

## 9. com debug
<img width="1920" height="1220" alt="image" src="https://github.com/user-attachments/assets/5572ae88-4ec6-49dc-bc4b-18789fe68b05" />

## 10. scheme sync
<img width="520" height="1006" alt="image" src="https://github.com/user-attachments/assets/7dece150-d9ec-4e5f-bf12-32bd578297b1" />

## 11. Batch Run
<img width="846" height="1085" alt="image" src="https://github.com/user-attachments/assets/22c7260e-bb3c-492c-ac5e-28435b44115d" />


## 12. clipbaord decode
<img width="639" height="515" alt="image" src="https://github.com/user-attachments/assets/db1351a7-0e72-4528-936a-bb93f5f64b4d" />

# 二、Additional
Manages projects by directory, centrally storing publish trees, subscription statuses, stream rules, connection configurations, etc., for easy environment switching by project or site.
## 1. Interface & User Experience
All functions are housed in dockable, tabbed dock panels for side-by-side debugging on dual screens or large windows.
No blank central area in the main window; left and right workspaces maximize horizontal space utilization.
Toolbar for quick connections and multiple connection profiles, ideal for switching between multiple Brokers.
## 2. Application Scenarios
MQTT debugging, packet capture, and message verification for IoT devices and gateways.
Temporary subscription to production/test Brokers by operation and maintenance personnel for health checks.
Client-side lightweight topic mapping and field rewriting for demonstrations or forwarding.
Monitoring scenarios requiring simultaneous viewing of key-value statuses of multiple Topics on a single screen.
## 3. System & Dependency Notes
Designed for Windows desktops (minimum version subject to actual testing; Windows 10 or later recommended).
Built with Qt and Paho; release packages typically include required Qt runtime libraries (subject to actual packaging method).
Users must prepare an accessible MQTT Broker (e.g., Mosquitto, EMQX, etc.).
