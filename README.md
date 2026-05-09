# Quartus 13.0 + MAX7000 image

This repository builds a Docker image based on `raetro/quartus:base` and installs:

- Quartus Web Edition 13.0sp1 installer from Intel CDN
- MAX family device support from `files/max_web-13.0.1.232.qdz`

## Build locally

```bash
docker build -t quartus13-max7000:latest .
```

## Notes

- The Dockerfile fetches `QuartusSetupWeb-13.0.1.232.run` from Intel CDN at build time.
- The resulting image is intended for EPM7128 / MAX7000 synthesis.
- You can later publish it to GHCR and consume it from CI.
