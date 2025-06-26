FROM ghcr.io/astral-sh/uv:python3.13-bookworm-slim

WORKDIR /app

COPY . .

RUN uv pip install --system --no-cache .
RUN apt-get update && apt-get install -y curl


EXPOSE 8002

CMD ["uv", "run", "app.py"]