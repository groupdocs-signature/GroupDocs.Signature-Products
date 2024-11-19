



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:30
draft: false
lang: vi
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Ký PDF bằng chữ ký điện tử trong JavaScript"
head_description: "Khai thác khả năng của API JavaScript để ký số và bảo vệ các tệp PDF, bao gồm PDF, tài liệu Word, bảng tính Excel, bài thuyết trình và định dạng hình ảnh."

############################# Header ############################
title: "Ký tệp PDF điện tử" 
description: "Sử dụng GroupDocs.Signature for Node.js via Java để chèn nhiều chữ ký điện tử vào tài liệu của bạn, đảm bảo tính toàn vẹn dữ liệu và tuân thủ cho các tệp như PDF, Word, Excel, bài thuyết trình và định dạng hình ảnh."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống ngay miễn phí"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Tổng quan về API GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) cung cấp một bộ công cụ mạnh mẽ để thêm chữ ký điện tử. Với API trực quan của nó, bạn có thể dễ dàng ký, tìm kiếm, xác minh, chỉnh sửa và xóa chữ ký từ nhiều loại tệp mà không cần phần mềm bên ngoài. Nó hỗ trợ việc ký mượt mà các tệp PDF, tài liệu Word, bảng tính Excel, slide PowerPoint và nhiều định dạng hình ảnh.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước ký PDF bằng JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) đơn giản hóa quy trình thêm chữ ký tùy chỉnh vào các tệp PDF. Các nhà phát triển Node.js via Java có thể dễ dàng tích hợp chức năng ký vào ứng dụng của họ.
      
      1. Tải tài liệu PDF vào thể hiện Signature.
      2. Cấu hình SignOptions để xác định các thuộc tính của chữ ký.
      3. Điều chỉnh các thuộc tính như kích thước, màu sắc và nội dung khi cần.
      4. Lưu tài liệu đã ký ở vị trí chỉ định.
   
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

        // Nhập tài liệu vào một thể hiện Signature
        const signature = new signatureLib.Signature('input.pdf');

        // Khởi tạo một đối tượng QrCodeSignOptions
        const options = new signatureLib.QrCodeSignOptions('QR code text');
        
        // Xác định tất cả các tùy chọn cần thiết
        options.setLeft(100);
        options.setTop(100);
        options.setForeColor(new Color(255, 0, 0));

        // Lưu tài liệu đã ký vào ổ đĩa cục bộ
        signature.sign('output.pdf', options);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Khả năng chữ ký điện tử nâng cao"
  description: "API nâng cao của chúng tôi tối ưu hóa quy trình kinh doanh bằng cách tạo điều kiện cho việc ký, xác minh, chỉnh sửa và quản lý chữ ký điện tử tự động cho một loạt tài liệu."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "Tính năng chữ ký điện tử"
  features:
    # feature loop
    - title: "Ký điện tử cho các tệp văn phòng"
      content: "Thêm chữ ký điện tử vào bất kỳ trang nào hoặc vị trí nào trong tài liệu. Tùy chỉnh chữ ký của bạn với các lựa chọn như chứng chỉ số, siêu dữ liệu, mã vạch hoặc các yếu tố hình ảnh để tăng cường bảo mật và tính toàn vẹn của tài liệu."

    # feature loop
    - title: "Kiểm soát chữ ký toàn diện"
      content: "Khi một tài liệu đã được ký, bạn có thể quản lý các chữ ký của nó một cách dễ dàng. Lấy danh sách đầy đủ tất cả các chữ ký, cho phép bạn cập nhật hoặc xóa chúng khi cần."

    # feature loop
    - title: "Tăng cường bảo mật tài liệu"
      content: "Sử dụng chứng chỉ số để bảo vệ tài liệu của bạn khỏi việc sửa đổi. Bạn có thể nhúng hoặc trích xuất siêu dữ liệu để tăng cường khả năng truy xuất và kiểm toán, đảm bảo tuân thủ và tính xác thực của tài liệu."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cách áp dụng chữ ký hình ảnh vào tài liệu"
      content: |
        Hướng dẫn này chi tiết quy trình gắn chữ ký hình ảnh vào một trang chỉ định trong tài liệu.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
        
          // Cung cấp tài liệu nguồn dưới dạng tham số đầu vào
          const signature = new signatureLib.Signature('input.pdf');

          // Xác định đường dẫn tệp hình ảnh trong tùy chọn cấu hình chữ ký
          const options = new signatureLib.ImageSignOptions('image.jpg');

          // Cấu hình kích thước và xác định các trang mục tiêu cho chữ ký
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setHeight(150);
          options.setWidth(200);
          options.setMargin(new signatureLib.Padding(50));
          options.setAllPages(true);

          // Thực hiện áp dụng chữ ký vào tài liệu
          signature.sign('output.pdf', options);

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
            link: "/examples/signature/formats/signature_esign.pdf"
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
    title: "Xem những khả năng phong phú của chúng tôi"
    exclude: "esign"
    description: "Chúng tôi cung cấp nhiều loại chữ ký và các thao tác phong phú."
    items: 
          
        # operation loop 1
        - name: "Chữ ký điện tử"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "Thêm các loại chữ ký khác nhau vào các định dạng tệp được hỗ trợ"

        # operation loop 2
        - name: "Thêm văn bản vào tài liệu"
          operation: "text"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Nâng cao nội dung tài liệu với các chữ ký văn bản tùy chỉnh"

        # operation loop 3
        - name: "Chữ ký hình ảnh"
          operation: "image"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Đặt bất kỳ hình ảnh nào ở bất kỳ vị trí nào trong tài liệu"

        # operation loop 4
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Tạo và chèn các mã vạch khác nhau vào các tài liệu được hỗ trợ"

        # operation loop 5
        - name: "Tạo mã QR"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Tạo mã QR, bao gồm mã QR, để ký tài liệu"
          
        # operation loop 6
        - name: "Chứng chỉ số"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Bảo mật doanh nghiệp và ký các tài liệu bằng chứng chỉ số"

        # operation loop 7
        - name: "Chữ ký đóng dấu"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pdf/"
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
    title: "Ký số cho nhiều định dạng tệp"
    exclude: "PDF"
    description: "API Node.js via Java cho phép bạn áp dụng chữ ký điện tử cho hơn 60 định dạng tệp, cung cấp cho bạn sự linh hoạt lớn trong việc bảo mật các tài liệu quan trọng cho doanh nghiệp."
    items: 
          
        # format loop 1
        - name: "Ký điện tử PDF"
          format: "PDF"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Ký điện tử DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/esign/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Ký điện tử JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Ký điện tử PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/esign/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Ký điện tử XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---