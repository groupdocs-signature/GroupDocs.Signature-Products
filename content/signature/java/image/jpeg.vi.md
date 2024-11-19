



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:09
draft: false
lang: vi
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Thêm chữ ký hình ảnh vào tệp JPEG bằng Java"
head_description: "Đặt chữ ký hình ảnh trên tệp JPEG cho Java bằng vài dòng mã. Sử dụng API GroupDocs.Signature for Java để thêm hình ảnh."

############################# Header ############################
title: "Ký tệp JPEG với chữ ký hình ảnh" 
description: "Sử dụng GroupDocs.Signature for Java để chèn hình ảnh vào nhiều định dạng tài liệu văn phòng khác nhau, bao gồm PDF, Word, Excel và các tệp hình ảnh. Một hình ảnh với chữ ký của sếp có thể tạo ấn tượng thú vị!"
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải về miễn phí"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Khám phá GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) cung cấp khả năng thêm chữ ký hình ảnh vào bất kỳ trang và vị trí nào trong các tài liệu kinh doanh. Tối ưu hóa quy trình làm việc của bạn bằng cách thêm hình ảnh vào PDF, tài liệu Word, bảng tính Excel, bài thuyết trình PowerPoint và các định dạng hình ảnh phổ biến.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước thêm hình ảnh vào bất kỳ vị trí nào trong tệp JPEG qua Java"
    content: |
      [GroupDocs.Signature](/signature/java/) nâng cao ứng dụng Java với khả năng thêm chữ ký vào bất kỳ trang nào của tài liệu JPEG một cách chính xác. Tăng cường chức năng sản phẩm của bạn bằng cách tích hợp thư viện của chúng tôi.
      
      1. Tạo một thể hiện của Signature với tài liệu JPEG.
      2. Sử dụng ImageSignOptions để chỉ định hình ảnh chữ ký.
      3. Đặt hình ảnh ở bất kỳ vị trí nào trên bất kỳ trang nào.
      4. Lưu tài liệu đã ký vào một vị trí mới.
   
    code:
      platform: "java"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Chữ ký mẫu"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "nhấp để sao chép"
        copy_done: "đã sao chép"
      links:
        #  loop
        - title: "Thêm ví dụ"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "Tài liệu hướng dẫn"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // Khởi tạo Signature với đường dẫn tài liệu
        Signature signature = new Signature("input.jpeg");

        // Tạo ImageSignOptions với hình ảnh cho chữ ký
        ImageSignOptions options = new ImageSignOptions("company_logo.jpg");

        // Đặt hình ảnh ở góc trên bên trái của tất cả các trang
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);

        // Lưu tài liệu đã ký
        SignResult result = signature.sign("output.jpeg", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Giải pháp ký tài liệu toàn diện"
  description: "API của chúng tôi hỗ trợ nhiều tính năng ký, cho phép bạn thêm, sửa đổi, xóa, tìm kiếm và xác minh nhiều loại chữ ký khác nhau, bao gồm cả chữ ký hình ảnh."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Ký hình ảnh"
  features:
    # feature loop
    - title: "Chèn hình ảnh vào tài liệu văn phòng"
      content: "Đặt chữ ký hình ảnh vào bất kỳ vị trí nào trên bất kỳ trang nào của tài liệu. Tăng cường nội dung của bạn với văn bản, hình ảnh, mã vạch, siêu dữ liệu và chứng chỉ số."

    # feature loop
    - title: "Tìm kiếm và xác minh chữ ký"
      content: "Xác minh dễ dàng tính hợp lệ của chữ ký trong các tài liệu đã ký. Lấy danh sách tất cả các chữ ký trong một tài liệu và kiểm tra thông tin chi tiết về từng chữ ký."

    # feature loop
    - title: "Sửa đổi chữ ký"
      content: "Cập nhật nội dung, diện mạo, kích thước hoặc vị trí của bất kỳ chữ ký nào đã được thêm vào tài liệu. API của chúng tôi giúp việc sửa đổi chữ ký trở nên đơn giản và hiệu quả."

    # feature loop
    - title: "Xóa chữ ký không cần thiết"
      content: "API của chúng tôi hỗ trợ các thao tác CRUD đầy đủ cho hầu hết các loại chữ ký. Bạn có thể dễ dàng xóa chữ ký khỏi hầu hết các loại tài liệu được hỗ trợ khi cần thiết."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Nâng cao nội dung tài liệu với chữ ký hình ảnh"
      content: |
        Tìm hiểu cách thêm hình ảnh vào tài liệu kinh doanh để cung cấp thêm thông tin.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Chọn tài liệu cần ký
          Signature signature = new Signature("input.jpeg");

          // Tạo tùy chọn hình ảnh với đường dẫn đến hình ảnh
          ImageSignOptions options = new ImageSignOptions("manager_signature.jpg");

          // Đặt kích thước cho chữ ký hình ảnh
          options.setWidth(100);
          options.setHeight(100);

          // Đặt hình ảnh ở góc dưới bên phải
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);

          // Áp dụng khoảng cách từ các góc trang nếu cần
          Padding padding = new Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // Thêm viền tùy chỉnh cho hình ảnh nếu muốn
          Border border = new Border();
          border.setColor(Color.RED);
          border.setDashStyle(DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // Xoay chữ ký để căn chỉnh tốt hơn
          options.setRotationAngle(45);

          // Lưu tài liệu đã cập nhật tại bất kỳ vị trí nào
          SignResult result = signature.sign("output.jpeg", options);

          ```
        platform: "java"
        copy_title: "Sao chép"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "nhấp để sao chép"
          copy_done: "đã sao chép"
        top_links:
          #  loop
          - title: "Tải xuống kết quả"
            icon: "download"
            link: "/examples/signature/formats/signature_image.jpeg"
        links:
          #  loop
          - title: "Thêm ví dụ"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Tài liệu hướng dẫn"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Sẵn sàng bắt đầu? "
  description: "Dùng thử các tính năng của GroupDocs.Signature miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "Tải xuống Maven"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "Giấy phép"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Hãy xem các tính năng hàng đầu của chúng tôi"
    exclude: "image"
    description: "Chúng tôi rất vui được giới thiệu nhiều công cụ và thao tác ký khác nhau."
    items: 
          
        # operation loop 1
        - name: "Chữ ký điện tử"
          operation: "esign"
          link: "/signature/java/esign/jpeg/"
          description: "Thêm các loại chữ ký khác nhau vào các định dạng tệp được hỗ trợ"

        # operation loop 2
        - name: "Thêm văn bản vào tài liệu"
          operation: "text"
          link: "/signature/java/text/jpeg/"
          description: "Nâng cao nội dung tài liệu với các chữ ký văn bản tùy chỉnh"

        # operation loop 3
        - name: "Chữ ký hình ảnh"
          operation: "image"
          link: "/signature/java/image/jpeg/"
          description: "Đặt bất kỳ hình ảnh nào ở bất kỳ vị trí nào trong tài liệu"

        # operation loop 4
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/signature/java/barcode/jpeg/"
          description: "Tạo và chèn các mã vạch khác nhau vào các tài liệu được hỗ trợ"

        # operation loop 5
        - name: "Tạo mã QR"
          operation: "qrcode"
          link: "/signature/java/qrcode/jpeg/"
          description: "Tạo mã QR, bao gồm mã QR, để ký tài liệu"
          
        # operation loop 6
        - name: "Chứng chỉ số"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "Bảo mật doanh nghiệp và ký các tài liệu bằng chứng chỉ số"

        # operation loop 7
        - name: "Chữ ký đóng dấu"
          operation: "stamp"
          link: "/signature/java/stamp/jpeg/"
          description: "Sử dụng Trình tạo đóng dấu để tạo các dấu tròn hoặc vuông tùy chỉnh"
          
        # operation loop 8
        - name: "Tìm kiếm chữ ký"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "Tìm bất kỳ chữ ký nào đã được thêm trước đó trong tài liệu"
          
        # operation loop 9
        - name: "Xác minh chữ ký"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "Xác minh tính xác thực của chữ ký sau khi đã được áp dụng"
          
        # operation loop 10
        - name: "Chỉnh sửa chữ ký"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "Chỉnh sửa dễ dàng nhiều loại chữ ký trong một tài liệu"
          
        # operation loop 11
        - name: "Xóa chữ ký"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "Xóa một loạt các chữ ký đã được áp dụng trước đó"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Thêm hình ảnh vào các định dạng tệp khác"
    exclude: "JPEG"
    description: "Với API Java, bạn có thể chèn các định dạng hình ảnh được hỗ trợ vào nhiều tài liệu khác nhau. Dễ dàng thay đổi kích thước, chọn vị trí và thêm chữ ký hình ảnh vào tài liệu của bạn."
    items: 
          
        # format loop 1
        - name: "Ký PDF bằng hình ảnh"
          format: "PDF"
          link: "/signature/java/image/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Ký DOCX bằng hình ảnh"
          format: "DOCX"
          link: "/signature/java/image/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Ký JPEG bằng hình ảnh"
          format: "JPEG"
          link: "/signature/java/image/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Ký PPTX bằng hình ảnh"
          format: "PPTX"
          link: "/signature/java/image/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Ký XLSX bằng hình ảnh"
          format: "XLSX"
          link: "/signature/java/image/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---