



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:05
draft: false
lang: vi
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Thêm mã vạch vào tệp DOCX bằng Java"
head_description: "Tạo và chèn chữ ký mã vạch vào tài liệu DOCX trong Java. GroupDocs.Signature cho phép tích hợp chữ ký linh hoạt cho nhiều định dạng."

############################# Header ############################
title: "Tạo mã vạch cho DOCX" 
description: "Thêm mã vạch của các định dạng phổ biến vào bất kỳ vị trí nào trong tài liệu của bạn với GroupDocs.Signature for Java. Giải pháp của chúng tôi cung cấp nhiều tùy chọn để tùy chỉnh chữ ký mã vạch."
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
       [GroupDocs.Signature for Java](/signature/java/) là một giải pháp ký tiên tiến hỗ trợ nhiều loại chữ ký khác nhau. Bạn có thể ký tài liệu với văn bản, hình ảnh, mã vạch, chứng chỉ số, dấu xác nhận và nhiều hơn nữa trên hơn 60 định dạng tệp, bao gồm PDF, MS Office, hình ảnh, tệp ZIP và các định dạng phổ biến khác trong kinh doanh. Ngoài ra, chữ ký trong các tài liệu đã ký có thể được tìm kiếm, xác minh, sửa đổi hoặc xóa bất cứ lúc nào.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước để tạo và thêm một mã vạch vào tệp DOCX"
    content: |
      [GroupDocs.Signature](/signature/java/) có thể tạo mã vạch ở nhiều định dạng phổ biến và đặt chúng trên các trang DOCX. Với hỗ trợ cho hơn 60 loại mã vạch, ứng dụng Java có thể dễ dàng được nâng cao với các khả năng ký mã vạch bằng cách tích hợp thư viện của chúng tôi.
      
      1. Cung cấp tệp DOCX hoặc luồng để được xử lý.
      2. Chuyển văn bản mã vạch cho thể hiện BarcodeSignOptions.
      3. Tùy chỉnh các tùy chọn mã vạch như vị trí, kích thước, v.v.
      4. Lưu tệp với mã vạch mới được thêm vào.
   
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
        // Tạo một thể hiện mới của Signature với đường dẫn tài liệu
        Signature signature = new Signature("input.docx");

        // Sử dụng BarcodeSignOptions để thêm một mã vạch vào tài liệu
        BarcodeSignOptions options = new BarcodeSignOptions("Business data");

        // Thiết lập loại mã vạch và các thuộc tính khác
        options.setEncodeType(BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);

        // Lưu tệp đã ký
        signature.sign("output.docx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Cải thiện hoặc bảo vệ nội dung tài liệu với chữ ký"
  description: "Thư viện GroupDocs.Signature for Java được thiết kế để ký và xử lý các định dạng tệp phổ biến. Nhanh chóng và linh hoạt thêm, sửa đổi, xác minh hoặc xóa nhiều loại chữ ký khác nhau."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Các tính năng của GroupDocs.Signature"
  features:
    # feature loop
    - title: "Ký tài liệu"
      content: "Ký bất kỳ trang nào của tài liệu được hỗ trợ với văn bản, hình ảnh, mã vạch, mã QR hoặc dấu xác nhận. Thêm siêu dữ liệu ẩn như EXIF trong hình ảnh hoặc bảo vệ nội dung tài liệu khỏi các thay đổi trái phép bằng cách sử dụng chứng chỉ số."

    # feature loop
    - title: "Tìm kiếm và xác minh chữ ký"
      content: "Bạn có thể thực hiện nhiều thao tác với tài liệu đã ký. Chúng tôi cung cấp dịch vụ xác minh chữ ký để đảm bảo mọi thứ đều đúng. Ngoài ra, bạn có thể lấy danh sách tất cả chữ ký của tài liệu thông qua tìm kiếm."

    # feature loop
    - title: "Sửa đổi chữ ký"
      content: "Hầu hết các chữ ký đã thêm trước đó có thể được sửa đổi. Dễ dàng chỉnh sửa văn bản, điều chỉnh vị trí hoặc thay đổi màu sắc."

    # feature loop
    - title: "Xóa chữ ký"
      content: "Giải pháp của chúng tôi hỗ trợ các hoạt động CRUD đầy đủ cho chữ ký. Nhiều loại chữ ký có thể được xóa khỏi tài liệu khi cần thiết."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cách tạo một chữ ký mã vạch"
      content: |
        Ví dụ này minh họa cách đặt một mã vạch tùy chỉnh lên các trang tài liệu DOCX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Cung cấp tài liệu cần được ký
          Signature signature = new Signature("input.docx");

          // Tạo các tùy chọn chữ ký với văn bản mong muốn
          BarcodeSignOptions signOptions = new BarcodeSignOptions("Accepted");
          signOptions.setEncodeType(BarcodeTypes.Code39FullASCII);

          // Thiết lập vị trí mã vạch tương đối trên trang
          signOptions.setVerticalAlignment(VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Left);

          // Thiết lập khoảng cách mã vạch từ cạnh trang
          Padding padding = new Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // Thiết lập màu sắc của các thanh
          signOptions.setForeColor(Color.RED);

          // Định nghĩa kiểu font chữ cho thông điệp
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Arial");
          signOptions.setFont(font);

          // Xác định vị trí thông điệp
          signOptions.setCodeTextAlignment(CodeTextAlignment.Above);

          // Ký và lưu tài liệu
          SignResult signResult = signature.sign("output.docx", signOptions);

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
            link: "/examples/signature/formats/signature_barcode.docx"
        links:
          #  loop
          - title: "Thêm ví dụ"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Tài liệu hướng dẫn"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################## Actions ############################

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
    title: "Khám phá các khả năng cốt lõi của chúng tôi"
    exclude: "barcode"
    description: "Chúng tôi tự hào giới thiệu một loạt chữ ký và chức năng được hỗ trợ đa dạng."
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
    title: "Ký tài liệu ở định dạng khác"
    exclude: "DOCX"
    description: "Hơn 60 định dạng có thể được ký sử dụng API Java của chúng tôi. Áp dụng nhiều chữ ký khác nhau vào bất kỳ trang hoặc vị trí nào trong tài liệu."
    items: 
          
        # format loop 1
        - name: "Thêm mã vạch vào PDF"
          format: "PDF"
          link: "/signature/java/barcode/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Thêm mã vạch vào DOCX"
          format: "DOCX"
          link: "/signature/java/barcode/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Thêm mã vạch vào JPEG"
          format: "JPEG"
          link: "/signature/java/barcode/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Thêm mã vạch vào PPTX"
          format: "PPTX"
          link: "/signature/java/barcode/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Thêm mã vạch vào XLSX"
          format: "XLSX"
          link: "/signature/java/barcode/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---