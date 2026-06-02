# Quartus 13.0 + MAX7000 image

This repository builds a Docker image based on `raetro/quartus:base` and installs:

- Quartus Web Edition 13.0sp1 installer from Intel CDN
- MAX7000 family device support from

## Build locally

```bash
docker build -t quartus13-max7000:latest .
```
