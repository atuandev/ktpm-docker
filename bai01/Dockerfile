# Sử dụng Node.js 18 Alpine (nhẹ hơn bản thông thường)
FROM node:18-alpine

# Tạo thư mục làm việc trong container
WORKDIR /usr/src/app

# Sao chép package.json và package-lock.json
COPY package*.json ./

# Cài đặt các dependencies (sử dụng --production nếu chỉ cần dependencies runtime)
RUN npm install --production

# Sao chép toàn bộ mã nguồn ứng dụng
COPY . .

# Mở cổng 3000 để ứng dụng lắng nghe
EXPOSE 3000

# Khởi chạy ứng dụng
CMD ["node", "index.js"]