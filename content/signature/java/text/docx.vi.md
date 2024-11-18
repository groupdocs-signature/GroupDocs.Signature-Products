



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:54
draft: false
lang: vi
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Tạo chữ ký văn bản DOCX với Java"
head_description: "Khai thác API Java để chèn chữ ký văn bản vào các tệp DOCX. Xử lý liền mạch các định dạng tài liệu phổ biến bao gồm PDF, Word, Excel, Bài thuyết trình, Hình ảnh và ZIP."

############################# Header ############################
title: "Tạo chữ ký văn bản cho DOCX" 
description: "Thêm chữ ký văn bản tùy chỉnh vào tài liệu kinh doanh của bạn bằng cách sử dụng GroupDocs.Signature for Java. Tối ưu hóa quy trình làm việc của tổ chức với các tùy chọn tùy chỉnh chữ ký."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Bắt đầu miễn phí"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Giới thiệu về giải pháp GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) cung cấp chữ ký văn bản linh hoạt và tùy chỉnh để đơn giản hóa các tác vụ quản lý tài liệu của bạn. Tùy chỉnh nội dung và thiết kế của chữ ký văn bản và áp dụng chúng vào bất kỳ trang nào, nâng cao quy trình làm việc tài liệu của tổ chức bạn.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước thêm chữ ký văn bản vào DOCX sử dụng Java"
    content: |
      [GroupDocs.Signature](/signature/java/) có thể được tích hợp vào các ứng dụng Java để thêm chữ ký văn bản vào tài liệu DOCX. Các nhà phát triển có thể nhanh chóng nâng cao chức năng sản phẩm của mình bằng cách sử dụng các giải pháp của chúng tôi.
      
      1. Sử dụng tài liệu DOCX làm tham số cho bộ dựng lớp Signature.
      2. Khởi tạo TextSignOptions với văn bản phù hợp.
      3. Cấu hình các tùy chọn hình thức cho chữ ký.
      4. Thêm chữ ký văn bản vào một hoặc nhiều trang của tài liệu.
   
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
        // Truyền đường dẫn tài liệu vào bộ dựng Signature
        Signature signature = new Signature("input.docx");

        // Khởi tạo TextSignOptions với văn bản chữ ký
        TextSignOptions options = new TextSignOptions("Approved");
        
        // Thiết lập màu sắc và thuộc tính phông chữ cho văn bản
        options.setForeColor(Color.RED);
        SignatureFont signatureFont = new SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName("Comic Sans MS");
        options.setFont(signatureFont);

        // Thêm chữ ký văn bản vào tài liệu
        SignResult result = signature.sign("output.docx", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Quản lý chữ ký văn bản tài liệu"
  description: "Với GroupDocs.Signature for Java, bạn có thể tối ưu hóa quy trình tài liệu của công ty bằng cách thêm chữ ký văn bản vào các định dạng tệp phổ biến. Dễ dàng cấu hình hình thức và nội dung của chữ ký."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Signature"
  features:
    # feature loop
    - title: "Chữ ký tài liệu"
      content: "Áp dụng chữ ký văn bản, hình ảnh, mã vạch, mã QR hoặc con dấu vào bất kỳ trang nào của tài liệu được hỗ trợ. Tận dụng siêu dữ liệu để nhúng nội dung ẩn và bảo mật tài liệu của bạn bằng các chứng chỉ kỹ thuật số."

    # feature loop
    - title: "Tìm kiếm và xác minh chữ ký"
      content: "Đảm bảo tính toàn vẹn của các tài liệu đã ký với công cụ xác minh chữ ký của chúng tôi. Bạn cũng có thể truy xuất và tìm kiếm tất cả các chữ ký được nhúng trong tài liệu."

    # feature loop
    - title: "Chỉnh sửa hoặc gỡ bỏ chữ ký"
      content: "Chỉnh sửa nội dung, vị trí và hình thức của các chữ ký đã thêm trước đó, hoặc gỡ bỏ chúng hoàn toàn khỏi tài liệu."

    # feature loop
    - title: "Chữ ký văn bản gốc"
      content: "Thêm các chữ ký văn bản cụ thể cho tài liệu, chẳng hạn như nhãn dán trong PDF hoặc hình mờ trong tài liệu Word, để tăng cường khả năng tùy chỉnh."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Đánh dấu tài liệu với chữ ký văn bản"
      content: |
        Tìm hiểu cách bổ sung thông tin văn bản vào tài liệu kinh doanh để cải thiện quy trình kinh doanh.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Chọn tài liệu để ký
          Signature signature = new Signature("input.docx");

          // Tạo tùy chọn văn bản với văn bản mong muốn
          TextSignOptions options = new TextSignOptions("Rescheduled to 03/04/2025");

          // Xác định kích thước và vị trí của chữ ký trên trang
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
          options.setHeight(30);

          // Chữ ký hỗ trợ khoảng đệm từ các góc trang.
          Padding padding = new Padding();
          padding.setBottom(20);
          padding.setRight(20);
          options.setMargin(padding);

          // Màu sắc và kiểu phông chữ có thể được tùy chỉnh.
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);

          // Chữ ký văn bản có thể bao gồm đường viền.
          Border border = new Border();
          border.setColor(Color.RED);
          border.setDashStyle(DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // Tùy chỉnh nền cũng có sẵn.
          Background background = new Background();
          background.setColor(Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // Văn bản có thể được lưu dưới dạng hình ảnh để bảo đảm tính tương thích.
          options.setSignatureImplementation(TextSignatureImplementation.Image);

          // Lưu tài liệu với chữ ký văn bản đã thêm.
          SignResult result = signature.sign("output.docx", options);
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
            link: "/examples/signature/formats/signature_text.docx"
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
    title: "Các tính năng chính và tùy chọn chữ ký"
    exclude: "text"
    description: "Giải pháp của chúng tôi hỗ trợ đầy đủ các thao tác CRUD và hơn thế nữa cho bảy loại chữ ký khác nhau."
    items: 
          
        # operation loop 1
        - name: "Chữ ký điện tử"
          operation: "esign"
          link: "/signature/java/esign/docx/"
          description: "Thêm các loại chữ ký khác nhau vào các định dạng tệp được hỗ trợ"

        # operation loop 2
        - name: "Thêm văn bản vào tài liệu"
          operation: "text"
          link: "/signature/java/text/docx/"
          description: "Nâng cao nội dung tài liệu với các chữ ký văn bản tùy chỉnh"

        # operation loop 3
        - name: "Chữ ký hình ảnh"
          operation: "image"
          link: "/signature/java/image/docx/"
          description: "Đặt bất kỳ hình ảnh nào ở bất kỳ vị trí nào trong tài liệu"

        # operation loop 4
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/signature/java/barcode/docx/"
          description: "Tạo và chèn các mã vạch khác nhau vào các tài liệu được hỗ trợ"

        # operation loop 5
        - name: "Tạo mã QR"
          operation: "qrcode"
          link: "/signature/java/qrcode/docx/"
          description: "Tạo mã QR, bao gồm mã QR, để ký tài liệu"
          
        # operation loop 6
        - name: "Chứng chỉ số"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "Bảo mật doanh nghiệp và ký các tài liệu bằng chứng chỉ số"

        # operation loop 7
        - name: "Chữ ký đóng dấu"
          operation: "stamp"
          link: "/signature/java/stamp/docx/"
          description: "Sử dụng Trình tạo đóng dấu để tạo các dấu tròn hoặc vuông tùy chỉnh"
          
        # operation loop 8
        - name: "Tìm kiếm chữ ký"
          operation: "search"
          link: "/signature/java/search/docx/"
          description: "Tìm bất kỳ chữ ký nào đã được thêm trước đó trong tài liệu"
          
        # operation loop 9
        - name: "Xác minh chữ ký"
          operation: "verify"
          link: "/signature/java/verify/docx/"
          description: "Xác minh tính xác thực của chữ ký sau khi đã được áp dụng"
          
        # operation loop 10
        - name: "Chỉnh sửa chữ ký"
          operation: "modify"
          link: "/signature/java/modify/docx/"
          description: "Chỉnh sửa dễ dàng nhiều loại chữ ký trong một tài liệu"
          
        # operation loop 11
        - name: "Xóa chữ ký"
          operation: "delete"
          link: "/signature/java/delete/docx/"
          description: "Xóa một loạt các chữ ký đã được áp dụng trước đó"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Thêm chữ ký văn bản vào các định dạng tệp khác nhau"
    exclude: "DOCX"
    description: "Sử dụng API Java để chèn chữ ký văn bản vào tài liệu Office, đảm bảo kiểm soát hoàn toàn nội dung ở mọi giai đoạn trong vòng đời của tài liệu."
    items: 
          
        # format loop 1
        - name: "Chữ ký văn bản PDF"
          format: "PDF"
          link: "/signature/java/text/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Chữ ký văn bản DOCX"
          format: "DOCX"
          link: "/signature/java/text/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Chữ ký văn bản JPEG"
          format: "JPEG"
          link: "/signature/java/text/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Chữ ký văn bản PPTX"
          format: "PPTX"
          link: "/signature/java/text/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Chữ ký văn bản XLSX"
          format: "XLSX"
          link: "/signature/java/text/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---