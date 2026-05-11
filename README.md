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

`mkdir wordpress-docker`

`cd wordpress-docker`

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

👉 KẾT QUẢ: GIAO DIỆN WORDPRESS

<img width="1920" height="1030" alt="image" src="https://github.com/user-attachments/assets/52599bbf-f7fc-415c-b56c-cce12d76e7fc" /></P>

---

## 9. CÀI PLUGIN 

- Plugins → Add Plugin

<img width="1545" height="750" alt="image" src="https://github.com/user-attachments/assets/2e1873fc-bc08-439c-8659-18f24e400fe5" /></p>

- Cài plugin login: Trong bài tập này em sẽ sử dụng Elementor. Đây là plugin "quốc dân" giúp bạn thiết kế giao diện website bằng cách kéo thả cực kỳ trực quan.

<img width="1548" height="746" alt="{25B7C6C3-3A31-4AA5-B24A-4C86D2113ED6}" src="https://github.com/user-attachments/assets/b28dc927-8608-46b7-88cb-1313475e4792" /></p>

- Nhấn nút **Install Now** tại plugin tên là *Elementor Website Builder* -> Sau khi cài xong, nhấn **Activate**.

<img width="1542" height="741" alt="{6A3E5F05-4FD4-4AAE-9871-A5BEDF3A7575}" src="https://github.com/user-attachments/assets/4f25356d-fb76-4274-8859-9d15cd8aa8a1" /></p>

👉 KẾT QUẢ: 

<img width="1920" height="1031" alt="image" src="https://github.com/user-attachments/assets/a282e3c1-b5fd-42a3-8a84-107fb5ea53ed" /></p>

- Tạo trang mới: Tiến hành kéo thả các Widget (Công cụ)

<img width="1920" height="1026" alt="{9CD82189-0FE6-43D9-A384-40502A486020}" src="https://github.com/user-attachments/assets/ccd5b814-578d-4baa-a368-09cdfd617c19" /></p>

✔️ Public

- Set làm trang chủ: Settings → Reading → A static page

<img width="1541" height="747" alt="{7C836A96-5AB7-4D2F-836E-E0D8E4AA031A}" src="https://github.com/user-attachments/assets/1069616b-5d7e-4ea6-abe1-f04aff03b319" /></p>

---

## 10. KIỂM TRA

- Truy cập: `http://<IP_UBUNTU>:8080/wp-admin`

<img width="1918" height="1027" alt="{77A06843-4410-4079-B687-4CB82A367D37}" src="https://github.com/user-attachments/assets/a0033d36-5ec1-4044-8507-b377611008be" /></p>

<img width="1920" height="1019" alt="{0615D502-B204-450A-B9C4-21A45EFEBDB8}" src="https://github.com/user-attachments/assets/2dd277e6-152c-4131-80c8-34a1c75149bd" /></p>

<img width="1920" height="1018" alt="{FA7EEFF3-0397-4A45-9B3E-04875559138D}" src="https://github.com/user-attachments/assets/b4ea5c5d-40eb-43be-b754-04ee9eef0409" /></p>

<img width="1920" height="1019" alt="{E2A0B92A-70CB-4CD0-812D-BB7F8801260E}" src="https://github.com/user-attachments/assets/5dc86fb4-75f4-40ab-81ce-d0bec1f9083b" /></p>

<img width="1920" height="1022" alt="{B8729AF9-9B3C-41B0-886D-51D442BB53FF}" src="https://github.com/user-attachments/assets/72d58a3e-61da-4588-9500-17f3370e729d" /></p>

<img width="1920" height="1025" alt="{0C46D5BE-314A-4495-8849-3F231EE55871}" src="https://github.com/user-attachments/assets/5cc510a2-9c66-4430-ba59-9a6e2e3a194d" /></p>

---

## 11. KIỂM TRA MARIADB

- Vào MariaDB sử dụng lệnh sau:

`sudo docker exec -it mariadb_container mariadb -u wp_user -pwp_pass wordpress`

- Sau khi vào thì ta có thể thử 1 số lệnh để check

`SHOW TABLES; `

<img width="1087" height="717" alt="{B79F15AF-BEF2-43BA-B47A-668CD798CA8E}" src="https://github.com/user-attachments/assets/14ca4c92-d0b8-425d-bdd9-a74937022dac" />

- Xem danh sách các trang/bài viết bạn đã tạo (để thấy cái "Elementor #7" của bạn nằm trong này):

`SELECT post_title, post_status FROM wp_posts WHERE post_type='page';`

<img width="1194" height="758" alt="{E66624C4-E249-49D5-9663-17434C82B146}" src="https://github.com/user-attachments/assets/063b108e-c64d-4e7e-b434-af80f1faadb9" />

- Xem thông tin user admin của bạn:

`SELECT user_login, user_email FROM wp_users;`

