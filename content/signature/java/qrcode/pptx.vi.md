



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:01
draft: false
lang: vi
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Tạo mã QR cho PPTX bằng Java"
head_description: "API GroupDocs.Signature cho phép tạo mã QR cho các tệp PPTX. Tạo mã QR từ nội dung của bạn và đặt chúng trên bất kỳ trang nào."

############################# Header ############################
title: "Tạo mã QR cho PPTX" 
description: "Tạo mã vạch 2D với dữ liệu văn bản và số và đặt chúng trên bất kỳ trang nào của nhiều tài liệu khác nhau bằng cách sử dụng GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Dùng thử miễn phí"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Tìm hiểu thêm về GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) cung cấp nhiều tính năng để tạo và nhúng nhiều loại chữ ký trong tất cả các định dạng tài liệu chính. Nó hỗ trợ các tệp PDF, tài liệu Word, bảng tính Excel, bài thuyết trình PowerPoint và hình ảnh. Nâng cao tài liệu của bạn với chữ ký văn bản, hình ảnh, mã vạch, mã QR, siêu dữ liệu, chữ ký số và chữ ký con dấu.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước để tạo và đặt mã QR tại bất kỳ vị trí nào trong PPTX"
    content: |
      [GroupDocs.Signature](/signature/java/) có thể tạo mã QR trong nhiều định dạng phổ biến và đặt chúng trên các trang PPTX. Hơn 10 loại mã QR được hỗ trợ và có thể nhanh chóng tích hợp vào các ứng dụng Java. Sử dụng sản phẩm của chúng tôi để ký tài liệu với mã QR đã tạo.
      
      1. Lấy tệp hoặc luồng PPTX cần ký bằng mã QR.
      2. Cung cấp văn bản cho QrCodeSignOptions.
      3. Tùy chỉnh các tùy chọn hiển thị như màu sắc, vị trí, kích thước, v.v.
      4. Lưu tệp với mã QR.
   
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
        // Truyền tài liệu vào một thể hiện mới của Signature
        Signature signature = new Signature("input.pptx");

        // Sử dụng QrCodeSignOptions để thêm mã QR vào tài liệu
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // Chỉ định loại chữ ký và vị trí trên trang
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // Lưu tệp với mã QR đã thêm
        signature.sign("output.pptx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Thêm chữ ký vào tài liệu của bạn"
  description: "API GroupDocs.Signature for Java hỗ trợ ký tất cả các định dạng tệp phổ biến. Tạo, sửa đổi, tìm kiếm, xác thực và xóa các loại chữ ký khác nhau."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Tính năng chính của GroupDocs.Signature"
  features:
    # feature loop
    - title: "Ký tài liệu"
      content: "GroupDocs.Signature hỗ trợ ký với chữ ký văn bản, hình ảnh, mã vạch, mã QR và chữ ký con dấu. Đặt chúng trên bất kỳ trang nào của bất kỳ định dạng tài liệu được hỗ trợ nào. Quản lý siêu dữ liệu tài liệu với chữ ký siêu dữ liệu và bảo vệ nội dung khỏi các thay đổi trái phép bằng cách sử dụng chứng thư số."

    # feature loop
    - title: "Tìm kiếm và xác thực"
      content: "Đảm bảo rằng tất cả chữ ký trong tài liệu đều hợp lệ qua quy trình xác thực. Truy xuất danh sách hoàn chỉnh các chữ ký trong tài liệu bằng cách sử dụng tính năng tìm kiếm tích hợp."

    # feature loop
    - title: "Sửa đổi chữ ký"
      content: "Dễ dàng sửa đổi thuộc tính chữ ký sau khi ký. Điều chỉnh nội dung, vị trí, màu sắc, kích thước và các thuộc tính khác khi cần."

    # feature loop
    - title: "Xóa chữ ký"
      content: "Xóa các chữ ký không mong muốn một cách dễ dàng. Nhiều loại chữ ký, bao gồm chứng thư số, có thể bị xóa lập trình từ tài liệu."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cách tùy chỉnh mã QR được tạo"
      content: |
        Sử dụng ví dụ này để tìm hiểu cách đặt một mã QR mới trên trang PPTX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Lấy tài liệu cần ký và truyền nó vào Signature
          Signature signature = new Signature("input.pptx");

          // Sử dụng tùy chọn mã QR để cung cấp văn bản với thông tin cần thiết
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // Đặt vị trí tương đối của mã QR trên trang
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // Đặt khoảng cách chữ ký
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Chỉ định màu sắc cho mã QR
          signOptions.setForeColor(Color.RED);

          // Xác định các tùy chọn phông chữ cho thông điệp
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Tùy chỉnh màu nền và cọ cho mã QR
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Thêm mã QR vào tài liệu
          SignResult signResult = signature.sign("output.pptx", signOptions);
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
            link: "/examples/signature/formats/signature_qrcode.pptx"
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
    title: "Khám phá các dịch vụ chính của chúng tôi"
    exclude: "qrcode"
    description: "Chúng tôi cung cấp một lựa chọn đa dạng các tính năng chữ ký và các thao tác nâng cao."
    items: 
          
        # operation loop 1
        - name: "Chữ ký điện tử"
          operation: "esign"
          link: "/signature/java/esign/pptx/"
          description: "Thêm các loại chữ ký khác nhau vào các định dạng tệp được hỗ trợ"

        # operation loop 2
        - name: "Thêm văn bản vào tài liệu"
          operation: "text"
          link: "/signature/java/text/pptx/"
          description: "Nâng cao nội dung tài liệu với các chữ ký văn bản tùy chỉnh"

        # operation loop 3
        - name: "Chữ ký hình ảnh"
          operation: "image"
          link: "/signature/java/image/pptx/"
          description: "Đặt bất kỳ hình ảnh nào ở bất kỳ vị trí nào trong tài liệu"

        # operation loop 4
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/signature/java/barcode/pptx/"
          description: "Tạo và chèn các mã vạch khác nhau vào các tài liệu được hỗ trợ"

        # operation loop 5
        - name: "Tạo mã QR"
          operation: "qrcode"
          link: "/signature/java/qrcode/pptx/"
          description: "Tạo mã QR, bao gồm mã QR, để ký tài liệu"
          
        # operation loop 6
        - name: "Chứng chỉ số"
          operation: "digital"
          link: "/signature/java/digital/pptx/"
          description: "Bảo mật doanh nghiệp và ký các tài liệu bằng chứng chỉ số"

        # operation loop 7
        - name: "Chữ ký đóng dấu"
          operation: "stamp"
          link: "/signature/java/stamp/pptx/"
          description: "Sử dụng Trình tạo đóng dấu để tạo các dấu tròn hoặc vuông tùy chỉnh"
          
        # operation loop 8
        - name: "Tìm kiếm chữ ký"
          operation: "search"
          link: "/signature/java/search/pptx/"
          description: "Tìm bất kỳ chữ ký nào đã được thêm trước đó trong tài liệu"
          
        # operation loop 9
        - name: "Xác minh chữ ký"
          operation: "verify"
          link: "/signature/java/verify/pptx/"
          description: "Xác minh tính xác thực của chữ ký sau khi đã được áp dụng"
          
        # operation loop 10
        - name: "Chỉnh sửa chữ ký"
          operation: "modify"
          link: "/signature/java/modify/pptx/"
          description: "Chỉnh sửa dễ dàng nhiều loại chữ ký trong một tài liệu"
          
        # operation loop 11
        - name: "Xóa chữ ký"
          operation: "delete"
          link: "/signature/java/delete/pptx/"
          description: "Xóa một loạt các chữ ký đã được áp dụng trước đó"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tạo mã QR cho các định dạng tệp bổ sung"
    exclude: "PPTX"
    description: "Nâng cao tất cả các định dạng tệp phổ biến với mã QR được tạo bằng API Java. Thêm dữ liệu mã vạch 2D để quét và xử lý dễ dàng."
    items: 
          
        # format loop 1
        - name: "Mã QR cho PDF"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Mã QR cho DOCX"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Mã QR cho JPEG"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Mã QR cho PPTX"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Mã QR cho XLSX"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---