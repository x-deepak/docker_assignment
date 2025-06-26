FROM ghcr.io/astral-sh/uv:python3.13-bookworm-slim

WORKDIR /app

COPY pyproject.toml uv.lock ./
RUN uv pip install --system --no-cache .

COPY . .

EXPOSE 8002

CMD ["uv", "run", "app.py"]