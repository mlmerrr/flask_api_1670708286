# ใช้ base image เป็น nginx
FROM nginx:alpine

# ลบ default config (optional แต่แนะนำ)
RUN rm -rf /usr/share/nginx/html/*

# คัดลอกไฟล์ HTML/CSS/JS ไปไว้ใน nginx
COPY . /usr/share/nginx/html

# Expose port 80 สำหรับให้ Azure เข้าถึง
EXPOSE 80

# ใช้คำสั่งเริ่มต้นของ nginx
CMD ["nginx", "-g", "daemon off;"]