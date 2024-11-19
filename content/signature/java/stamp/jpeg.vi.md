



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:05
draft: false
lang: vi
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Thêm dấu đóng vào JPEG bằng Java"
head_description: "Tận dụng GroupDocs.Signature và Java để tạo các dấu đóng tùy chỉnh và đặt chúng trên bất kỳ trang nào trong tài liệu JPEG."

############################# Header ############################
title: "Thêm dấu đóng tùy chỉnh vào JPEG" 
description: "Thiết kế và áp dụng dấu đóng tròn hoặc vuông cho bất kỳ phần nào của tài liệu bạn bằng GroupDocs.Signature for Java. Giải pháp của chúng tôi cung cấp nhiều tùy chọn tùy chỉnh để đáp ứng mọi nhu cầu kinh doanh của bạn."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống miễn phí"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Giới thiệu về GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) là một công cụ mạnh mẽ cho phép bạn thêm nhiều kiểu chữ ký đóng vào tài liệu. Nó hỗ trợ hơn 60 định dạng file khác nhau, bao gồm PDF, Word, Excel, hình ảnh và tệp ZIP. Bạn có thể áp dụng chữ ký văn bản, hình ảnh, mã vạch, siêu dữ liệu, chứng chỉ số và chữ ký đóng. Ngoài việc thêm chữ ký, bạn có thể tìm kiếm, xác minh, sửa đổi và loại bỏ chúng.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước để thêm dấu đóng vào JPEG qua Java"
    content: |
      [GroupDocs.Signature](/signature/java/) cung cấp một bộ tạo dấu đóng có thể hữu ích cho các ứng dụng Java. Sử dụng nó để tạo ra các dấu đóng được tùy chỉnh tốt cho các trang tài liệu của bạn.
      
      1. Cung cấp tài liệu JPEG cần được đóng dấu.
      2. Sử dụng StampSignOptions để cấu hình tất cả các tham số cần thiết.
      3. Thêm bao nhiêu dòng tùy thích.
      4. Áp dụng dấu đóng và lưu tài liệu.
   
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
        // Sử dụng đường dẫn tài liệu với đối tượng Signature
        Signature signature = new Signature("input.jpeg");

        // Khởi tạo StampSignOptions với nội dung chữ ký mong muốn
        StampSignOptions options = new StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // Thêm một hoặc nhiều dòng dấu đóng
        StampLine outerLine = new StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(Color.WHITE);
        outerLine.setBackgroundColor(Color.BLUE);
        options.getOuterLines().add(outerLine);

        // Lưu tài liệu đã đóng dấu
        SignResult result = signature.sign("output.jpeg", options);
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "Bảo vệ nội dung tài liệu của bạn bằng chữ ký"
  description: "Thư viện GroupDocs.Signature for Java được thiết kế để ký và quản lý chữ ký trên các định dạng file phổ biến. Dễ dàng thêm, sửa đổi, xác minh hoặc loại bỏ dấu đóng và các loại chữ ký khác."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Chữ ký dấu đóng với GroupDocs.Signature"
  features:
    # feature loop
    - title: "Ký tài liệu của bạn"
      content: "Áp dụng chữ ký tùy chỉnh cho bất kỳ phần nào trong tài liệu của bạn. Lựa chọn từ nhiều loại chữ ký, bao gồm văn bản, hình ảnh, mã vạch, mã QR và dấu đóng. Bên cạnh đó, có thể thêm hoặc sửa đổi siêu dữ liệu ẩn để tăng cường bảo mật tài liệu."

    # feature loop
    - title: "Tìm kiếm và xác minh chữ ký"
      content: "Khi tài liệu đã được ký, hãy sử dụng công cụ xác minh của chúng tôi để đảm bảo nội dung chữ ký hợp lệ. Tìm kiếm và lấy danh sách tất cả các chữ ký để xử lý thêm."

    # feature loop
    - title: "Cập nhật chữ ký khi cần"
      content: "Sửa đổi nhiều loại chữ ký đã áp dụng vào một tài liệu. Cập nhật các thuộc tính như kích thước, màu sắc, vị trí, nội dung và hơn thế nữa."

    # feature loop
    - title: "Xóa chữ ký"
      content: "Cần xóa chữ ký khỏi tài liệu? API của chúng tôi hoàn toàn hỗ trợ việc xóa chữ ký, giúp bạn quản lý tài liệu một cách hiệu quả."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Thêm dấu đóng tùy chỉnh vào tài liệu bằng chữ ký đặc biệt"
      content: |
        Tìm hiểu cách tạo và thêm dấu đóng tùy chỉnh với thông tin văn bản quan trọng vào tài liệu của bạn.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Cung cấp tài liệu cần đóng dấu
          Signature signature = new Signature("input.jpeg");

          // Khởi tạo đối tượng tùy chọn dấu đóng
          StampSignOptions options = new StampSignOptions();

          // Đặt kích thước và vị trí trên trang
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setAllPages(true);

          // Thêm một hoặc nhiều đường tròn ngoài với văn bản
          StampLine outerLine1 = new StampLine();
          outerLine1.setText("* The best  choice *");
          outerLine1.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
          SignatureFont signatureFont1 = new SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName("Arial");
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(Color.WHITE);
          outerLine1.setBackgroundColor(Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // Thêm một hoặc nhiều đường vuông bên trong
          StampLine innerLine1 = new StampLine();
          innerLine1.setText("Company #1");
          innerLine1.setTextColor(Color.RED);
          SignatureFont signFont1 = new SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);

          // Lưu tài liệu đã đóng dấu
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
            link: "/examples/signature/formats/signature_stamp.jpeg"
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
    title: "Khám phá các tính năng chính của chúng tôi"
    exclude: "stamp"
    description: "Sử dụng nhiều tùy chọn để thêm, quản lý và xóa chữ ký."
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
    title: "Thêm dấu đóng trên nhiều định dạng file"
    exclude: "JPEG"
    description: "API GroupDocs.Signature hỗ trợ đóng dấu trên hơn 60 định dạng. Đặt dấu trên bất kỳ trang hoặc khu vực nào để cải thiện quản lý tài liệu và tùy chỉnh."
    items: 
          
        # format loop 1
        - name: "Đóng dấu PDF"
          format: "PDF"
          link: "/signature/java/stamp/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Đóng dấu DOCX"
          format: "DOCX"
          link: "/signature/java/stamp/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Đóng dấu JPEG"
          format: "JPEG"
          link: "/signature/java/stamp/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Đóng dấu PPTX"
          format: "PPTX"
          link: "/signature/java/stamp/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Đóng dấu XLSX"
          format: "XLSX"
          link: "/signature/java/stamp/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---