# Security Policy

## Supported Version

This repository currently supports the `main` branch.

## Reporting a Vulnerability

If you find a security issue, avoid posting secrets or private data in a public issue. Contact the repository owner directly, or use GitHub private vulnerability reporting if it is enabled.

## Operational Guidance

- Set a strong `API_KEY` before exposing the API outside your local machine.
- Do not commit `.env`, `HF_TOKEN`, API keys, model weights, or generated private outputs.
- Rotate `API_KEY` and `HF_TOKEN` immediately if they are exposed.
- Run the service behind a trusted network or reverse proxy before public use.
- Keep Docker images and Python dependencies updated.
