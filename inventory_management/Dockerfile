# Your Solution
FROM --platform=linux/amd64 python:3.11-slim
WORKDIR /usr/src/app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . /usr/src/app
EXPOSE 8001
ENV DATABASE_URL=postgresql://sit722_sandara_user:G1wuYwwPCbcjIlLJZpBZD9d5B4eNSbVY@dpg-crpn8ct6l47c73am2i6g-a.oregon-postgres.render.com/sit722_sandara
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8001"]
