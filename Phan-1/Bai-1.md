# 🌐 Bài 1: Tổng quan về Mạng máy tính

## 1. Mạng máy tính là gì?

**Mạng máy tính (Computer Network)** là tập hợp **từ 2 thiết bị trở lên** được kết nối với nhau để:

* Trao đổi dữ liệu
* Chia sẻ tài nguyên
* Liên lạc với nhau

### 3 thành phần cơ bản

| Thành phần          | Vai trò               | Ví dụ                          |
| ------------------- | --------------------- | ------------------------------ |
| **Thiết bị (Node)** | Gửi/nhận dữ liệu      | Laptop, điện thoại, server     |
| **Đường truyền**    | Nơi dữ liệu di chuyển | Cáp Ethernet, cáp quang, Wi-Fi |
| **Giao thức**       | Quy tắc giao tiếp     | TCP/IP, HTTP, Ethernet         |

> **Ghi nhớ:** Chỉ cần 2 thiết bị có thể kết nối và trao đổi dữ liệu với nhau thì đã có thể hình thành một mạng.

---

## 2. Ví dụ dễ hiểu

Có thể hình dung mạng máy tính giống như hai người nói chuyện:

* **Thiết bị** → người nói/người nghe
* **Đường truyền** → môi trường truyền âm thanh
* **Giao thức** → ngôn ngữ chung

Nếu hai người không hiểu cùng một ngôn ngữ thì dù âm thanh truyền được, họ vẫn không thể hiểu nhau.

Tương tự, các thiết bị mạng cần sử dụng những **giao thức tương thích** để giao tiếp.

---

## 3. Vì sao cần mạng máy tính?

Mục đích lớn nhất của mạng máy tính là:

> **CHIA SẺ**

### Các lợi ích chính

| Lợi ích                | Ví dụ                             |
| ---------------------- | --------------------------------- |
| **Chia sẻ tài nguyên** | Nhiều máy dùng chung máy in       |
| **Chia sẻ dữ liệu**    | File Server, Google Drive         |
| **Liên lạc**           | Email, Zalo, Discord, Google Meet |
| **Quản lý tập trung**  | Server công ty                    |
| **Sao lưu dữ liệu**    | NAS, Cloud Backup                 |
| **Truy cập từ xa**     | VPN                               |
| **Tiết kiệm chi phí**  | Không cần mỗi người một máy in    |

### Lưu ý

Mạng máy tính **không trực tiếp**:

* Làm CPU chạy nhanh hơn
* Tăng RAM vật lý
* Tăng dung lượng ổ cứng vật lý

---

# 4. Các thành phần của mạng

## 4.1 Node

**Node** là thiết bị tham gia vào mạng và có khả năng gửi hoặc nhận dữ liệu.

Ví dụ:

* Laptop
* Smartphone
* Server
* Máy in mạng
* Camera IP
* Smart TV
* Router

---

## 4.2 Đường truyền – Network Media

Là môi trường mà dữ liệu đi qua.

### Có dây

* Cáp xoắn đôi Ethernet
* Cáp quang

### Không dây

* Wi-Fi
* Bluetooth
* 4G
* 5G

---

## 4.3 NIC – Network Interface Card

**NIC** là phần cứng cho phép thiết bị kết nối vào mạng.

Ví dụ:

* Card Ethernet
* Card Wi-Fi

NIC thường có một địa chỉ gọi là:

```text
MAC Address
```

Ví dụ:

```text
00:1A:2B:3C:4D:5E
```

MAC Address dùng để nhận diện giao diện mạng ở tầng liên kết dữ liệu.

> MAC thường được nhà sản xuất gán sao cho hạn chế trùng lặp, nhưng MAC vẫn có thể bị thay đổi hoặc giả mạo.

---

# 5. Các thiết bị mạng quan trọng

## Switch

Dùng để kết nối nhiều thiết bị trong cùng mạng LAN.

```text
PC ──┐
PC ──┼── Switch
PC ──┤
PC ──┘
```

Switch chủ yếu sử dụng:

```text
MAC Address
```

để chuyển frame đến đúng thiết bị.

---

## Router

Router dùng để:

* Kết nối các mạng khác nhau
* Định tuyến gói tin
* Đưa thiết bị trong LAN ra Internet

Router chủ yếu đưa ra quyết định định tuyến dựa trên:

```text
IP Address
```

---

## Access Point

