



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:56
draft: false
lang: vi
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Thêm chữ ký văn bản vào JPEG qua JavaScript"
head_description: "Sử dụng API JavaScript để tích hợp mượt mà chữ ký văn bản vào tài liệu JPEG. API của chúng tôi hỗ trợ một loạt các định dạng, bao gồm PDF, Word, Excel, Bài thuyết trình, Hình ảnh, và tệp ZIP."

############################# Header ############################
title: "Thêm chữ ký văn bản vào JPEG" 
description: "Kết hợp chữ ký văn bản cá nhân hóa vào các tệp công việc của bạn với GroupDocs.Signature for Node.js via Java. Kiểm soát quy trình tài liệu của bạn bằng cách nâng cao chúng với các tùy chọn chữ ký bảo mật và tùy chỉnh."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Bắt đầu dùng thử miễn phí"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Giới thiệu về GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) là giải pháp sáng tạo được thiết kế để hỗ trợ việc thêm chữ ký văn bản vào tài liệu. Tùy chỉnh và đặt chữ ký trên bất kỳ trang nào, nâng cao hiệu quả trong việc xử lý tài liệu. Tinh giản quy trình làm việc của tổ chức bạn bằng cách tích hợp các ký hiệu văn bản cá nhân hóa, nâng cao cả chức năng và tính chuyên nghiệp.

