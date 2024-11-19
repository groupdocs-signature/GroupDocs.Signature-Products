



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:06
draft: false
lang: vi
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Tạo và thêm dấu vào PPTX qua JavaScript"
head_description: "Tận dụng sức mạnh của GroupDocs.Signature và JavaScript để tạo và đặt dấu tùy chỉnh trên bất kỳ trang nào trong tài liệu PPTX của bạn."

############################# Header ############################
title: "Chèn dấu tùy chỉnh vào tệp PPTX" 
description: "Sử dụng GroupDocs.Signature for Node.js via Java để tạo dấu được căn chỉnh và chèn chúng vào bất kỳ vị trí nào trong tài liệu của bạn. Nền tảng của chúng tôi cung cấp nhiều tùy chọn để cá nhân hóa dấu theo yêu cầu kinh doanh cụ thể của bạn."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Dùng thử miễn phí"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java là gì?"
    link: "/signature/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) cung cấp một giải pháp mạnh mẽ và linh hoạt cho việc ký tài liệu. Nó cho phép người dùng thêm dấu và các loại chữ ký khác nhau qua hơn 60 định dạng khác nhau, như PDF, Word, Excel, tệp hình ảnh và tệp ZIP. Nền tảng này cho phép bạn chèn chữ, hình ảnh, mã vạch, mã QR, siêu dữ liệu, chứng chỉ số và chữ ký dấu. Ngoài việc ký, bạn có thể tìm kiếm, xác minh, sửa đổi hoặc xóa bất kỳ chữ ký nào có trong tài liệu của bạn.