**Access Point (AP)** cho phép các thiết bị Wi-Fi kết nối vào mạng.

```text
Laptop )))
Phone  ))) → Access Point → LAN
Tablet )))
```

---

## Modem / ONT

Thiết bị kết nối mạng nhà bạn với hạ tầng của nhà cung cấp Internet.

Trong mạng cáp quang gia đình thường sử dụng **ONT**.

---

# 6. Client – Server

Mô hình phổ biến nhất trên Internet.

```text
Client
   │
   │ Request
   ▼
Server
   │
   │ Response
   ▼
Client
```

### Client

Thiết bị/phần mềm yêu cầu dịch vụ.

Ví dụ:

* Chrome
* Firefox
* App điện thoại

### Server

Máy/phần mềm cung cấp dịch vụ.

Ví dụ:

* Web Server
* Database Server
* File Server
* DNS Server

### Ví dụ

Khi mở:

```text
https://google.com
```

Trình duyệt là:

```text
Client
```

Google cung cấp:

```text
Server
```

---

# 7. Peer-to-Peer – P2P

Trong mô hình **Peer-to-Peer**, các thiết bị có vai trò tương đối ngang nhau.

Một thiết bị có thể vừa:

* Gửi dữ liệu
* Nhận dữ liệu
* Cung cấp tài nguyên

Ví dụ:

```text
PC A ←────→ PC B
 ↑           ↑
 └──── PC C ─┘
```

Ứng dụng điển hình:

* BitTorrent
* Một số hệ thống chia sẻ file ngang hàng

---

# 8. Client-Server vs Peer-to-Peer

| Client-Server           | Peer-to-Peer                         |
| ----------------------- | ------------------------------------ |
| Có server trung tâm     | Không nhất thiết có server trung tâm |
| Quản lý dễ              | Quản lý khó hơn                      |
| Phù hợp hệ thống lớn    | Phù hợp chia sẻ ngang hàng           |
| Server cung cấp dịch vụ | Peer vừa cho vừa nhận                |

---

# 9. Mạng gia đình

Một mạng gia đình thường có dạng:

```text
                    INTERNET
                        │
                        │
                     ISP
                        │
                        ▼
                 ┌──────────────┐
                 │ Router / ONT │
                 └──────┬───────┘
                        │
           ┌────────────┼────────────┐
           │            │            │
         Wi-Fi        Wi-Fi       Ethernet
           │            │            │
           ▼            ▼            ▼
        Laptop        Phone        Desktop
```

---

# 10. ISP là gì?

**ISP – Internet Service Provider**

Là nhà cung cấp dịch vụ Internet.

Ví dụ tại Việt Nam:

* Viettel
* VNPT
* FPT

ISP kết nối mạng nhà bạn với Internet.

---

# 11. LAN là gì?

**LAN – Local Area Network**

Là mạng trong phạm vi nhỏ.

Ví dụ:

* Nhà
* Phòng máy
* Trường học
* Văn phòng

Ví dụ IP trong LAN:

```text
192.168.1.10
192.168.1.20
192.168.1.30
```

---

# 12. Mạng có dây và không dây

| Có dây                 | Không dây              |
| ---------------------- | ---------------------- |
| Ethernet               | Wi-Fi                  |
| Ổn định                | Linh hoạt              |
| Độ trễ thường thấp     | Dễ bị nhiễu            |
| Tốc độ ổn định         | Phụ thuộc khoảng cách  |
| Ít chịu nhiễu vô tuyến | Chịu ảnh hưởng vật cản |

Trong thực tế thường sử dụng **kết hợp cả hai**.

Ví dụ:

```text
Server  → Ethernet
Desktop → Ethernet
Laptop  → Wi-Fi
Phone   → Wi-Fi
```

---

# 13. Internet là gì?

**Internet** là một hệ thống khổng lồ kết nối rất nhiều mạng khác nhau trên toàn thế giới.

Có thể hiểu đơn giản:

> Internet = Network of Networks

```text
Mạng nhà ──────┐
               │
Mạng trường ───┼──── INTERNET ──── Mạng Google
               │
Mạng công ty ──┘                 └─ Mạng YouTube
```

Internet phát triển từ các hệ thống mạng nghiên cứu ban đầu như **ARPANET** vào cuối những năm 1960.

---

# 14. Điều gì xảy ra khi mở một website?

Ví dụ nhập:

```text
google.com
```

## Bước 1 – DNS

Máy tính cần biết địa chỉ IP của:

