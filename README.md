# Enterprise Network Simulation｜企業網路模擬

這是「資訊網路」課程的 Cisco Packet Tracer 練習，模擬企業內部不同部門的網路架構，以及透過路由器連接另一端網路的情境。

This is a Cisco Packet Tracer lab project from my Computer Networks course. It models departmental networks, VLAN segmentation, IP addressing, and connections between two simulated network sites.

## 使用工具 | Tool

- Cisco Packet Tracer

## 專案內容 | Project Overview

- 規劃六個內部部門的 VLAN（10、20、30、40、50、60）。
  - Designed six VLANs (10, 20, 30, 40, 50, 60) for different internal departments.

- 使用 `192.168.10.0/24` 至 `192.168.60.0/24` 作為各部門的網段，預設閘道規劃為各網段的 `.254`。
  - Assigned subnets ranging from `192.168.10.0/24` to `192.168.60.0/24`, with `.254` configured as the default gateway for each subnet.

- 使用核心交換器連接各部門交換器、電腦、印表機及電話等模擬設備。
  - Used a core switch to connect departmental switches, computers, printers, and IP phones.

- 另一端模擬網路使用 VLAN 1、2，並透過路由器與內部網路連接。
  - Configured VLANs 1 and 2 for the second simulated network site, connected to the internal network through routers.

- 在資訊部網段配置模擬 Email Server，IP 為 `192.168.30.3`。
  - Configured a simulated email server in the IT department subnet with the IP address `192.168.30.3`.

- 練習子網路位址與廣播位址計算，例如 `192.168.21.0/24` 的廣播位址為 `192.168.21.255`。
  - Practiced subnet and broadcast address calculations. For example, the broadcast address of `192.168.21.0/24` is `192.168.21.255`.

- 課堂紀錄提到外部電腦可連至 Router5；其他服務的端到端連通性尚未在此文件逐項驗證。
  - According to the lab records, an external computer successfully connected to Router5. End-to-end connectivity for other services has not been individually verified in this documentation.

## Network Design | 網路設計

| VLAN | 部門 Department | 網段 Subnet |
|------|----------------|-------------|
| 10 | 總經理辦公室 / Management | 192.168.10.0/24 |
| 20 | 技術部 / Technical | 192.168.20.0/24 |
| 30 | 資訊部 / IT | 192.168.30.0/24 |
| 40 | 資安部 / Information Security | 192.168.40.0/24 |
| 50 | 人資部 / HR | 192.168.50.0/24 |
| 60 | 財務部 / Finance | 192.168.60.0/24 |

## How to Open | 開啟方式

1. 安裝 Cisco Packet Tracer。
   - Install Cisco Packet Tracer.

2. 下載本專案的 `資網練習.pkt`。
   - Download the `資網練習.pkt` file from this repository.

3. 使用 Packet Tracer 開啟檔案，查看網路拓樸與設備設定。
   - Open the file using Cisco Packet Tracer to explore the network topology and device configurations.

## Learning Outcomes | 練習重點

- VLAN 與部門網路分段
  - VLAN configuration and departmental network segmentation.

- IPv4 網段、子網路遮罩與預設閘道規劃
  - IPv4 subnet planning, subnet mask configuration, and default gateway assignment.

- Switch、Router 與終端設備的模擬配置
  - Simulated configuration of switches, routers, and end devices.

- Email Server 的模擬網路位置規劃
  - Planning the network placement of a simulated email server.
