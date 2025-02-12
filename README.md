

# Forkify 🍴

Forkify là một ứng dụng web cho phép bạn tìm kiếm và lưu trữ công thức nấu ăn từ nhiều nguồn khác nhau. Ứng dụng này được xây dựng bằng JavaScript và sử dụng API để lấy dữ liệu công thức.

Forkify is a web application that allows you to search and store recipes from various sources. This application is built with JavaScript and uses an API to fetch recipe data.

## Tính năng ✨ / Features ✨

- Tìm kiếm công thức nấu ăn 🔍 / Search for recipes 🔍
- Xem chi tiết công thức 📋 / View recipe details 📋
- Lưu công thức yêu thích ❤️ / Save favorite recipes ❤️
- Điều chỉnh số lượng nguyên liệu dựa trên khẩu phần ăn 🍽️ / Adjust ingredient quantities based on servings 🍽️

## Kiến trúc MVC 🏗️ / MVC Architecture 🏗️

Ứng dụng này được xây dựng theo mô hình MVC (Model-View-Controller):

This application is built following the MVC (Model-View-Controller) pattern:

- **Model**: Quản lý dữ liệu và logic nghiệp vụ. Các tệp liên quan bao gồm `model.js`, xử lý trạng thái ứng dụng và xử lý dữ liệu từ API. / Manages data and business logic. Relevant files include `model.js`, which handles the application state, and processes data from the API.
- **View**: Hiển thị dữ liệu và giao diện người dùng. Các tệp liên quan bao gồm `views/recipeView.js`, `views/resultsView.js`, `views/bookmarksView.js`, `views/addRecipeView.js`, và `views/paginationView.js`. / Displays data and user interface. Relevant files include `views/recipeView.js`, `views/resultsView.js`, `views/bookmarksView.js`, `views/addRecipeView.js`, and `views/paginationView.js`.
- **Controller**: Xử lý tương tác người dùng và cập nhật Model và View. Tệp liên quan là `controller.js`, điều phối các hành động giữa Model và View. / Handles user interactions and updates the Model and View. The relevant file is `controller.js`, which coordinates actions between the Model and View.

## API 🌐

Forkify sử dụng API để lấy dữ liệu công thức. Dưới đây là một số thông tin về cách API được sử dụng trong ứng dụng:
Link lấy API: [https://forkify-api.jonas.io/api/v2/recipes?search=pizza](https://forkify-api.jonas.io/)
Forkify uses an API to fetch recipe data. Below is some information on how the API is used in the application:

- **URL API**: URL cơ bản của API được lưu trữ trong tệp `config.js` và được sử dụng trong các hàm gọi API. / The base URL of the API is stored in the `config.js` file and is used in API call functions.
- **Trợ giúp AJAX**: Hàm AJAX trong tệp `helpers.js` được sử dụng để thực hiện các yêu cầu HTTP tới API. / The AJAX function in the `helpers.js` file is used to make HTTP requests to the API.

### Các hàm API chính / Main API Functions

- `loadRecipe`: Hàm này tải dữ liệu công thức dựa trên ID và cập nhật trạng thái ứng dụng. / This function loads recipe data based on the ID and updates the application state.
- `loadSearchResults`: Hàm này tải kết quả tìm kiếm dựa trên từ khóa tìm kiếm và cập nhật trạng thái ứng dụng. / This function loads search results based on the search keyword and updates the application state.
- `uploadRecipe`: Hàm này tải lên một công thức mới và cập nhật trạng thái ứng dụng. / This function uploads a new recipe and updates the application state.

Để biết thêm thông tin, liên hệ vanlocdev@gmail.com.

For more information, contact vanlocdev@gmail.com.
