



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:52
draft: false
lang: vi
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Thêm chữ ký hình ảnh vào tệp DOCX bằng JavaScript"
head_description: "Đặt chữ ký hình ảnh trên tệp DOCX cho Node.js bằng một vài dòng mã. Sử dụng API GroupDocs.Signature for Node.js via Java để thêm hình ảnh."

############################# Header ############################
title: "Ký tệp DOCX bằng chữ ký hình ảnh" 
description: "Tận dụng khả năng của GroupDocs.Signature for Node.js via Java để nhúng hình ảnh vào nhiều định dạng tài liệu văn phòng như PDF, Word, Excel và nhiều định dạng hình ảnh khác. Việc thêm hình ảnh chữ ký lãnh đạo có thể nâng cao tính chuyên nghiệp và độ tin cậy của tài liệu của bạn, tạo nên một bài trình bày tinh tế và hoàn hảo."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống miễn phí"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Giới thiệu về GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) cho phép người dùng thêm chữ ký hình ảnh tại bất kỳ vị trí nào trong tài liệu của bạn. Công cụ này giúp doanh nghiệp đơn giản hóa quy trình làm việc bằng cách thêm hình ảnh vào PDF, Word, Excel, PowerPoint và các định dạng hình ảnh phổ biến, nâng cao hiệu quả quản lý tài liệu.

