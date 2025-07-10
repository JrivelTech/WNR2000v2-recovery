# 🔧 Netgear WNR2000v2 Recovery

Este repositorio documenta el proceso completo de recuperación de un router Netgear WNR2000v2 mediante UART, TFTP y modo CFE, probando múltiples firmwares y técnicas de hard reset.  
Una guía técnica para entusiastas del rescate embebido.

## 📦 Requisitos

- Adaptador USB a TTL
- Cables jumper
- Software terminal (PuTTY, Tera Term, etc.)
- Laptop con servidor TFTP activo
- Firmwares originales desde la web de Netgear

## ⚙️ Procedimiento resumido

1. Conectar por UART con configuración 115200 8N1
2. Acceder al modo CFE en terminal
3. Transferir firmware vía TFTP:
   ```bash
   tftp -i 192.168.1.1 PUT firmware.img
