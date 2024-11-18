



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:59
draft: false
lang: vi
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Thêm chữ ký điện tử vào tệp XLSX bằng JavaScript"
head_description: "Đặt chữ ký điện tử trên tệp XLSX bằng JavaScript chỉ với vài dòng mã. Sử dụng GroupDocs.Signature for Node.js via Java để ký nhiều định dạng tệp."

############################# Header ############################
title: "Bảo vệ XLSX bằng chứng chỉ điện tử" 
description: "Đảm bảo an ninh cho tài liệu kinh doanh của bạn bằng cách nhúng các chứng chỉ điện tử sử dụng các khả năng tiên tiến của GroupDocs.Signature for Node.js via Java. Chúng tôi cung cấp các tùy chọn linh hoạt để bảo vệ và xác thực tài liệu của bạn."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải về miễn phí"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Giới thiệu về GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) là một giải pháp ký toàn diện được thiết kế để xử lý nhiều nhu cầu xử lý tài liệu khác nhau. Nó cho phép bạn kết hợp văn bản, hình ảnh, chứng chỉ điện tử và con dấu vào hơn 60 định dạng tệp khác nhau, bao gồm PDF, MS Office, hình ảnh và tệp ZIP. Thêm vào đó, tài liệu đã ký có thể dễ dàng tìm kiếm, xác minh, chỉnh sửa hoặc xóa khi cần.

