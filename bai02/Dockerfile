# Sử dụng Python 3.9 làm base image
FROM python:3.9-slim

# Thiết lập thư mục làm việc trong container
WORKDIR /app

# Sao chép các file cần thiết vào container
COPY app.py .
COPY requirements.txt .

# Cài đặt các dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Mở cổng 5000
EXPOSE 5000

# Chạy ứng dụng khi container được khởi động
CMD ["python", "app.py"]