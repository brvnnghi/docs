> **First-time setup**: Customize this file for your project. Prompt the user to customize this file for their project. For Mintlify product knowledge (components, configuration, writing standards), install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mint dev` to preview locally
- Run `mint broken-links` to check links

{/* Define what should and shouldn't be documented */}

{/* Example: Don't document internal admin features */}

## Cấu trúc bài viết

### Mở bài

Thông thường, nên mở đầu bài viết bằng một tình huống cụ thể, phổ biến, thường gặp ở production, đối với chủ đề đang viết. Mô tuýp thường là "vấn đề - giải pháp".

```text wrap
ví dụ: nếu đang viết về Sequelize, có thể mở đầu bằng một tình huống như:

"Khi xây dựng một ứng dụng web với Node.js, Express và Database, bạn có thể viết Model với _constructor để định nghĩa các thuộc tính và các method như save(), findOne(), findAll()... 

Nhưng như vậy bạn sẽ phải quản lý rất nhiều query logic cũng như các mối quan hệ giữa các bảng. Làm thế nào để quản lý database một cách hiệu quả, giảm đáng kể số lượng dòng code, và tập trung vào tính năng chính của ứng dụng? 

Đó là lúc bạn cần đến Sequelize - một ORM (Object-Relational Mapping) mạnh mẽ, giúp bạn tương tác với database một cách dễ dàng và hiệu quả. Trong bài viết này, chúng ta sẽ tìm hiểu về Sequelize và cách sử dụng nó để quản lý cơ sở dữ liệu trong ứng dụng của bạn."
```

Trong một số trường hợp nếu kiến thức quá cơ bản, thì có thể mở bài ngắn gọn bằng việc lý giải tầm quan trọng của kiến thức này đối với một số mô hình, ứng dụng...

```text wrap
ví dụ:
Arrow Function không phải chỉ là việc viết ngắn gọn cách khởi tạo 1 function để trông có vẻ "cool ngầu" và tiết kiệm được số dòng code. Việc hiểu rõ Arrow Functionc có thể giúp ích cho việc viết các hàm callback, vai trò của 'this', chaining... trong các framework như React và Next.js sau này.
```

### Diễn giải khái niệm

Diễn giải các khái niệm liên quan, chuẩn bị cho người đọc kiến thức cần thiết để hiểu được chủ đề đang viết.

- chỉ diễn giải ngắn gọn, súc tích, dễ hiểu, tránh dài dòng, phức tạp
- nếu khái niệm có vẻ phức tạp, dài dòng, dẫn liên kết đến một bài viết chi tiết khác đã từng viết trong repo này (nếu có)

```text wrap
ví dụ:
- Sequelize là một ORM (Object-Relational Mapping) cho Node.js, giúp bạn tương tác với cơ sở dữ liệu một cách dễ dàng và hiệu quả...
- ORM là một kỹ thuật lập trình cho phép bạn làm việc với cơ sở dữ liệu bằng cách sử dụng các đối tượng trong ngôn ngữ lập trình của bạn, thay vì phải viết các câu lệnh SQL phức tạp...
- Sequelize hỗ trợ nhiều loại cơ sở dữ liệu phổ biến như MySQL, PostgreSQL, SQLite và MSSQL...
- Sequelize có thể được cài đặt thông qua npm hoặc yarn, và có thể được sử dụng trong nhiều môi trường khác nhau như Node.js, Express, Koa, NestJS...
```

### Hướng dẫn chi tiết

bắt đầu đi vào hướng dẫn chi tiết, từng bước, trong đó:

- cần làm gì, sẽ diễn ra như thế nào, kết quả là gì
- cài đặt như thế nào, ở môi trường nào
- import hoặc cấu hình ra sao
- đưa ra code samples cơ bản nhất, tránh phức tạp hóa
- giải thích từng phần của code sample, tránh bỏ qua những chi tiết quan trọng

```text wrap
ví dụ:
- nếu diễn giải về Sequelize, chỉ cần đưa ra một Model phổ biến (Post), với một vài trường cơ bản (id, title, content, createdAt, updatedAt)
- không cần đến các trường phức tạp khác (excerpt, slug...) trừ phi cần diễn giải mối quan hệ giữa các trường đó
```

### Mở rộng, đào sâu, đi vào thực tế

Chỉ mở rộng, đào sâu ở những phần được xem là quan trọng, có tính chất liên kết các hướng dẫn và lý thuyết bên trên, và thường gặp trong những tình huống thực tế, edge-case...

```text wrap
ví dụ, nếu đang diễn giải về Sequelize, có thể mở rộng ở phần Types (DataTypes), để giải thích về các loại dữ liệu phổ biến (STRING, TEXT, INTEGER, BOOLEAN, DATE...)

ví dụ khác, nếu có các mối quan hệ giữa các bảng, có thể mở rộng ở phần Associations (hasOne, hasMany, belongsTo, belongsToMany) để giải thích cách thiết lập và sử dụng các mối quan hệ này
```

### Nhắc nhở các nguyên tắc (golden rules)

đưa ra các kinh nghiệm thực tiễn, nguyên tắc, lưu ý, do & don't, best practices, để giúp người đọc tránh những sai lầm phổ biến, và viết code chất lượng hơn

```text wrap
- ví dụ, nếu đang diễn giải về Sequelize, có thể đưa ra các nguyên tắc về cách đặt tên Model, cách tổ chức file, cách xử lý lỗi, cách tối ưu hiệu suất...
```

### Kết

kết thúc bài viết bằng một phần tóm tắt, nhấn mạnh những điểm chính đã trình bày

Gợi ý các stack liên quan mật thiết (`Express + Sequelize`), các bước tiếp theo (`Migration, Seeding...`), hoặc các chủ đề nâng cao hơn (`Transactions, Hooks, Scopes, Drizzle ORM...`).

## Yêu cầu chung

- viết bằng tiếng Việt
- dễ hiểu, thân thiện, gần gũi
- không nên quá dài, vừa đủ như một bài blog (tối đa 3,000 chữ)
- nếu dài quá, nên chia thành nhiều phần, hoặc viết thành series

```text wrap
ví dụ: Sequelize cơ bản (cài đặt và sử dụng), Sequelize nâng cao (mối quan hệ, migration, seeding), Sequelize chuyên sâu (transactions, hooks, scopes, Drizzle ORM...)
```