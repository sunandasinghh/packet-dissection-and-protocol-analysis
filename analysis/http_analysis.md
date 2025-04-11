# HTTP Protocol Analysis

## Capture File: `http_capture.pcapng`

## Summary

- **Protocol:** HTTP
- **Captured Using:** Wireshark and `curl http://example.com`
- **Source IP:** 192.168.x.x (local machine)
- **Destination IP:** 93.184.216.34 (example.com)
- **Ports:**
  - Source Port: 56789 (random high port)
  - Destination Port: 80 (HTTP)

---

## Packet Breakdown

### HTTP GET Request

- **Method:** `GET`
- **Host:** example.com
- **User-Agent:** curl/7.x.x
- **Accept:** */*

This is the request sent by my system to fetch the webpage.

---

### HTTP Response

- **Status Line:** `HTTP/1.1 200 OK`
- **Content-Type:** `text/html`
- **Content-Length:** Varies
- **Server:** ECS (Edgecast)

This is the server replying with the requested HTML content.

---

## Wireshark Filters Used

```plaintext
http
http.request
http.response

