# Naive-Bayes-for-Classificaion
## Giới thiệu
**Text Classification (Tạm dịch: Phân loại văn bản)** là một trong những bài toán phổ biến trong lĩnh vực Machine Learning và Natural Language Processing. Trong đó, nhiệm vụ của chúng ta là xây dựng một chương trình có khả năng phân loại văn bản vào các phân lớp do chúng ta quy định. Các ứng dụng phổ biến liên quan đến loại chương trình này có thể kể đến phát hiện các bình luận tiêu cực trên không gian mạng, các đánh giá tích cực của sản phẩm...

<img width="640" height="239" alt="Screenshot 2025-07-23 at 9 36 04 PM" src="https://github.com/user-attachments/assets/ed269722-0522-42f2-8cf8-63b8d96008d2" />

Trong project này, chúng ta sẽ xây dựng một chương trình Text Classification liên quan đến việc phân loại một đoạn tin nhắn là tin nhắn spam hay không. Dự án sẽ khám phá và triển khai hai phương pháp tiếp cận chính để giải quyết bài toán này:
- **Naive Bayes Classifier**: Một thuật toán học máy truyền thống dựa trên định lý Bayes với giả định độc lập có điều kiện giữa các đặc trưng, thường hiệu quả cho các bài toán phân loại văn bản.
- **Phân loại sử dụng Cơ sở dữ liệu Vector (Vector Database) và Sentence Embeddings**: Một phương pháp hiện đại hơn, trong đó các tin nhắn được biểu diễn dưới dạng vector ngữ nghĩa (embeddings) và việc phân loại dựa trên việc tìm kiếm sự tương đồng trong một cơ sở dữ liệu vector tốc độ cao như FAISS.

Theo đó, Input/Output chung của chương trình sẽ bao gồm:
- **Input**: Một đoạn tin nhắn (text).
- **Output**: Có là tin nhắn spam hay không (bool).

Dựa vào các thông tin trên, ta sẽ xây dựng được 2 luồng xử lý (pipeline) cho bài toán này như
sau:

<img width="667" height="614" alt="Screenshot 2025-07-23 at 9 41 25 PM" src="https://github.com/user-attachments/assets/b8226349-1ffe-491d-ac32-fa39a4b537cc" />

