



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:07
draft: false
lang: vi
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Tạo mã vạch cho JPEG bằng các ứng dụng JavaScript"
head_description: "Nhanh chóng tạo và nhúng một chữ ký mã vạch vào tài liệu JPEG với JavaScript chỉ bằng vài dòng mã. GroupDocs.Signature hỗ trợ ký kết trên nhiều định dạng tệp khác nhau."

############################# Header ############################
title: "Tạo và thêm Mã vạch vào JPEG một cách dễ dàng" 
description: "Sử dụng GroupDocs.Signature for Node.js via Java để tích hợp mã vạch vào tài liệu kinh doanh của bạn, đặt chúng chính xác ở vị trí cần thiết. Giải pháp của chúng tôi cung cấp nhiều tùy chọn tùy chỉnh để điều chỉnh chữ ký mã vạch theo yêu cầu của bạn."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải Xuống Ngay – Miễn Phí!"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Giới thiệu về GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) là một công cụ ký tài liệu mạnh mẽ, hỗ trợ nhiều loại chữ ký khác nhau bao gồm văn bản, hình ảnh, mã vạch, chứng chỉ số và con dấu. Với khả năng tương thích trên hơn 60 định dạng tệp, như PDF, tệp MS Office, hình ảnh, và kho lưu trữ ZIP, nó cho phép quản lý tài liệu toàn diện. Các chữ ký trong tài liệu có thể được tìm kiếm, xác minh, thay đổi hoặc xóa theo yêu cầu.

############################# Steps ############################
steps:
    enable: true
    title: "Cách tạo và nhúng mã vạch vào tệp JPEG"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) cho phép tạo và đặt mã vạch vào nhiều định dạng phổ biến trên các trang JPEG. Với sự hỗ trợ cho hơn 60 loại mã vạch, các ứng dụng Node.js via Java có thể được nâng cao dễ dàng với các tính năng ký mã vạch bằng cách tích hợp thư viện của chúng tôi.
      
      1. Cung cấp tệp hoặc luồng JPEG để xử lý.
      2. Chuyển văn bản mã vạch cho một phiên bản BarcodeSignOptions.
      3. Điều chỉnh các cài đặt mã vạch như vị trí, kích thước, v.v.
      4. Lưu tài liệu với mã vạch mới được thêm vào.
   
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

        // Khởi tạo một đối tượng Signature với đường dẫn tài liệu
        const signature = new signatureLib.Signature('input.jpeg');

        // Sử dụng BarcodeSignOptions để tích hợp mã vạch vào tài liệu
        const options = new signatureLib.BarcodeSignOptions('Business data');

        // Cấu hình loại mã vạch và các tham số bổ sung
        options.setEncodeType(signatureLib.BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);
  
        // Lưu tài liệu đã ký
        signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tăng cường và bảo mật tài liệu của bạn với các tùy chọn chữ ký tiên tiến"
  description: "Thư viện GroupDocs.Signature for Node.js via Java được thiết kế để đơn giản hóa việc ký và quản lý các định dạng tài liệu phổ biến. Nhanh chóng và hiệu quả thêm, sửa đổi, xác minh hoặc xóa nhiều loại chữ ký."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Tính Năng Chính của GroupDocs.Signature"
  features:
    # feature loop
    - title: "Ký tài liệu động"
      content: "Ký bất kỳ trang nào trong tài liệu của bạn bằng nhiều loại chữ ký khác nhau, bao gồm văn bản, hình ảnh, mã vạch, mã QR và con dấu. Thêm vào đó, bạn có thể nhúng metadata ẩn như dữ liệu EXIF trong hình ảnh hoặc bảo mật tài liệu chống lại việc chỉnh sửa trái phép bằng cách sử dụng chứng chỉ số."

    # feature loop
    - title: "Xác minh và tìm kiếm chữ ký mạnh mẽ"
      content: "Giải pháp của chúng tôi cung cấp nhiều công cụ để quản lý tài liệu đã ký. Xác minh tính xác thực của chữ ký để đảm bảo tính toàn vẹn của tài liệu và sử dụng tính năng tìm kiếm để liệt kê tất cả chữ ký được nhúng trong một tài liệu."

    # feature loop
    - title: "Sửa đổi chữ ký một cách dễ dàng"
      content: "Hầu hết các chữ ký được thêm vào trước đó có thể dễ dàng sửa đổi. Cập nhật văn bản, di chuyển vị trí, hoặc thay đổi kiểu dáng của chữ ký cho phù hợp với nhu cầu của bạn."

    # feature loop
    - title: "Xóa chữ ký một cách đơn giản"
      content: "Với hỗ trợ toàn diện cho các thao tác CRUD, công cụ của chúng tôi cho phép xóa chữ ký một cách hiệu quả khỏi tài liệu của bạn, đảm bảo chỉ giữ lại những chữ ký phù hợp nhất."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cách áp dụng chữ ký mã vạch"
      content: |
        Ví dụ này minh họa cách nhúng một mã vạch tùy chỉnh vào các trang tài liệu JPEG.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Cung cấp tài liệu cần ký
          const signature = new signatureLib.Signature('input.jpeg');

          // Sử dụng BarcodeSignOptions để tích hợp mã vạch vào tài liệu
          const signOptions = new signatureLib.BarcodeSignOptions('Accepted');
          signOptions.setEncodeType(signatureLib.BarcodeTypes.Code39FullASCII);

          // Cấu hình loại mã vạch và các tham số bổ sung
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Left);

          // Xác định độ lề của mã vạch từ cạnh trang
          const padding = new signatureLib.Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // Chọn màu của mã vạch
          signOptions.setForeColor(signatureLib.Color.RED);

          // Chỉ định kiểu chữ cho thông điệp
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName('Arial');
          signOptions.setFont(font);

          // Chỉ định vị trí của thông điệp
          signOptions.setCodeTextAlignment(signatureLib.CodeTextAlignment.Above);

          // Ký và lưu tài liệu
          signature.sign('output.jpeg', signOptions);

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
            link: "/examples/signature/formats/signature_barcode.jpeg"
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
    title: "Khám phá các tính năng chính của chúng tôi"
    exclude: "barcode"
    description: "Trải nghiệm nhiều loại chữ ký và công cụ mà chúng tôi cung cấp."
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
    title: "Ký trên nhiều định dạng tài liệu khác nhau"
    exclude: "JPEG"
    description: "API Node.js via Java cho phép bạn ký trên hơn 60 định dạng khác nhau. Dù là thêm chữ ký vào các trang cụ thể hay định vị chúng một cách chính xác, công cụ của chúng tôi giúp việc áp dụng nhiều loại chữ ký trở nên dễ dàng."
    items: 
          
        # format loop 1
        - name: "Thêm mã vạch vào PDF"
          format: "PDF"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Thêm mã vạch vào DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Thêm mã vạch vào JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Thêm mã vạch vào PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Thêm mã vạch vào XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---