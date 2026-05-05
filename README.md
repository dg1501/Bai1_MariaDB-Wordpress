## PHÁT TRIỂN ỨNG DỤNG VỚI MÃ NGUỒN MỞ (MARIADB + WORDPRESS)
### HỌ TÊN: NGUYỄN ĐỨC DƯƠNG
### LỚP: K58KTP
### MSSV: K225480106093

---

## 1. CHUẨN BỊ 

1. Kiểm tra phiên bản Docker & Docker Compose

`docker --version`

`docker-compose --version`

<img width="1028" height="260" alt="{9551D12A-6892-417F-AD61-BCE85556540A}" src="https://github.com/user-attachments/assets/7e834818-bd3c-4505-b753-40ee652c15f2" /></p>

---

## 2. TẠO PROJECT

`
mkdir wordpress-docker
cd wordpress-docker
`

<img width="1000" height="689" alt="{8BA11C69-CDFD-4924-9951-6B42061B89ED}" src="https://github.com/user-attachments/assets/0e78aa4b-ae97-4b56-91a2-6e2d1acbd70e" /></p>

---

## 3. TẠO FILE DOCKER - COMPOSE.YML

`nano docker-compose.yml`

- Ban đầu file yml sẽ trống -> ta cần thêm nội dung vào file.

<img width="1270" height="831" alt="{56CAB8BD-8816-4A4A-A91E-45E24EF38501}" src="https://github.com/user-attachments/assets/e5d62221-1c59-41e9-836d-5b88e0aef998" /></P>

<img width="1337" height="879" alt="{CDF9D334-1502-4413-AF46-2C6A6D8F7175}" src="https://github.com/user-attachments/assets/d261863c-0221-4118-a773-66b59b0aecfd" /></p>

---

## 4. CHẠY HỆ THỐNG 

`docker-compose up -d`

<img width="1251" height="883" alt="{47393016-F945-42B4-A9D7-7FC26DE1E43E}" src="https://github.com/user-attachments/assets/3b134739-08c3-4ad8-9904-6cfa77d58c1b" /></p>

---

## 5. KIỂM TRA CONTAINER 

`docker ps`

<img width="999" height="706" alt="{5C6AA715-6795-4CF9-BC47-DE55AA5C5157}" src="https://github.com/user-attachments/assets/24fd0219-9317-4526-9bcf-816ee8d07b15" /></P>

🚀 Nếu thấy 2 container: **Mariadb** và **Wordpress** là đã thành công.

---

## 6. TRUY CẬP WEBSITE 

- Lấy IP ubuntu

`ip a`

<img width="1000" height="706" alt="image" src="https://github.com/user-attachments/assets/d9d3846b-617b-4a69-b39c-fa32217d3093" /></p>

- Truy cập: `http://172.28.35.87:8080`

<img width="1920" height="1080" alt="{9C0BDBD4-272E-4EE2-B3EF-52920027C8F1}" src="https://github.com/user-attachments/assets/a71abeca-db72-4dfb-a6f3-70c807f66aef" /></p>

---

## 7. CÀI ĐẶT WORDPRESS

- Khi mở web sẽ thấy giao diện cài đặt.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/2c7c358d-a1bf-4fcb-b147-f0d2f5a32456" /></p>

Điền:

Site Title: My Website

Username: Nguyễn Đức Dương

Password: (tự đặt)

Email: (tùy)

👉 Đây chính là login WordPress

<img width="1920" height="1027" alt="{3678C901-BD8F-45AE-BD73-C77CC9DE8D3C}" src="https://github.com/user-attachments/assets/6e11f09c-cae5-4a43-afb6-6c067cb7f641" /></p>

🎯 KẾT QUẢ

<img width="1538" height="766" alt="{EE5E022C-41E4-4934-A69E-EA6F346580D7}" src="https://github.com/user-attachments/assets/14d23382-b0b3-4f8f-952e-663c634ec928" /></p>

---

## 8. ĐĂNG NHẬP ADMIN

- Sau khi cài xong: truy cập `http://<IP>:8080/wp-admin` -> Đăng nhập bằng tài khoản vừa tạo.

<img width="1549" height="740" alt="{BC5B9FDB-1FC3-48CA-A678-E9249B791BA5}" src="https://github.com/user-attachments/assets/e9866b61-e3e1-4482-9ff3-a8768c917c1a" /></p>









