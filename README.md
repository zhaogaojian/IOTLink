# IOTLink Product Overview

<img width="1181" height="634" alt="图片" src="https://github.com/user-attachments/assets/c95c951a-3bb7-4b73-b1aa-a2ddfa7182cc" />


IOTLink is a local desktop workbench for IoT, edge-device, and field operations debugging. It brings MQTT message testing, SSH remote terminals, SFTP file transfer, UART serial debugging, Modbus tools, HEX inspection, VNC remote desktop, and AI-assisted analysis into one workspace. It is designed for engineers, testers, delivery teams, and operations users who need to troubleshoot an end-to-end device-to-cloud chain.

The product is not intended to replace one specific tool. Its value is in reducing context switching across many single-purpose tools during field debugging. Within one scheme, users can preserve publish topic trees, subscriptions, connection sessions, quick commands, macros, and workspace layout, turning a troubleshooting process into reusable project knowledge.

## Positioning

IOTLink is useful when device-side, edge-side, and cloud message-side signals must be inspected together. A typical issue may involve device boot logs over UART, a Linux service checked through SSH, cloud messages observed through MQTT, and payloads that need to be decoded as HEX, JSON, Modbus, or another custom format. IOTLink keeps these work surfaces inside one evolving local client.

Current version: `v1.0.5.7`.

## Core Capabilities

<img width="1121" height="535" alt="图片" src="https://github.com/user-attachments/assets/ac9cac57-3d14-4033-90a4-6ab301feb17f" />


**MQTT Debugging**  
Manage multiple Broker profiles, publish and subscribe to topics, filter messages, inspect payloads, export data, run JavaScript preprocessing before publish, and build stream conversion rules for protocol validation and lightweight message routing experiments.

**SSH / SFTP Remote Work**  
Use interactive SSH terminals, SFTP file browsing and transfer, multi-tab connections, quick commands, and SSH macros. Remote commands, file operations, and session logs can be organized around the same workspace for parallel host troubleshooting.

**Serial and Modbus Debugging**  
The serial panel supports UART logs, console interaction, and send-window workflows. The Modbus tool provides dedicated protocol debugging. Selected log text can be decoded through context menus or sent to AI for assisted analysis.

**HEX and "Decode As"**  
Binary payloads, serial data, and log fragments can be inspected and decoded through a unified entry point. The context-menu "Decode As" flow helps interpret selected content without copying it into external tools.

**AI Chat Assistance**  
The AI chat window uses a light blue-accented style and can receive selected text from MQTT, serial, SSH Term, and related views. It is intended for log explanation, configuration review, script drafting, SSH macro suggestions, and protocol-fragment analysis. AI output is never executed automatically; users remain in control of all actions.

**Schemes and Session Reuse**  
Scheme folders and session recovery preserve structured debugging state. Teams can reuse common topic trees, subscriptions, quick commands, macros, and workspace layouts as project assets.

## Typical Workflow

![IOTLink debugging workflow](assets/debug-workflow-en.svg)

1. **Connect to the field**: connect to an MQTT Broker, SSH host, serial device, or VNC desktop.
2. **Observe data**: inspect subscribed messages, terminal output, serial logs, and file transfer results.
3. **Decode payloads**: run "Decode As" on payloads, logs, Modbus data, or HEX fragments.
4. **Use AI assistance**: send key fragments to AI for log analysis, script suggestions, or troubleshooting steps.
5. **Preserve and reuse**: save connections, schemes, quick commands, and macros as reusable field-debugging templates.

## Use Cases

- MQTT protocol testing, serial boot-log inspection, and binary payload validation during device development.
- SSH-based remote inspection, log troubleshooting, and file transfer for edge gateways, Linux devices, or servers.
- Field delivery scenarios with weak networks, offline environments, or serial-console-only access.
- Cross-chain issues that require observing device-side, edge-side, and cloud-message-side behavior together.
- Projects that need to turn one troubleshooting session into reusable schemes, macros, and team configuration.

## Product Value

- **Less tool switching**: MQTT, SSH, serial, HEX, Modbus, VNC, and AI assistance work in one workspace.
- **Shorter troubleshooting path**: move from log observation to payload decoding, script suggestions, and scheme reuse in one flow.
- **Lower operational risk**: AI output is not auto-executed; decode menus are placed at the bottom of context menus; high-risk commands and macros can be paired with confirmation flows.
- **Reusable team knowledge**: scheme folders, session recovery, quick commands, and macros make debugging experience portable.
- **Local-first usage**: as a desktop client, it remains practical in offline, weak-network, and restricted field environments.

## Version Highlights

`v1.0.5.7` focuses on AI-assisted workflows and context-menu decoding:

- AI chat now uses a Codex-like light theme with blue accents.
- Selected text from MQTT, serial, and SSH Term views can be sent to AI from context menus.
- Modbus logs now support "Decode As" and reuse the MQTT-style decoding flow.
- "Decode As" menus are consistently placed at the bottom of context menus to reduce accidental submenu popups.
- Odd-length pure-HEX selections no longer show a blocking "must be even bytes" warning; they are handled as plain text.
- The send-window page has been restyled to better match the receive view, with blue-tinted borders.

## Boundaries

IOTLink is a local debugging and operations-assistance tool. It does not replace an MQTT Broker, SSH server, device firmware, production monitoring platform, or formal release system. For high-risk operations such as deletion, overwrite, restart, and batch execution, users should follow the actual field permissions, backup strategy, and manual confirmation process.# IOTLink Product Overview
