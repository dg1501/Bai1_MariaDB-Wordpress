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