```text
google.com
```

Nó hỏi DNS:

```text
google.com → IP nào?
```

DNS trả lại một địa chỉ IP phù hợp.

---

## Bước 2 – Tạo kết nối

Máy tính bắt đầu giao tiếp với server Google.

Các giao thức có thể tham gia gồm:

```text
IP
TCP hoặc QUIC/UDP
TLS
HTTP
```

---

## Bước 3 – Đóng gói dữ liệu

Dữ liệu được xử lý qua nhiều tầng mạng.

Ví dụ đơn giản:

```text
HTTP Data
   ↓
Transport
   ↓
IP Packet
   ↓
Ethernet / Wi-Fi Frame
```

---

## Bước 4 – Router gửi dữ liệu

```text
Computer
   ↓
Router
   ↓
ISP
   ↓
Internet
   ↓
Google Server
```

Các router trên Internet giúp đưa gói tin đến mạng đích.

---

## Bước 5 – Server trả dữ liệu

Google xử lý request rồi gửi response.

```text
Google Server
      ↓
   Internet
      ↓
   Router
      ↓
   Computer
```

---

## Bước 6 – Trình duyệt hiển thị

Browser nhận các tài nguyên như:

```text
HTML
CSS
JavaScript
Images
```

Sau đó render thành trang web.

---

# 15. Tổng quan quá trình

```text
Bạn nhập google.com
        │
        ▼
       DNS
        │
        ▼
   Lấy địa chỉ IP
        │
        ▼
 TCP/QUIC + TLS
        │
        ▼
      HTTP
        │
        ▼
      Router
        │
        ▼
        ISP
        │
        ▼
     Internet
        │
        ▼
 Google Server
        │
        ▼
     Response
        │
        ▼
     Browser
```

---

# 16. Một số thuật ngữ cần nhớ

| Thuật ngữ        | Ý nghĩa                             |
| ---------------- | ----------------------------------- |
| **Network**      | Mạng                                |
| **Node**         | Thiết bị/nút mạng                   |
| **Client**       | Máy/phần mềm yêu cầu dịch vụ        |
| **Server**       | Máy/phần mềm cung cấp dịch vụ       |
| **Protocol**     | Giao thức                           |
| **NIC**          | Card/giao diện mạng                 |
| **MAC Address**  | Địa chỉ tầng liên kết               |
| **IP Address**   | Địa chỉ logic trên mạng IP          |
| **LAN**          | Mạng cục bộ                         |
| **WAN**          | Mạng diện rộng                      |
| **ISP**          | Nhà cung cấp Internet               |
| **Router**       | Thiết bị định tuyến                 |
| **Switch**       | Thiết bị kết nối các node trong LAN |
| **Access Point** | Thiết bị cung cấp kết nối Wi-Fi     |
| **DNS**          | Phân giải tên miền                  |
| **HTTP/HTTPS**   | Giao thức web                       |
| **TCP**          | Giao thức truyền tải tin cậy        |
| **UDP**          | Giao thức truyền tải không kết nối  |

---

# 17. Thực hành

## Bài 1 – Xác định mạng quanh bạn

Liệt kê 3 mạng bạn sử dụng.

Ví dụ:

### Wi-Fi nhà

```text
Node:
- Laptop
- Điện thoại
- Smart TV

Thiết bị trung tâm:
- Router

Kết nối:
- Wi-Fi
- Ethernet
```

### Mạng 4G/5G

```text
Node:
- Smartphone

Kết nối:
- Sóng di động

Nhà mạng:
- Viettel / Vinaphone / Mobifone
```

### Wi-Fi trường

```text
Node:
- Laptop
- Smartphone

Thiết bị:
- Access Point
- Switch
- Router
```

---

# 18. Xem địa chỉ IP

## Windows

Mở:

```text
Command Prompt
```

Gõ:

```bash
ipconfig
```

Tìm:

```text
IPv4 Address
```

Ví dụ:

```text
IPv4 Address : 192.168.1.12
```

---

## Linux

```bash
ip addr
```

Có thể thấy:

```text
inet 192.168.1.12/24
```

---

# 19. Kiểm tra kết nối bằng Ping

Thử:

```bash
ping google.com
```

Windows thường hiển thị:

```text
Reply from ...: bytes=32 time=25ms TTL=117
```

Linux có thể hiển thị:

```text
64 bytes from ... time=25 ms
```

---

## time là gì?

Ví dụ:

