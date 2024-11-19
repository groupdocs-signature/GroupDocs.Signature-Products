



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:22
draft: false
lang: vi
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Tạo mã QR trong tài liệu PDF với JavaScript"
head_description: "Sử dụng API GroupDocs.Signature để tạo và tích hợp mã vạch 2D vào các tệp PDF. Đặt mã QR một cách linh hoạt trên bất kỳ trang tài liệu nào."

############################# Header ############################
title: "Tạo mã QR cho PDF" 
description: "Tạo và nhúng mã vạch 2D với nội dung tùy chỉnh, bao gồm văn bản và dữ liệu số, trên nhiều loại tài liệu khác nhau như PDF, Word, Excel và Hình ảnh với GroupDocs.Signature for Node.js via Java."
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
    title: "Khám phá khả năng của GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) cung cấp các công cụ nâng cao tài liệu, cho phép tạo và nhúng nhiều loại chữ ký, trong đó có mã QR, vào các định dạng tệp phổ biến. Ký và bảo mật các tệp PDF, tài liệu Word, bảng tính Excel, bài thuyết trình PowerPoint và hình ảnh với Chữ ký Văn bản, Hình ảnh, Mã vạch, Mã QR, Siêu dữ liệu, Chữ ký Điện tử và Dấu.

############################# Steps ############################
steps:
    enable: true
    title: "Hướng dẫn tạo và nhúng mã QR vào bất kỳ vị trí nào trong PDF"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) cho phép tạo mã QR trong nhiều định dạng phổ biến và tích hợp chúng vào các trang PDF. Hỗ trợ hơn 10 loại mã QR khác nhau, giải pháp của chúng tôi có thể được tích hợp liền mạch vào các ứng dụng Node.js via Java, làm phong phú thêm khả năng ký mã QR.
      
      1. Cung cấp tệp PDF hoặc luồng để ký mã QR.
      2. Nhập văn bản mong muốn vào thể hiện QrCodeSignOptions.
      3. Điều chỉnh các cài đặt trực quan như màu sắc, vị trí, kích thước, v.v.
      4. Lưu tài liệu chứa mã QR.
   
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

        // Tạo một thể hiện Signature và truyền đường dẫn tài liệu
        const signature = new signatureLib.Signature('input.pdf');

        // Sử dụng QrCodeSignOptions để chèn mã QR vào tài liệu
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // Xác định loại chữ ký và vị trí trên trang
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // Lưu tài liệu với mã QR mới được thêm vào
        signature.sign('output.pdf', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tích hợp chữ ký và mã QR toàn diện"
  description: "Với API GroupDocs.Signature for Node.js via Java, bạn có thể quản lý toàn bộ các loại chữ ký. Tạo, tùy chỉnh, xác minh, tìm kiếm và xóa chữ ký một cách linh hoạt trên nhiều loại tài liệu khác nhau, mang lại khả năng linh hoạt chưa từng có cho quy trình làm việc của bạn."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Các tính năng chữ ký và mã QR"
  features:
    # feature loop
    - title: "Ký tài liệu đa định dạng"
      content: "Thêm nhiều loại chữ ký, bao gồm Chữ ký Văn bản, Hình ảnh, Mã vạch, Mã QR và Dấu vào bất kỳ định dạng tài liệu nào được hỗ trợ. Đặt chúng trên bất kỳ trang nào và quản lý siêu dữ liệu tài liệu. Đảm bảo an ninh tài liệu thông qua các chứng chỉ số để ngăn chặn các thay đổi không được phép."

    # feature loop
    - title: "Xác minh chữ ký hiệu quả"
      content: "Xác minh tất cả các chữ ký trong tài liệu để đảm bảo chúng đáp ứng các tiêu chuẩn yêu cầu. Dễ dàng lấy và xem xét các chữ ký qua chức năng tìm kiếm tích hợp."

    # feature loop
    - title: "Chỉnh sửa chữ ký linh hoạt"
      content: "Cập nhật hoặc thay đổi chữ ký hiện có, điều chỉnh các yếu tố như nội dung, vị trí, kích thước và màu sắc để phù hợp với yêu cầu của tài liệu sau khi ký."

    # feature loop
    - title: "Xóa chữ ký thật đơn giản"
      content: "Xóa bất kỳ chữ ký không mong muốn hoặc lỗi thời nào, bao gồm cả chứng chỉ số, một cách dễ dàng. Quản lý chữ ký hoàn toàn mang lại một tài liệu sạch sẽ và gọn gàng."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tùy chỉnh mã QR được tạo ra"
      content: |
        Ví dụ này chi tiết quy trình thêm mã QR tùy chỉnh vào một trang PDF.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Lấy tài liệu cần ký và truyền nó cho Signature
          const signature = new signatureLib.Signature('input.pdf');

          // Thiết lập các tùy chọn mã QR với văn bản cần thiết
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // Xác định vị trí của mã QR trên trang
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Chỉ định khoảng cách chữ ký
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Chọn màu sắc cho mã QR
          signOptions.setForeColor(signatureLib.Color.RED);

          // Định nghĩa các tùy chọn phông chữ cho thông điệp đi kèm
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Tùy chỉnh màu nền và cọ cho mã QR
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Nhúng mã QR vào tài liệu
          signature.sign('output.pdf', signOptions);
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
            link: "/examples/signature/formats/signature_qrcode.pdf"
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
    title: "Hiểu khả năng chính của chúng tôi"
    exclude: "qrcode"
    description: "Chúng tôi cung cấp một lựa chọn phong phú các định dạng chữ ký và các thao tác phù hợp với nhu cầu của bạn."
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
    title: "Tích hợp mã QR với nhiều định dạng tệp"
    exclude: "PDF"
    description: "Tận dụng API Node.js via Java để tạo mã QR và nhúng chúng vào nhiều định dạng tệp phổ biến. Ghi lại dữ liệu quan trọng trong những mã vạch này để tích hợp liền mạch và dễ dàng truy xuất sau này."
    items: 
          
        # format loop 1
        - name: "Mã QR cho PDF"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Mã QR cho DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Mã QR cho JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Mã QR cho PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Mã QR cho XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---