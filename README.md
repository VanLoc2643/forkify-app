# Forkify

Forkify là một ứng dụng web cho phép bạn tìm kiếm và lưu trữ các công thức nấu ăn từ nhiều nguồn khác nhau. Ứng dụng này được xây dựng bằng JavaScript và sử dụng API để lấy dữ liệu công thức.

## Tính năng

- Tìm kiếm công thức nấu ăn
- Xem chi tiết công thức
- Lưu công thức yêu thích
- Điều chỉnh số lượng nguyên liệu theo khẩu phần

## Kiến trúc MVC

Ứng dụng này được xây dựng theo mô hình MVC (Model-View-Controller):

- **Model**: Quản lý dữ liệu và logic nghiệp vụ. Các tệp liên quan bao gồm `model.js`, nơi quản lý trạng thái ứng dụng, tải và xử lý dữ liệu từ API.
- **View**: Hiển thị dữ liệu và giao diện người dùng. Các tệp liên quan bao gồm `views/recipeView.js`, `views/resultsView.js`, `views/bookmarksView.js`, `views/addRecipeView.js`, và `views/paginationView.js`.
- **Controller**: Xử lý các tương tác từ người dùng và cập nhật Model và View. Tệp liên quan là `controller.js`, nơi điều phối các hành động giữa Model và View.

## API

Ứng dụng Forkify sử dụng API để lấy dữ liệu công thức nấu ăn. Dưới đây là một số thông tin về cách sử dụng API trong ứng dụng:

- **API URL**: URL cơ bản của API được lưu trong tệp `config.js` và được sử dụng trong các hàm gọi API.
- **AJAX Helper**: Hàm AJAX trong tệp `helpers.js` được sử dụng để thực hiện các yêu cầu HTTP đến API.

### Các hàm API chính

- `loadRecipe`: Hàm này tải dữ liệu công thức dựa trên ID và cập nhật trạng thái ứng dụng.
- `loadSearchResults`: Hàm này tải kết quả tìm kiếm dựa trên từ khóa tìm kiếm và cập nhật trạng thái ứng dụng.
- `uploadRecipe`: Hàm này tải lên một công thức mới và cập nhật trạng thái ứng dụng.
