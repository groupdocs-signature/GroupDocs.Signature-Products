



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:16
draft: false
lang: vi
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Thêm chữ ký điện tử vào file DOCX bằng Java"
head_description: "Đặt chữ ký điện tử trên file DOCX bằng Java chỉ với vài dòng mã. Sử dụng GroupDocs.Signature for Java để ký nhiều định dạng file khác nhau."

############################# Header ############################
title: "Ký DOCX với chữ ký điện tử" 
description: "Bảo vệ nội dung tài liệu kinh doanh của bạn bằng cách niêm phong chúng với chứng chỉ điện tử thông qua các tính năng của GroupDocs.Signature for Java. Chúng tôi cung cấp nhiều cách để đánh dấu và bảo mật tài liệu của bạn."
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
    title: "Về GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) là một giải pháp ký kết toàn diện hỗ trợ nhiều loại xử lý tài liệu. Bạn có thể thêm văn bản, hình ảnh, chứng chỉ điện tử và con dấu vào các file ở hơn 60 định dạng, bao gồm PDF, MS Office, hình ảnh, file ZIP, và các định dạng kinh doanh phổ biến khác. Hơn nữa, các tài liệu đã ký có thể được tìm kiếm, xác minh, sửa đổi hoặc xóa tự động một cách thuận tiện.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước bảo vệ DOCX bằng chứng chỉ điện tử trong Java"
    content: |
      [GroupDocs.Signature](/signature/java/) cho phép các nhà phát triển Java ngăn chặn các thay đổi trong tài liệu DOCX bằng cách sử dụng chữ ký điện tử. Tăng cường ứng dụng doanh nghiệp của bạn với khả năng bảo vệ dữ liệu quan trọng.
      
      1. Truyền tài liệu DOCX vào constructor của lớp Signature.
      2. Sử dụng một chứng chỉ điện tử và mật khẩu của nó để bảo vệ tài liệu.
      3. Tùy chọn, thêm đại diện hình ảnh cho chữ ký điện tử trên các trang tài liệu.
      4. Ký tài liệu để ngăn chặn bất kỳ thay đổi nào trong tương lai.
   
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
        // Sử dụng Signature với tài liệu để ký điện tử
        Signature signature = new Signature("input.docx");

        // Cung cấp một chứng chỉ điện tử và mật khẩu
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Thiết lập đại diện hình ảnh nếu cần thiết
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);

        // Bảo vệ tài liệu với chứng chỉ điện tử
        SignResult result = signature.sign("output.docx", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Cải thiện hoặc bảo vệ nội dung tài liệu với chữ ký"
  description: "Thư viện GroupDocs.Signature for Java có khả năng ký tất cả các định dạng file phổ biến. Thêm, sửa đổi, xác minh hoặc xóa các loại chữ ký khác nhau một cách tự động để tối ưu hóa quy trình kinh doanh của bạn."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Các tính năng của GroupDocs.Signature"
  features:
    # feature loop
    - title: "Thêm chữ ký vào tài liệu"
      content: "Chữ ký Văn bản, Hình ảnh, Mã vạch, QR-Code, hoặc Con dấu có thể được thêm chính xác vào bất kỳ trang nào của bất kỳ tài liệu hỗ trợ nào. Siêu dữ liệu ẩn như EXIF có thể được thêm hoặc chỉnh sửa trong hình ảnh và hầu hết các loại file. Bảo vệ nội dung tài liệu khỏi những thay đổi trái phép bằng cách sử dụng chữ ký điện tử."

    # feature loop
    - title: "Tìm kiếm và xác minh chữ ký"
      content: "Tài liệu có thể được xử lý theo nhiều cách khác nhau sau khi ký. Xác minh tài liệu đã ký để đảm bảo chúng đã được xử lý đúng cách. Nếu bạn cần kiểm soát nhiều hơn, bạn có thể lấy danh sách tất cả các chữ ký thông qua tìm kiếm."

    # feature loop
    - title: "Chỉnh sửa chữ ký"
      content: "Hầu hết các loại chữ ký đều hỗ trợ chỉnh sửa thêm. Bạn có thể sửa văn bản, thay đổi vị trí, màu sắc, kích thước, và nhiều hơn nữa."

    # feature loop
    - title: "Xóa những chữ ký không cần thiết"
      content: "Giải pháp của chúng tôi hỗ trợ đầy đủ các hoạt động CRUD cho chữ ký. Nhiều loại chữ ký, bao gồm cả chứng chỉ điện tử, có thể bị xóa khỏi tài liệu khi cần thiết."
      
  code_samples:
    # code sample loop
    - title: "Bảo vệ tài liệu bằng chữ ký điện tử"
      content: |
        Tìm hiểu cách bảo vệ tài liệu khỏi các thay đổi bằng cách sử dụng chữ ký điện tử.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Cung cấp một tài liệu để ký
        Signature signature = new Signature("input.docx");

        // Sử dụng một chứng chỉ điện tử hợp lệ với mật khẩu
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Chỉ định dữ liệu văn bản bổ sung
        options.setReason("Security issue");
        options.setContact("John Smith");
        options.setLocation("Office D.W.");

        // Sử dụng hình ảnh và các tùy chọn khác cho đại diện hình ảnh
        options.setImageFilePath("image.png");

        options.setAllPages(true);
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        Padding padding = new Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);

        // Lưu tài liệu đã bảo vệ vào một vị trí khác
        SignResult result = signature.sign("output.docx", options);
        ```
        {{< /landing/code >}}


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
    title: "Khám phá bộ tính năng toàn diện của chúng tôi"
    exclude: "digital"
    description: "Chúng tôi tự hào về sự đa dạng chức năng và hỗ trợ chữ ký mà nền tảng của chúng tôi cung cấp."
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
    title: "Ký tài liệu ở các định dạng khác"
    exclude: "DOCX"
    description: "API Java cho phép bạn xử lý hơn 60 định dạng. Tạo và thêm nhiều chữ ký vào bất kỳ trang nào, niêm phong nội dung bằng chứng chỉ điện tử, và quản lý cùng chỉnh sửa các chữ ký hiện có trong tài liệu."
    items: 
          
        # format loop 1
        - name: "Bảo vệ PDF"
          format: "PDF"
          link: "/signature/java/digital/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Bảo vệ DOCX"
          format: "DOCX"
          link: "/signature/java/digital/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Bảo vệ PPTX"
          format: "PPTX"
          link: "/signature/java/digital/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 4
        - name: "Bảo vệ XLSX"
          format: "XLSX"
          link: "/signature/java/digital/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---