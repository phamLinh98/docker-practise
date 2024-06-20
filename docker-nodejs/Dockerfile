# Sử dụng image chính thức của Node.js
FROM node:18

# Tạo và chỉ định thư mục làm việc trong container
WORKDIR /usr/src/app

# Sao chép file package.json và package-lock.json (nếu có)
COPY package*.json ./

# Cài đặt các phụ thuộc của dự án
RUN npm install

# Sao chép toàn bộ mã nguồn của dự án vào container
COPY . .

# Expose cổng mà ứng dụng sẽ chạy
EXPOSE 3000

# Lệnh để chạy ứng dụng
CMD [ "node", "app.js" ]