############################# Steps ############################
steps:
    enable: true
    title: "Hướng dẫn chèn dấu vào PPTX sử dụng JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) cung cấp một công cụ mạnh mẽ cho việc tạo và nhúng dấu, có thể nâng cao đáng kể các ứng dụng Node.js via Java. Sử dụng tính năng này để tạo và áp dụng các dấu tùy chỉnh cho các trang tài liệu của bạn.
      
      1. Nhập tài liệu PPTX cần chèn dấu.
      2. Triển khai StampSignOptions để định nghĩa tất cả các tham số cần thiết.
      3. Chèn bao nhiêu dòng dấu tùy ý.
      4. Áp dụng dấu và lưu tài liệu cuối cùng.
   
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

        // Liên kết đường dẫn tài liệu với phiên bản Signature
        const signature = new signatureLib.Signature('input.pptx');

        // Tạo StampSignOptions với nội dung chữ ký cần thiết
        const options = new signatureLib.StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // Kết hợp một hoặc nhiều dòng dấu
        const outerLine = new signatureLib.StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(signatureLib.Color.WHITE);
        outerLine.setBackgroundColor(signatureLib.Color.BLUE);
        options.getOuterLines().add(outerLine);

        // Lưu tài liệu với dấu đã áp dụng
        const result = signature.sign('output.pptx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tăng cường an ninh tài liệu bằng chữ ký"
  description: "Với GroupDocs.Signature for Node.js via Java, bạn có thể thêm, chỉnh sửa, xác thực hoặc xóa dấu và các loại chữ ký khác trong tất cả các định dạng tài liệu phổ biến. API đơn giản hóa quy trình quản lý chữ ký để cải thiện tính toàn vẹn và tùy chỉnh của tài liệu."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Các tính năng của GroupDocs.Signature"
  features:
    # feature loop
    - title: "Ký tài liệu tùy chỉnh"
      content: "Áp dụng các chữ ký như văn bản, hình ảnh, mã vạch, mã QR và dấu vào bất kỳ phần nào của tài liệu của bạn. Công cụ này cũng cho phép bao gồm siêu dữ liệu ẩn và chứng chỉ số để bảo vệ nội dung của bạn khỏi những thay đổi trái phép."

    # feature loop
    - title: "Tìm và xác minh chữ ký"
      content: "Sau khi tài liệu đã được ký, hãy sử dụng hệ thống xác minh của chúng tôi để đảm bảo tính toàn vẹn của các chữ ký. Thêm vào đó, nền tảng của chúng tôi cho phép bạn tìm kiếm và lấy thông tin chi tiết về tất cả các chữ ký được áp dụng cho một tài liệu."

    # feature loop
    - title: "Sửa đổi chữ ký khi cần thiết"
      content: "Điều chỉnh và cập nhật các chữ ký đã áp dụng trước đó một cách hiệu quả. Dù thay đổi nội dung, màu sắc, kích thước hay vị trí của chữ ký, GroupDocs.Signature for Node.js via Java cung cấp các tùy chọn tùy chỉnh đầy đủ."

    # feature loop
    - title: "Xóa chữ ký không cần thiết"
      content: "Dễ dàng xóa bất kỳ chữ ký nào không cần thiết khỏi tài liệu của bạn. API của chúng tôi hỗ trợ việc xóa nhiều loại chữ ký, bao gồm dấu và chứng chỉ số, mang đến cho bạn sự linh hoạt hoàn toàn trong việc quản lý tài liệu."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Nhúng dấu tùy chỉnh vào tài liệu"
      content: |
        Tìm hiểu cách thiết kế và áp dụng các dấu tùy chỉnh chứa văn bản quan trọng vào tài liệu của bạn.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Cung cấp tài liệu để chèn dấu
          const signature = new signatureLib.Signature('input.pptx');

          // Thiết lập tùy chọn dấu với các cấu hình mong muốn
          const options = new signatureLib.StampSignOptions();

          // Xác định kích thước và vị trí của dấu trên trang
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setAllPages(true);

          // Bao gồm các đường tròn bên ngoài với văn bản tùy chỉnh
          const outerLine1 = new signatureLib.StampLine();
          outerLine1.setText('* The best  choice *');
          outerLine1.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
          const signatureFont1 = new signatureLib.SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName('Arial');
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(signatureLib.Color.WHITE);
          outerLine1.setBackgroundColor(signatureLib.Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // Thêm các đường vuông bên trong nếu cần
          const innerLine1 = new signatureLib.StampLine();
          innerLine1.setText('Company #1');
          innerLine1.setTextColor(signatureLib.Color.RED);
          const signFont1 = new signatureLib.SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);
          
          // Lưu tài liệu đã được chèn dấu
          const result = signature.sign('output.pptx', options);
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
            link: "/examples/signature/formats/signature_stamp.pptx"
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
    title: "Khám phá các tính năng chính"
    exclude: "stamp"
    description: "Giải pháp của chúng tôi cung cấp nhiều công cụ để tạo, quản lý và xóa các loại chữ ký khác nhau, mang đến cho người dùng quyền kiểm soát hoàn toàn đối với quy trình làm việc của tài liệu."
    items: 
          
        # operation loop 1
        - name: "Chữ ký điện tử"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pptx/"
          description: "Thêm các loại chữ ký khác nhau vào các định dạng tệp được hỗ trợ"

        # operation loop 2
        - name: "Thêm văn bản vào tài liệu"
          operation: "text"
          link: "/signature/nodejs-java/text/pptx/"
          description: "Nâng cao nội dung tài liệu với các chữ ký văn bản tùy chỉnh"

        # operation loop 3
        - name: "Chữ ký hình ảnh"
          operation: "image"
          link: "/signature/nodejs-java/image/pptx/"
          description: "Đặt bất kỳ hình ảnh nào ở bất kỳ vị trí nào trong tài liệu"

        # operation loop 4
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "Tạo và chèn các mã vạch khác nhau vào các tài liệu được hỗ trợ"

        # operation loop 5
        - name: "Tạo mã QR"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "Tạo mã QR, bao gồm mã QR, để ký tài liệu"
          
        # operation loop 6
        - name: "Chứng chỉ số"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "Bảo mật doanh nghiệp và ký các tài liệu bằng chứng chỉ số"

        # operation loop 7
        - name: "Chữ ký đóng dấu"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pptx/"
          description: "Sử dụng Trình tạo đóng dấu để tạo các dấu tròn hoặc vuông tùy chỉnh"
          
        # operation loop 8
        - name: "Tìm kiếm chữ ký"
          operation: "search"
          link: "/signature/nodejs-java/search/pptx/"
          description: "Tìm bất kỳ chữ ký nào đã được thêm trước đó trong tài liệu"
          
        # operation loop 9
        - name: "Xác minh chữ ký"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pptx/"
          description: "Xác minh tính xác thực của chữ ký sau khi đã được áp dụng"
          
        # operation loop 10
        - name: "Chỉnh sửa chữ ký"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pptx/"
          description: "Chỉnh sửa dễ dàng nhiều loại chữ ký trong một tài liệu"
          
        # operation loop 11
        - name: "Xóa chữ ký"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pptx/"
          description: "Xóa một loạt các chữ ký đã được áp dụng trước đó"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Áp dụng chữ ký dấu trên nhiều loại tệp"
    exclude: "PPTX"
    description: "API GroupDocs.Signature hỗ trợ chữ ký dấu qua 60+ định dạng tệp, cho phép người dùng đặt dấu tùy chỉnh trên bất kỳ trang hoặc khu vực nào, cải thiện khả năng truy cập và an ninh của tài liệu."
    items: 
          
        # format loop 1
        - name: "Đóng dấu PDF"
          format: "PDF"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Đóng dấu DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Đóng dấu JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Đóng dấu PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/stamp/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Đóng dấu XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---