############################# Steps ############################
steps:
    enable: true
    title: "Hướng dẫn thêm hình ảnh vào DOCX bằng JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) giúp các ứng dụng Node.js via Java tích hợp chữ ký hình ảnh vào tài liệu DOCX một cách liền mạch. Nâng cao khả năng của ứng dụng bạn với thư viện toàn diện của chúng tôi.
      
      1. Khởi tạo Signature với tài liệu DOCX
      2. Sử dụng ImageSignOptions để chỉ định hình ảnh chữ ký
      3. Đặt hình ảnh chính xác ở bất kỳ trang nào
      4. Lưu tài liệu đã ký vào vị trí mong muốn
   
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

        // Khởi tạo Signature với đường dẫn tới tài liệu
        const signature = new signatureLib.Signature('input.docx');

        // Cấu hình ImageSignOptions để bao gồm chữ ký hình ảnh mong muốn
        const options = new signatureLib.ImageSignOptions('company_logo.jpg');

        // Đặt hình ảnh ở góc trên bên trái trên tất cả các trang
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);
        
        // Lưu tài liệu với chữ ký hình ảnh đã áp dụng
        const result = signature.sign('output.docx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Khả năng ký tài liệu nâng cao"
  description: "API của chúng tôi cung cấp một bộ tính năng giúp đơn giản hóa việc ký điện tử. Bạn có thể thêm, chỉnh sửa, xóa, tìm kiếm và xác thực nhiều loại chữ ký khác nhau, bao gồm cả chữ ký hình ảnh."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Chữ ký hình ảnh"
  features:
    # feature loop
    - title: "Kết hợp hình ảnh vào tài liệu văn phòng"
      content: "Đặt chữ ký hình ảnh ở bất kỳ đâu trong tài liệu của bạn, cho dù là PDF, Word hay Excel. Nâng cao tài liệu của bạn bằng cách thêm hình ảnh, mã vạch, siêu dữ liệu hoặc chứng chỉ số để tăng thêm chức năng."

    # feature loop
    - title: "Tìm kiếm và xác thực chữ ký"
      content: "Đảm bảo tính xác thực của tài liệu đã ký bằng cách xác thực chữ ký. Sử dụng chức năng tìm kiếm để truy xuất và xem tất cả các chữ ký được nhúng trong tài liệu của bạn."

    # feature loop
    - title: "Chỉnh sửa chữ ký hiện có"
      content: "API của chúng tôi cho phép người dùng cập nhật và điều chỉnh chữ ký khi cần. Chỉnh sửa kích thước, vị trí hoặc các thuộc tính khác của bất kỳ chữ ký nào đã được thêm trước đó để có sự linh hoạt trong việc xử lý tài liệu."

    # feature loop
    - title: "Xóa chữ ký không cần thiết"
      content: "Quản lý tài liệu của bạn một cách hiệu quả bằng cách xóa các chữ ký không còn cần thiết. API của chúng tôi hỗ trợ các thao tác CRUD hoàn chỉnh cho hầu hết tất cả các loại chữ ký."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Nâng cao tài liệu với chữ ký hình ảnh"
      content: |
        Tìm hiểu cách kết hợp hình ảnh vào tài liệu kinh doanh để thêm thông tin bổ sung.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Chọn tài liệu cần được ký
          const signature = new signatureLib.Signature('input.docx');

          // Cấu hình tùy chọn hình ảnh với đường dẫn đến hình ảnh
          const options = new signatureLib.ImageSignOptions('manager_signature.jpg');

          // Điều chỉnh kích thước của chữ ký hình ảnh
          options.setWidth(100);
          options.setHeight(100);

          // Đặt hình ảnh ở góc dưới bên phải
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Áp dụng khoảng đệm từ các góc trang nếu cần
          const padding = new signatureLib.Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // Tùy chọn, thêm viền tùy chỉnh cho hình ảnh
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // Xoay chữ ký hình ảnh cho ngoại hình tối ưu
          options.setRotationAngle(45);

          // Lưu tài liệu đã cập nhật vào vị trí mong muốn
          const result = signature.sign('output.docx', options);
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
            link: "/examples/signature/formats/signature_image.docx"
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
    title: "Khám phá các chức năng chúng tôi cung cấp"
    exclude: "image"
    description: "Chúng tôi tự hào giới thiệu một loạt các phương thức và thao tác chữ ký."
    items: 
          
        # operation loop 1
        - name: "Chữ ký điện tử"
          operation: "esign"
          link: "/signature/nodejs-java/esign/docx/"
          description: "Thêm các loại chữ ký khác nhau vào các định dạng tệp được hỗ trợ"

        # operation loop 2
        - name: "Thêm văn bản vào tài liệu"
          operation: "text"
          link: "/signature/nodejs-java/text/docx/"
          description: "Nâng cao nội dung tài liệu với các chữ ký văn bản tùy chỉnh"

        # operation loop 3
        - name: "Chữ ký hình ảnh"
          operation: "image"
          link: "/signature/nodejs-java/image/docx/"
          description: "Đặt bất kỳ hình ảnh nào ở bất kỳ vị trí nào trong tài liệu"

        # operation loop 4
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "Tạo và chèn các mã vạch khác nhau vào các tài liệu được hỗ trợ"

        # operation loop 5
        - name: "Tạo mã QR"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Tạo mã QR, bao gồm mã QR, để ký tài liệu"
          
        # operation loop 6
        - name: "Chứng chỉ số"
          operation: "digital"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Bảo mật doanh nghiệp và ký các tài liệu bằng chứng chỉ số"

        # operation loop 7
        - name: "Chữ ký đóng dấu"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "Sử dụng Trình tạo đóng dấu để tạo các dấu tròn hoặc vuông tùy chỉnh"
          
        # operation loop 8
        - name: "Tìm kiếm chữ ký"
          operation: "search"
          link: "/signature/nodejs-java/search/docx/"
          description: "Tìm bất kỳ chữ ký nào đã được thêm trước đó trong tài liệu"
          
        # operation loop 9
        - name: "Xác minh chữ ký"
          operation: "verify"
          link: "/signature/nodejs-java/verify/docx/"
          description: "Xác minh tính xác thực của chữ ký sau khi đã được áp dụng"
          
        # operation loop 10
        - name: "Chỉnh sửa chữ ký"
          operation: "modify"
          link: "/signature/nodejs-java/modify/docx/"
          description: "Chỉnh sửa dễ dàng nhiều loại chữ ký trong một tài liệu"
          
        # operation loop 11
        - name: "Xóa chữ ký"
          operation: "delete"
          link: "/signature/nodejs-java/delete/docx/"
          description: "Xóa một loạt các chữ ký đã được áp dụng trước đó"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Thêm hình ảnh vào nhiều loại tệp khác nhau"
    exclude: "DOCX"
    description: "API Node.js via Java cho phép bạn nhúng hình ảnh vào một loạt các định dạng tài liệu. Tùy chỉnh kích thước, vị trí và định dạng trang để nâng cao quy trình ký tài liệu của bạn."
    items: 
          
        # format loop 1
        - name: "Ký PDF bằng hình ảnh"
          format: "PDF"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Ký DOCX bằng hình ảnh"
          format: "DOCX"
          link: "/signature/nodejs-java/image/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Ký JPEG bằng hình ảnh"
          format: "JPEG"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Ký PPTX bằng hình ảnh"
          format: "PPTX"
          link: "/signature/nodejs-java/image/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Ký XLSX bằng hình ảnh"
          format: "XLSX"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---