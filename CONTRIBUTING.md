# Contributing

Thanks for helping improve this project. Keep changes focused, practical, and easy to review.

## Workflow

1. Create a branch from `main`.
2. Make a small, focused change.
3. Run the basic local checks.
4. Open a Pull Request into `main`.

```bash
python -m py_compile server.py
docker compose --env-file .env.example config --quiet
```

## Pull Request Checklist

- README examples still match the actual API endpoints and ports.
- `.env`, tokens, model files, and generated images are not committed.
- Docker Compose still validates with `.env.example`.
- Changes are scoped to one clear purpose.

## Development Notes

- Keep the API local-first and simple to run.
- Prefer environment variables for runtime configuration.
- Do not download model weights during tests or CI.
- Keep large model assets and generated outputs outside Git.
