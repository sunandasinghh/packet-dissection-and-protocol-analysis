# HTTP Arotocol Analysis
## CAPTURE :'http_capture.pcapng'
  -**Protocol** :HTTP
  -**Captured using** : Wireshark + 'curl http://example.com'
  -**Source IP** :192.168.x.x [local machine]
  -**Destination IP:** 93.184.216.34 *(example.com)*
##Ports
  -Source port : 5678(some random high port)
  -Destination port 80 
  ## 🔍 Packet Breakdown

### ▶️ HTTP GET Request

- **Method:** `GET`
- **Host:** example.com
- **User-Agent:** curl/7.x.x
- **Accept:** */*

📌 *This is the request sent by your system to fetch the webpage.*

---

### ◀️ HTTP Response

- **Status Line:** `HTTP/1.1 200 OK`
- **Content-Type:** `text/html`
- **Content-Length:** Varies
- **Server:** ECS (Edgecast)

📌 *This is the server replying with the requested page (HTML).*