############################# Steps ############################
steps:
    enable: true
    title: "Hướng dẫn bảo mật XLSX bằng chứng chỉ điện tử trong JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) cho phép các nhà phát triển Node.js via Java bảo vệ tài liệu XLSX khỏi sự chỉnh sửa bằng cách sử dụng chữ ký điện tử. Nâng cao ứng dụng kinh doanh của bạn với các tính năng bảo mật dữ liệu toàn diện.
      
      1. Chuyển tài liệu XLSX vào constructor của lớp Signature.
      2. Áp dụng một chứng chỉ điện tử và mật khẩu tương ứng để bảo vệ tài liệu.
      3. Tùy chọn, thêm một hình ảnh đại diện cho chữ ký điện tử vào các trang tài liệu.
      4. Ký tài liệu để ngăn chặn bất kỳ thay đổi nào trong tương lai.
   
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

        // Sử dụng Signature để áp dụng chữ ký điện tử vào tài liệu
        const signature = new signatureLib.Signature('input.xlsx');

        // Cung cấp chứng chỉ điện tử và mật khẩu cần thiết
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // Cấu hình thiết lập chữ ký hình ảnh nếu cần thiết
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);
        
        // Mã hóa tài liệu bằng chứng chỉ điện tử
        const result = signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tối ưu hoặc bảo mật nội dung tài liệu bằng chữ ký"
  description: "GroupDocs.Signature for Node.js via Java được xây dựng để ký tất cả các định dạng tệp chính, mang đến cho bạn khả năng thêm, điều chỉnh, xác minh hoặc xóa nhiều loại chữ ký khác nhau."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Signature"
  features:
    # feature loop
    - title: "Thêm chữ ký vào tài liệu của bạn"
      content: "Đặt dễ dàng chữ ký Văn bản, Hình ảnh, Mã vạch, QR-Code, hoặc con dấu trên bất kỳ trang nào của tài liệu được hỗ trợ. Bạn cũng có thể chèn hoặc chỉnh sửa siêu dữ liệu ẩn, chẳng hạn như EXIF trong hình ảnh. Bảo vệ nội dung tài liệu của bạn khỏi những thay đổi trái phép bằng các chứng chỉ điện tử."

    # feature loop
    - title: "Tìm và xác minh chữ ký"
      content: "Sau khi ký, tài liệu của bạn có thể trải qua nhiều lần xác minh. Xác nhận tính toàn vẹn của nội dung đã ký, hoặc tiến hành tìm kiếm chi tiết để liệt kê tất cả các chữ ký hiện có."

    # feature loop
    - title: "Sửa đổi các chữ ký hiện có"
      content: "Hầu hết các loại chữ ký cho phép chỉnh sửa sau khi tạo. Bạn có thể dễ dàng sửa đổi văn bản, điều chỉnh vị trí các phần tử, điều chỉnh màu sắc, thay đổi kích thước và thực hiện các thay đổi cần thiết khác."

    # feature loop
    - title: "Loại bỏ các chữ ký không cần thiết"
      content: "Giải pháp của chúng tôi cho phép thực hiện toàn bộ các thao tác CRUD cho chữ ký. Nếu cần, bạn có thể xóa các loại chữ ký khác nhau, bao gồm chứng chỉ điện tử, khỏi tài liệu của bạn."
      
  code_samples:
    # code sample loop
    - title: "Bảo vệ tài liệu bằng chữ ký điện tử"
      content: |
        Tìm hiểu cách khóa một tài liệu chống lại các thay đổi bằng chữ ký điện tử.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Cung cấp tài liệu cần ký
        const signature = new signatureLib.Signature('input.xlsx');

        // Sử dụng chứng chỉ điện tử phù hợp và mật khẩu của nó
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // Bao gồm bất kỳ thông tin văn bản bổ sung nào
        options.setReason('Security issue');
        options.setContact('John Smith');
        options.setLocation('Office D.W.');

        // Thêm các yếu tố hình ảnh như hình ảnh cho đại diện chữ ký
        options.setImageFilePath('image.png');
        options.setAllPages(true);
        options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
        options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        const padding = new signatureLib.Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);
        
        // Lưu tài liệu đã được bảo mật bằng chữ ký điện tử vào vị trí được chỉ định
        const result = signature.sign('output.xlsx', options);
        ```
        {{< /landing/code >}}


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
    title: "Khám phá các chức năng chính của chúng tôi"
    exclude: "digital"
    description: "Chúng tôi tự hào hỗ trợ một bộ các tùy chọn và chức năng chữ ký toàn diện."
    items: 
          
        # operation loop 1
        - name: "Chữ ký điện tử"
          operation: "esign"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "Thêm các loại chữ ký khác nhau vào các định dạng tệp được hỗ trợ"

        # operation loop 2
        - name: "Thêm văn bản vào tài liệu"
          operation: "text"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Nâng cao nội dung tài liệu với các chữ ký văn bản tùy chỉnh"

        # operation loop 3
        - name: "Chữ ký hình ảnh"
          operation: "image"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Đặt bất kỳ hình ảnh nào ở bất kỳ vị trí nào trong tài liệu"

        # operation loop 4
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "Tạo và chèn các mã vạch khác nhau vào các tài liệu được hỗ trợ"

        # operation loop 5
        - name: "Tạo mã QR"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Tạo mã QR, bao gồm mã QR, để ký tài liệu"
          
        # operation loop 6
        - name: "Chứng chỉ số"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Bảo mật doanh nghiệp và ký các tài liệu bằng chứng chỉ số"

        # operation loop 7
        - name: "Chữ ký đóng dấu"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "Sử dụng Trình tạo đóng dấu để tạo các dấu tròn hoặc vuông tùy chỉnh"
          
        # operation loop 8
        - name: "Tìm kiếm chữ ký"
          operation: "search"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "Tìm bất kỳ chữ ký nào đã được thêm trước đó trong tài liệu"
          
        # operation loop 9
        - name: "Xác minh chữ ký"
          operation: "verify"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "Xác minh tính xác thực của chữ ký sau khi đã được áp dụng"
          
        # operation loop 10
        - name: "Chỉnh sửa chữ ký"
          operation: "modify"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "Chỉnh sửa dễ dàng nhiều loại chữ ký trong một tài liệu"
          
        # operation loop 11
        - name: "Xóa chữ ký"
          operation: "delete"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "Xóa một loạt các chữ ký đã được áp dụng trước đó"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Ký tài liệu trên nhiều định dạng"
    exclude: "XLSX"
    description: "API Node.js via Java hỗ trợ hơn 60 định dạng, cho phép bạn áp dụng nhiều loại chữ ký trên bất kỳ trang nào, thực thi bảo mật nội dung bằng các chứng chỉ điện tử, và quản lý chữ ký trong tài liệu một cách hiệu quả."
    items: 
          
        # format loop 1
        - name: "Bảo vệ PDF"
          format: "PDF"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Bảo vệ DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Bảo vệ PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 4
        - name: "Bảo vệ XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---