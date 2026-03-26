This Application is Completely Free
1. Overall Interface
<img width="1920" height="1215" alt="image" src="https://github.com/user-attachments/assets/f81b225f-614b-42ef-bc36-72856f237fab" />
Core Features
2. Publish Topics
<img width="970" height="1090" alt="image" src="https://github.com/user-attachments/assets/0aad9bcb-1fb3-4d5f-a0f6-1ffde67f4c39" />
Tree-structured topic grouping supports folders and topic nodes for easy management of large numbers of Topics.
Each topic can be configured with QoS, Retain, and encoding formats (e.g., UTF-8 text / Hex).
Multi-tab editing: Payload, Markdown notes, and pre-publish JavaScript preprocessing (dynamic payload rewriting).
Code editor with syntax highlighting, JSON formatting, and other features to improve editing efficiency.
Publish & Subscribe: Independently configurable filters for "auto-subscribe to Broker after successful publishing" per topic; publish-time filtering is synchronized with subscription-side message filtering to prevent accidental overwriting of user-defined conditions.
Supports opening/saving topic lists (JSON) for easy backup and sharing.
3. Subscribe Topics
<img width="955" height="1085" alt="image" src="https://github.com/user-attachments/assets/ab3aac72-31ab-4a1b-9cac-42690ddd3044" />
Multi-topic subscription list supporting + / # wildcards.
Real-time message table displaying timestamp, topic, QoS, and payload preview; supports detailed viewing and JSON formatting.
Multiple message filtering rules (topic / content / global × include or exclude), coordinated with publish-side filtering.
Supports common operations such as enabling/disabling subscription items and exporting data.
4. Stream Transformation
<img width="955" height="1095" alt="image" src="https://github.com/user-attachments/assets/141f111c-3e8d-48a0-b4f4-6437b7b79eb7" />
Multiple transformation rules: Listen to source topic → Transform via JS script → Publish to target topic.
Rules can be individually enabled/disabled, with runtime logs and basic statistics for easy script troubleshooting.
Provides a test area to verify script output before deployment.
5. Real-Time Dashboard
<img width="964" height="1095" alt="image" src="https://github.com/user-attachments/assets/6f082019-4333-4dc2-bec0-d2adf283bf14" />
Configurable multi-row, multi-column monitoring grid, with each cell independently subscribing to topics (wildcards supported).
Automatically parses JSON objects/arrays or multi-line "key=value" text, displaying key-value pairs in a table format—ideal for real-time monitoring of telemetry and status Topics.
Layout and grid configurations adapt to window resizing to fully utilize the docking area and minimize blank space.
6. Project Management
<img width="975" height="1090" alt="image" src="https://github.com/user-attachments/assets/815f6f78-4afc-40ee-8d8b-c90247f7dac9" />
7. System Scripts
<img width="950" height="1085" alt="image" src="https://github.com/user-attachments/assets/111e0561-c122-4dda-b910-55f857ac5982" />
8. Task Management
<img width="955" height="1084" alt="image" src="https://github.com/user-attachments/assets/580da077-f9a5-4179-ba5e-ac363deb0dad" />
Manages projects by directory, centrally storing publish trees, subscription statuses, stream rules, connection configurations, etc., for easy environment switching by project or site.
9. Interface & User Experience
All functions are housed in dockable, tabbed dock panels for side-by-side debugging on dual screens or large windows.
No blank central area in the main window; left and right workspaces maximize horizontal space utilization.
Toolbar for quick connections and multiple connection profiles, ideal for switching between multiple Brokers.
10. Application Scenarios
MQTT debugging, packet capture, and message verification for IoT devices and gateways.
Temporary subscription to production/test Brokers by operation and maintenance personnel for health checks.
Client-side lightweight topic mapping and field rewriting for demonstrations or forwarding.
Monitoring scenarios requiring simultaneous viewing of key-value statuses of multiple Topics on a single screen.
11. System & Dependency Notes
Designed for Windows desktops (minimum version subject to actual testing; Windows 10 or later recommended).
Built with Qt and Qt MQTT; release packages typically include required Qt runtime libraries (subject to actual packaging method).
Users must prepare an accessible MQTT Broker (e.g., Mosquitto, EMQX, etc.).
