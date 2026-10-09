# Báo cáo thực hành kiểm thử API bằng Postman

## 1. Mục tiêu

* Làm quen với công cụ Postman.
* Thực hành gửi HTTP GET Request.
* Kiểm tra HTTP status code và dữ liệu JSON.
* Viết test script tự động bằng JavaScript.
* Lưu trữ bộ kiểm thử trên GitHub.

## 2. Công cụ sử dụng

* **Postman:** Gửi request và thực hiện kiểm thử API.
* **PokéAPI:** API cung cấp dữ liệu Pokémon.
* **GitHub:** Lưu trữ Collection và báo cáo.

## 3. Nội dung thực hành

### 3.1. Kiểm thử thông tin Pikachu

* Method: GET
* URL: `https://pokeapi.co/api/v2/pokemon/pikachu`
* Kết quả mong đợi: HTTP 200 và dữ liệu JSON của Pikachu.

Các test đã thực hiện:

1. Kiểm tra status code bằng 200.
2. Kiểm tra response có định dạng JSON.
3. Kiểm tra tên Pokémon bằng `pikachu`.
4. Kiểm tra Pokémon có danh sách abilities.

**Kết quả:** 4/4 test PASSED.

![Kết quả kiểm thử Pikachu](screenshots/get-pikachu.png)

### 3.2. Kiểm thử danh sách Pokémon

* Method: GET
* URL: `https://pokeapi.co/api/v2/pokemon?limit=10`
* Kết quả mong đợi: HTTP 200 và danh sách Pokémon có dữ liệu.

Các test đã thực hiện:

1. Kiểm tra status code bằng 200.
2. Kiểm tra response có danh sách Pokémon.
3. Kiểm tra phần tử đầu tiên có tên và URL.

**Kết quả:** Ghi lại số test thành công sau khi chạy thực tế.

![Kết quả kiểm thử danh sách Pokémon](screenshots/get-pokemon-list.png)

## 4. Kết luận

Qua bài thực hành, sinh viên đã sử dụng Postman để gửi GET Request, kiểm tra dữ liệu JSON và xây dựng các test tự động. Bộ kiểm thử được lưu dưới dạng Postman Collection để thuận tiện cho việc chia sẻ và thực hiện lại.

## 5. Tài liệu tham khảo

* Video hướng dẫn: https://www.youtube.com/watch?v=MFxk5BZulVU
* PokéAPI: https://pokeapi.co/
* Postman Learning Center: https://learning.postman.com/docs/getting-started/overview/

## 6. Sản phẩm

* `postman-collection.json`: Bộ request và test script.
* `screenshots/`: Ảnh chụp kết quả thực hành.