############################# Steps ############################
steps:
    enable: true
    title: "Hướng dẫn tạo chữ ký văn bản cho JPEG bằng JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) cho phép thêm chữ ký văn bản vào tài liệu JPEG trong các ứng dụng Node.js via Java. Nhanh chóng nâng cao khả năng của sản phẩm với các giải pháp mạnh mẽ của chúng tôi.
      
      1. Cung cấp tài liệu JPEG như một đối số cho lớp Signature.
      2. Khởi tạo TextSignOptions với nội dung văn bản cần thiết.
      3. Thiết lập các thuộc tính trực quan của chữ ký văn bản.
      4. Thêm chữ ký văn bản vào trang mong muốn của tài liệu.
   
    code:
      platform: "nodejs-java"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Chữ ký mẫu"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "nhấp để sao chép"
        copy_done: "đã sao chép"
      links:
        #  loop
        - title: "Thêm ví dụ"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "Tài liệu hướng dẫn"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // Khởi tạo lớp Signature với đường dẫn tài liệu
        const signature = new signatureLib.Signature('input.jpeg');

        // Tạo TextSignOptions với nội dung chữ ký cần thiết
        const options = new signatureLib.TextSignOptions('Approved');

        // Cấu hình màu sắc văn bản và thuộc tính phông chữ
        options.setForeColor(new signatureLib.Color(255, 0, 0));
        const signatureFont = new signatureLib.SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName('Comic Sans MS');
        options.setFont(signatureFont);
        
        // Thêm chữ ký văn bản vào tài liệu
        const result = signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Kiểm soát chữ ký văn bản nâng cao"
  description: "Với GroupDocs.Signature for Node.js via Java, bạn có thể cải thiện đáng kể việc quản lý chữ ký dựa trên văn bản trong các định dạng tài liệu chính. Công cụ này cho phép bạn cấu hình kiểu dáng, vị trí và nội dung của chữ ký một cách hiệu quả, cho phép các doanh nghiệp tùy chỉnh các quy trình tài liệu của mình."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Signature"
  features:
    # feature loop
    - title: "Chữ ký tài liệu động"
      content: "Chèn nhiều loại chữ ký—như văn bản, hình ảnh, mã vạch, mã QR hoặc con dấu—trên bất kỳ trang nào của tài liệu được hỗ trợ. Nhúng siêu dữ liệu để truyền tải thông tin ẩn hoặc áp dụng chứng chỉ số để tăng cường biện pháp bảo mật."

    # feature loop
    - title: "Tìm kiếm và xác thực chữ ký"
      content: "Xác minh tính xác thực của các chữ ký nhúng trong tài liệu của bạn. Thực hiện tìm kiếm hiệu quả để xác định tất cả các trường hợp chữ ký, đảm bảo việc theo dõi và quản lý tài liệu một cách toàn diện."

    # feature loop
    - title: "Chỉnh sửa hoặc xóa chữ ký"
      content: "Sửa đổi hoặc xóa các chữ ký đã thêm trước đó khi cần. Bạn có thể điều chỉnh diện mạo, vị trí hoặc nội dung của bất kỳ chữ ký nào để đáp ứng các yêu cầu đang thay đổi, đảm bảo tính linh hoạt trong việc xử lý tài liệu."

    # feature loop
    - title: "Tùy chỉnh chữ ký bản địa"
      content: "Đối với một số loại tệp, điều chỉnh vị trí chữ ký với các tính năng tài liệu tích hợp, chẳng hạn như thêm dấu hiệu vào tệp Word hoặc con dấu tùy chỉnh vào PDF, nâng cao tính độc đáo của các tài liệu của bạn."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Triển khai chữ ký văn bản trong tài liệu"
      content: |
        Tìm hiểu cách nhúng chữ ký văn bản vào tài liệu kinh doanh để tối ưu hóa quy trình.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Chọn tài liệu sẽ được ký
          const signature = new signatureLib.Signature('input.jpeg');

          // Xác định các tùy chọn văn bản với nội dung đã chỉ định
          const options = new signatureLib.TextSignOptions('Rescheduled to 03/04/2025');

          // Đặt kích thước và vị trí của chữ ký trên trang
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
          options.setHeight(30);

          // Áp dụng khoảng cách cho chữ ký từ các cạnh của trang
          const padding = new signatureLib.Padding();
          padding.setBottom(20);
          padding.setRight(20);
          options.setMargin(padding);

          // Tùy chỉnh màu chữ và kiểu phông chữ
          options.setForeColor(signatureLib.Color.RED);
          const signatureFont = new signatureLib.SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName('Comic Sans MS');
          options.setFont(signatureFont);

          // Thêm viền cho chữ ký văn bản nếu cần
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // Cấu hình nền cho chữ ký
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // Tùy chọn, lưu chữ ký văn bản dưới dạng hình ảnh để tương thích
          options.setSignatureImplementation(signatureLib.TextSignatureImplementation.Image);
          
          // Lưu tài liệu với chữ ký văn bản đã thêm
          const result = signature.sign('output.jpeg', options);
          ```
        platform: "nodejs-java"
        copy_title: "Sao chép"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "nhấp để sao chép"
          copy_done: "đã sao chép"
        top_links:
          #  loop
          - title: "Tải xuống kết quả"
            icon: "download"
            link: "/examples/signature/formats/signature_text.jpeg"
        links:
          #  loop
          - title: "Thêm ví dụ"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "Tài liệu hướng dẫn"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Sẵn sàng bắt đầu? "
  description: "Dùng thử các tính năng của GroupDocs.Signature miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "Tải xuống NPM"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "Giấy phép"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Các tính năng quản lý chữ ký toàn diện"
    exclude: "text"
    description: "Nền tảng của chúng tôi cung cấp đầy đủ các thao tác CRUD và các tính năng nâng cao cho việc quản lý bảy loại chữ ký khác nhau, cho phép bạn quản lý chữ ký tài liệu của mình một cách chính xác và hiệu quả."
    items: 
          
        # operation loop 1
        - name: "Chữ ký điện tử"
          operation: "esign"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "Thêm các loại chữ ký khác nhau vào các định dạng tệp được hỗ trợ"

        # operation loop 2
        - name: "Thêm văn bản vào tài liệu"
          operation: "text"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "Nâng cao nội dung tài liệu với các chữ ký văn bản tùy chỉnh"

        # operation loop 3
        - name: "Chữ ký hình ảnh"
          operation: "image"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "Đặt bất kỳ hình ảnh nào ở bất kỳ vị trí nào trong tài liệu"

        # operation loop 4
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "Tạo và chèn các mã vạch khác nhau vào các tài liệu được hỗ trợ"

        # operation loop 5
        - name: "Tạo mã QR"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "Tạo mã QR, bao gồm mã QR, để ký tài liệu"
          
        # operation loop 6
        - name: "Chứng chỉ số"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Bảo mật doanh nghiệp và ký các tài liệu bằng chứng chỉ số"

        # operation loop 7
        - name: "Chữ ký đóng dấu"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "Sử dụng Trình tạo đóng dấu để tạo các dấu tròn hoặc vuông tùy chỉnh"
          
        # operation loop 8
        - name: "Tìm kiếm chữ ký"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Tìm bất kỳ chữ ký nào đã được thêm trước đó trong tài liệu"
          
        # operation loop 9
        - name: "Xác minh chữ ký"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Xác minh tính xác thực của chữ ký sau khi đã được áp dụng"
          
        # operation loop 10
        - name: "Chỉnh sửa chữ ký"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "Chỉnh sửa dễ dàng nhiều loại chữ ký trong một tài liệu"
          
        # operation loop 11
        - name: "Xóa chữ ký"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "Xóa một loạt các chữ ký đã được áp dụng trước đó"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Áp dụng chữ ký văn bản trên nhiều định dạng khác nhau"
    exclude: "JPEG"
    description: "Khám phá khả năng của API Node.js via Java để tích hợp chữ ký dựa trên văn bản vào một loạt các định dạng Office. Kiểm soát dòng chảy thông tin tại mỗi giai đoạn của vòng đời tài liệu bằng cách thêm các dấu văn bản có thể tùy chỉnh."
    items: 
          
        # format loop 1
        - name: "Chữ ký văn bản PDF"
          format: "PDF"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Chữ ký văn bản DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/text/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Chữ ký văn bản JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Chữ ký văn bản PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/text/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Chữ ký văn bản XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---