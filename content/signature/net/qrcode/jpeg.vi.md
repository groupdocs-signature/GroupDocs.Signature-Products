



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:21
draft: false
lang: vi
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tạo mã QR cho tệp JPEG bằng C#"
head_description: "Sử dụng API GroupDocs.Signature để tạo mã QR cho tệp JPEG. Nhúng mã QR một cách liền mạch trên bất kỳ trang nào để nâng cao chức năng."

############################# Header ############################
title: "Tạo mã QR cho JPEG" 
description: "Tạo mã vạch 2D bằng văn bản hoặc dữ liệu số và áp dụng chúng trên nhiều trang và định dạng khác nhau, bao gồm PDF, Word, Excel và nhiều hơn nữa, thông qua GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Bắt đầu dùng thử miễn phí"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Khám phá khả năng của GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) cung cấp một loạt các tính năng, cho phép người dùng tạo và nhúng nhiều loại chữ ký khác nhau trên các định dạng tài liệu hàng đầu. Dù là PDF, tài liệu Word, bảng tính Excel, bài thuyết trình PowerPoint hay tệp hình ảnh, bạn có thể nâng cao tài liệu của mình với các chữ ký Text, Image, Barcode, QR Code, Metadata, Digital và Stamp.

############################# Steps ############################
steps:
    enable: true
    title: "Cách tạo và chèn mã QR ở bất kỳ đâu trong JPEG"
    content: |
      [GroupDocs.Signature](/signature/net/) hỗ trợ việc tạo mã QR trong nhiều định dạng phổ biến và vị trí của chúng trên các trang JPEG. Hỗ trợ hơn 10 loại mã QR, thư viện của chúng tôi có thể được tích hợp liền mạch vào các ứng dụng .NET. Nâng cao tài liệu của bạn với các chữ ký mã QR sử dụng sản phẩm của chúng tôi.
      
      1. Lấy tệp JPEG hoặc luồng cần được ký với mã QR.
      2. Cung cấp văn bản cần thiết cho QrCodeSignOptions.
      3. Tùy chỉnh các tham số hình ảnh như màu sắc, vị trí, kích thước, v.v.
      4. Lưu tài liệu với mã QR nhúng.
   
    code:
      platform: "net"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Chữ ký mẫu"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "nhấp để sao chép"
        copy_done: "đã sao chép"
      links:
        #  loop
        - title: "Thêm ví dụ"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "Tài liệu hướng dẫn"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // Khởi tạo một phiên bản Signature mới với tài liệu
        using (Signature signature = new Signature("input.jpeg"))
        {
            // Sử dụng QrCodeSignOptions để nhúng mã QR vào tài liệu
            QrCodeSignOptions options = new QrCodeSignOptions("Text Content")
                {
                    // Xác định loại chữ ký và chỉ định vị trí của nó trên trang
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150
                };

            // Lưu tài liệu với mã QR đã tích hợp
            SignResult result = signature.Sign("output.jpeg", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tích hợp chữ ký toàn diện cho tài liệu"
  description: "Với API GroupDocs.Signature for .NET, người dùng có thể tạo, sửa đổi, tìm kiếm, xác minh và loại bỏ nhiều loại chữ ký khác nhau, đơn giản hóa quy trình làm việc với tài liệu một cách chính xác chưa từng thấy."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Signature"
  features:
    # feature loop
    - title: "Ký tài liệu với nhiều loại chữ ký"
      content: "GroupDocs.Signature cho phép áp dụng chữ ký Text, Image, Barcode, QR Code và Stamp cho bất kỳ định dạng tài liệu nào. Các chữ ký có thể được đặt chính xác trên bất kỳ trang nào, và metadata có thể được quản lý liền mạch thông qua chữ ký metadata. Bảo vệ tính toàn vẹn của tài liệu bằng cách kết hợp các chứng chỉ số để ngăn chặn các thay đổi trái phép."

    # feature loop
    - title: "Tìm kiếm và xác minh chữ ký"
      content: "Xác minh tính xác thực và độ chính xác của chữ ký tài liệu thông qua quy trình xác minh tiên tiến. Dễ dàng truy xuất danh sách chi tiết tất cả các chữ ký được nhúng trong một tài liệu để có cái nhìn tổng quan."

    # feature loop
    - title: "Sửa đổi chữ ký tùy chỉnh"
      content: "Cập nhật và tinh chỉnh các chữ ký đã áp dụng trước đó bằng cách điều chỉnh nội dung, vị trí, màu sắc, kích thước, và các thuộc tính khác để đáp ứng nhu cầu cụ thể của bạn."

    # feature loop
    - title: "Loại bỏ chữ ký hiệu quả"
      content: "Đơn giản hóa việc quản lý tài liệu bằng cách lập trình loại bỏ các chữ ký không mong muốn. Dù là liên quan đến chứng chỉ số hay các loại chữ ký khác, việc loại bỏ có thể được thực hiện nhanh chóng và hiệu quả."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cách tạo mã QR với nhiều tùy chọn khác nhau?"
      content: |
        Ví dụ này minh họa cách đặt mã QR tùy chỉnh trên trang JPEG.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Lấy tài liệu cần ký và truyền vào Signature
          using (Signature signature = new Signature("input.jpeg"))
          {
              // Cấu hình tùy chọn mã QR với văn bản cần thiết
              QrCodeSignOptions options = new QrCodeSignOptions("Archived on July 11, 2019")
              {
                    // Chỉ định vị trí tương đối của mã QR trên trang
                    VerticalAlignment = Domain.VerticalAlignment.Top,
                    HorizontalAlignment = Domain.HorizontalAlignment.Right,

                    // Đặt khoảng cách chữ ký
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // Xác định màu sắc của mã QR
                    ForeColor = Color.Red,

                    // Xác định tùy chọn phông chữ cho thông điệp
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // Tùy chỉnh màu nền và bút vẽ của mã QR
                    Background = new Background()
                    {
                        Color = Color.LimeGreen,
                        Transparency = 0.5,
                        Brush = new Domain.Extensions.LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                    }
              };

              // Nhúng mã QR vào tài liệu
              SignResult result = signature.Sign("output.jpeg", options);
          }
          ```
        platform: "net"
        copy_title: "Sao chép"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "nhấp để sao chép"
          copy_done: "đã sao chép"
        top_links:
          #  loop
          - title: "Tải xuống kết quả"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.jpeg"
        links:
          #  loop
          - title: "Thêm ví dụ"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "Tài liệu hướng dẫn"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Sẵn sàng bắt đầu? "
  description: "Dùng thử các tính năng của GroupDocs.Signature miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "Tải xuống Nuget"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "Giấy phép"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Tìm hiểu về giải pháp chữ ký của chúng tôi"
    exclude: "qrcode"
    description: "Chúng tôi tự hào giới thiệu một loạt các loại chữ ký và các tính năng hoạt động"
    items: 
          
        # operation loop 1
        - name: "Chữ ký điện tử"
          operation: "esign"
          link: "/signature/net/esign/jpeg/"
          description: "Thêm các loại chữ ký khác nhau vào các định dạng tệp được hỗ trợ"

        # operation loop 2
        - name: "Thêm văn bản vào tài liệu"
          operation: "text"
          link: "/signature/net/text/jpeg/"
          description: "Nâng cao nội dung tài liệu với các chữ ký văn bản tùy chỉnh"

        # operation loop 3
        - name: "Chữ ký hình ảnh"
          operation: "image"
          link: "/signature/net/image/jpeg/"
          description: "Đặt bất kỳ hình ảnh nào ở bất kỳ vị trí nào trong tài liệu"

        # operation loop 4
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/signature/net/barcode/jpeg/"
          description: "Tạo và chèn các mã vạch khác nhau vào các tài liệu được hỗ trợ"

        # operation loop 5
        - name: "Tạo mã QR"
          operation: "qrcode"
          link: "/signature/net/qrcode/jpeg/"
          description: "Tạo mã QR, bao gồm mã QR, để ký tài liệu"
          
        # operation loop 6
        - name: "Chứng chỉ số"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "Bảo mật doanh nghiệp và ký các tài liệu bằng chứng chỉ số"

        # operation loop 7
        - name: "Chữ ký đóng dấu"
          operation: "stamp"
          link: "/signature/net/stamp/jpeg/"
          description: "Sử dụng Trình tạo đóng dấu để tạo các dấu tròn hoặc vuông tùy chỉnh"
          
        # operation loop 8
        - name: "Tìm kiếm chữ ký"
          operation: "search"
          link: "/signature/net/search/pdf/"
          description: "Tìm bất kỳ chữ ký nào đã được thêm trước đó trong tài liệu"
          
        # operation loop 9
        - name: "Xác minh chữ ký"
          operation: "verify"
          link: "/signature/net/verify/pdf/"
          description: "Xác minh tính xác thực của chữ ký sau khi đã được áp dụng"
          
        # operation loop 10
        - name: "Chỉnh sửa chữ ký"
          operation: "modify"
          link: "/signature/net/modify/pdf/"
          description: "Chỉnh sửa dễ dàng nhiều loại chữ ký trong một tài liệu"
          
        # operation loop 11
        - name: "Xóa chữ ký"
          operation: "delete"
          link: "/signature/net/delete/pdf/"
          description: "Xóa một loạt các chữ ký đã được áp dụng trước đó"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tạo mã QR cho các định dạng tài liệu khác"
    exclude: "JPEG"
    description: "Nâng cao tất cả các định dạng tệp tiêu chuẩn ngành với khả năng nhúng mã QR thông qua API .NET. Lưu trữ và mã hóa thông tin quan trọng vào mã vạch 2D để quét và truy xuất dữ liệu một cách liền mạch."
    items: 
          
        # format loop 1
        - name: "Mã QR cho PDF"
          format: "PDF"
          link: "/signature/net/qrcode/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Mã QR cho DOCX"
          format: "DOCX"
          link: "/signature/net/qrcode/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Mã QR cho JPEG"
          format: "JPEG"
          link: "/signature/net/qrcode/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Mã QR cho PPTX"
          format: "PPTX"
          link: "/signature/net/qrcode/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Mã QR cho XLSX"
          format: "XLSX"
          link: "/signature/net/qrcode/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---