```text
time=25ms
```

Là **Round Trip Time – RTT**.

Có thể hiểu đơn giản:

```text
Máy bạn
   ↓
Google
   ↓
Máy bạn
```

Tổng thời gian đi và quay lại:

```text
25 ms
```

Thông thường:

```text
RTT càng thấp
→ phản hồi mạng càng nhanh
```

Nhưng ping không phải là phép đo đầy đủ của tốc độ tải xuống/upload.

---

# 20. Các lệnh mạng cơ bản

### Windows

```bash
ipconfig
```

Xem cấu hình IP.

```bash
ping google.com
```

Kiểm tra khả năng kết nối và RTT.

```bash
tracert google.com
```

Xem các hop/router mà gói tin đi qua.

```bash
nslookup google.com
```

Kiểm tra DNS.

```bash
arp -a
```

Xem bảng ARP.

```bash
netstat -ano
```

Xem các kết nối và port đang sử dụng.

---

### Linux

```bash
ip addr
```

Xem IP.

```bash
ip route
```

Xem bảng định tuyến.

```bash
ping google.com
```

Kiểm tra kết nối.

```bash
traceroute google.com
```

Xem đường đi.

```bash
nslookup google.com
```

hoặc:

```bash
dig google.com
```

Kiểm tra DNS.

---

# 🧠 Mindmap ghi nhớ

```text
NETWORK
│
├── Node
│   ├── PC
│   ├── Phone
│   ├── Server
│   └── Printer
│
├── Media
│   ├── Ethernet
│   ├── Fiber
│   └── Wi-Fi
│
├── Devices
│   ├── Switch
│   ├── Router
│   └── Access Point
│
├── Address
│   ├── MAC
│   └── IP
│
├── Protocol
│   ├── TCP
│   ├── UDP
│   ├── HTTP
│   └── DNS
│
└── Model
    ├── Client-Server
    └── Peer-to-Peer
```

---

# 🔑 Kiến thức bắt buộc nhớ

### 1

```text
Network = từ 2 thiết bị trở lên kết nối để trao đổi dữ liệu.
```

### 2

Ba yếu tố cơ bản:

```text
Device + Media + Protocol
```

### 3

Mục đích chính:

```text
CHIA SẺ
```

### 4

```text
Switch → kết nối thiết bị trong LAN
Router → kết nối/định tuyến giữa các mạng
Access Point → cung cấp kết nối Wi-Fi
```

### 5

```text
MAC → nhận diện giao diện mạng ở Layer 2
IP  → địa chỉ logic dùng cho định tuyến
```

### 6

```text
Client → yêu cầu dịch vụ
Server → cung cấp dịch vụ
```

### 7

```text
LAN → mạng cục bộ
WAN → mạng diện rộng
Internet → mạng của các mạng
```

### 8

Khi truy cập website:

```text
Domain
   ↓
DNS
   ↓
IP
   ↓
Router
   ↓
Internet
   ↓
Server
   ↓
Response
```

---

# 🎯 Câu hỏi tự kiểm tra

1. Mạng máy tính là gì?
2. Hai máy tính kết nối với nhau có được gọi là mạng không?
3. Node là gì?
4. NIC có chức năng gì?
5. MAC Address là gì?
6. IP Address dùng để làm gì?
7. Switch và Router khác nhau như thế nào?
8. Access Point dùng để làm gì?
9. LAN là gì?
10. ISP là gì?
11. Client là gì?
12. Server là gì?
13. Peer-to-Peer khác Client-Server như thế nào?
14. DNS có nhiệm vụ gì?
15. Khi nhập `google.com`, tại sao máy tính phải hỏi DNS?
16. `ping` dùng để làm gì?
17. `time=20ms` trong ping có ý nghĩa gì?
18. Internet được gọi là “mạng của các mạng” vì sao?

---

# 📌 Công thức nhớ nhanh

```text
Thiết bị muốn giao tiếp
        ↓
       NIC
        ↓
Ethernet / Wi-Fi
        ↓
      Switch
        ↓
      Router
        ↓
       ISP
        ↓
    INTERNET
        ↓
     SERVER
```

Đây là **bức tranh nền tảng** trước khi học sâu hơn về:

```text
OSI
TCP/IP
Ethernet
MAC
ARP
IPv4
Subnetting
DHCP
DNS
Routing
TCP/UDP
HTTP/HTTPS
NAT
Firewall
VPN
```