<img width="1080" height="731" alt="{F6A39398-3D25-422D-99B0-0FA982BE9D38}" src="https://github.com/user-attachments/assets/5d5fbb22-3f47-4dc5-bacb-387e9b5197a0" /></P>

---

## 12. PUBLIC WEB 

- Bước 1: Login Cloudflare `cloudflared tunnel login ` -> Sau khi truy cập đường dẫn sẽ hiển thị cửa sổ claudfare -> tại đây ta chọn **Authrize** để đăng nhập

<img width="1400" height="741" alt="image" src="https://github.com/user-attachments/assets/2bcee916-e8c6-4f40-893b-1ebf80f63ed5" /></p>

<img width="1163" height="613" alt="{66FDB182-ED93-49A2-9B89-FD4DD4B1DBFB}" src="https://github.com/user-attachments/assets/00d1cffd-d220-46f8-a25c-54b0aa94721f" /></p>

✔ Sau khi click vào **Authorize** sẽ hiện thông báo Success -> Đồng thời trong Ubuntu cũng tự động sinh ra file **.pem**

<img width="1920" height="1027" alt="{B4F53AC3-E388-44D6-8915-07F87957A4C0}" src="https://github.com/user-attachments/assets/929648ba-7540-49db-9277-ca128052992b" /></p>

<img width="1129" height="719" alt="{4FD3631D-095C-45AB-8F2F-F1AFF54ED658}" src="https://github.com/user-attachments/assets/85a3959e-47bb-4522-9ccd-5c528d897ab2" /></p>


- Bước 2: Thêm cloudflared service `mkdir cloudflare`

<img width="1544" height="590" alt="{48874CBE-15E5-47DF-9B73-5DCA9B4EDA77}" src="https://github.com/user-attachments/assets/581ad2ef-6b0b-4691-a8c8-f21844543941" /></p>

- Bước 3: Tạo tunnel `cloudflared tunnel create wordpress-duong`

<img width="1268" height="744" alt="{83236AA0-B6BE-4AED-A050-E97AB5B00C09}" src="https://github.com/user-attachments/assets/d060732c-7981-4bf4-9d94-efe2febfefb2" /></P>

- Bước 5: Tạo config `nano cloudflare/config.yml`

<img width="1362" height="873" alt="{D8AA6F04-0D5F-4727-A79F-AD9D6302C52E}" src="https://github.com/user-attachments/assets/e2d1621d-908a-458f-8e6f-bb35b553032c" /></p>

- Bước 6: Thêm service claudfare

<img width="1142" height="663" alt="{94531F32-A851-4A3D-898A-09745355A0AA}" src="https://github.com/user-attachments/assets/892080b5-0e00-49f7-a983-26a0e798743f" /></p>

- Bước 7: Tạo DNS

`
docker run --rm -it \
-v ~/.cloudflared:/home/nonroot/.cloudflared \
cloudflare/cloudflared:latest \
tunnel --origincert /home/nonroot/.cloudflared/cert.pem route dns 3166e182-f17b-4f59-991d-40e033c46fac wp.ducduong.id.vn
`

<img width="1228" height="839" alt="{A9CA7AB8-1386-4E97-955D-E3E526169485}" src="https://github.com/user-attachments/assets/baa5ff51-7050-4caf-b39e-59b9ed8bad32" /></p>

- Bước 8: Chạy tunnel

`
docker run --rm -it \
  -v ~/.cloudflared:/home/nonroot/.cloudflared \
  cloudflare/cloudflared:latest \
  tunnel --config /home/nonroot/.cloudflared/config.yml run
`

<img width="1222" height="837" alt="{4F0161C6-1D11-488B-92F2-A2625B79E03F}" src="https://github.com/user-attachments/assets/b5ae2066-4d64-4c0b-bd96-4f7d6b54f85d" /></p>

---

## 13. KIỂM TRA

👉 Truy cập  `http://wp.ducduong.id.vn `

- Bài viết Giới thiệu bản thân

<img width="1920" height="1024" alt="{31587753-1E98-4B9C-8F4D-404684B60725}" src="https://github.com/user-attachments/assets/b6b5cb77-3081-499c-b567-322f0b37c9bb" /></p>

- Bài viết Giới thiệu nghành học yêu thích

<img width="1920" height="1022" alt="{92FA1F12-B6AD-4C77-BCBA-8F1811BC9835}" src="https://github.com/user-attachments/assets/1baa4737-8f01-40ab-9e34-753060eaecb3" /></p>

<img width="1920" height="1015" alt="{5CB6E49F-B145-47F9-ACC9-2DBF9B153B78}" src="https://github.com/user-attachments/assets/f47f9211-9dbf-45ed-9d45-24eb14a0a229" /></p>

- Video giới thiệu nghành học

<img width="1920" height="1012" alt="{C2F02C0C-92B8-4DBF-8A75-82AB915104FA}" src="https://github.com/user-attachments/assets/e39d34ca-b964-4285-967b-b8c2ece25bb2" /></p>
























