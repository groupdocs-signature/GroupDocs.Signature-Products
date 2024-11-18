



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:59
draft: false
lang: vi
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Thêm chữ ký điện tử số vào tệp PDF bằng C#"
head_description: "Đặt chữ ký số trên tệp PDF bằng C# chỉ với vài dòng mã. Sử dụng GroupDocs.Signature for .NET để ký nhiều định dạng tệp khác nhau."

############################# Header ############################
title: "Ký PDF bằng chữ ký số" 
description: "Bảo vệ tính toàn vẹn của tài liệu kinh doanh của bạn bằng cách niêm phong chúng bằng chứng chỉ số thông qua các tính năng mạnh mẽ của GroupDocs.Signature for .NET. Chúng tôi cung cấp các giải pháp linh hoạt để đánh dấu và bảo mật tài liệu của bạn."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống miễn phí"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Giới thiệu về GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) là một giải pháp ký kết tinh vi hỗ trợ một loạt các nhiệm vụ xử lý tài liệu. Nó cho phép bạn nhúng văn bản, hình ảnh, chứng chỉ số và con dấu vào tệp ở hơn 60 định dạng, bao gồm PDF, MS Office, hình ảnh, tệp ZIP và các định dạng kinh doanh thiết yếu khác. Hơn nữa, các tài liệu đã ký có thể được tìm kiếm, xác minh, sửa đổi hoặc xóa dễ dàng khi cần thiết.

############################# Steps ############################
steps:
    enable: true
    title: "Cách bảo mật PDF bằng chứng chỉ số trong C#"
    content: |
      [GroupDocs.Signature](/signature/net/) giúp các nhà phát triển .NET bảo vệ tài liệu PDF khỏi các thay đổi bằng cách sử dụng chữ ký số. Tăng cường khả năng bảo vệ dữ liệu cho ứng dụng kinh doanh của bạn.
      
      1. Chuyển tài liệu PDF đến hàm khởi tạo lớp Signature.
      2. Sử dụng một chứng chỉ số và mật khẩu của nó để bảo vệ tài liệu.
      3. Tùy chọn, thêm một đại diện hình ảnh của chữ ký số trên các trang tài liệu.
      4. Ký tài liệu để đảm bảo nó không bị thay đổi.
   
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
        // Sử dụng Signature để ký số tài liệu
        using (Signature signature = new Signature("input.pdf"))
        {
            // Cung cấp chứng chỉ số và mật khẩu liên quan
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // Cấu hình đại diện hình ảnh nếu cần thiết
                PageNumber = 1,
                Left = 50,
                Top = 50
            };

            // Bảo mật tài liệu bằng chứng chỉ số
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Nâng cao hoặc bảo vệ nội dung tài liệu bằng chữ ký"
  description: "Thư viện GroupDocs.Signature for .NET được thiết kế để ký tất cả các định dạng tệp phổ biến. Tinh giản quy trình kinh doanh của bạn bằng cách thêm, sửa đổi, xác minh hoặc xóa nhiều loại chữ ký một cách dễ dàng."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Các tính năng nổi bật của GroupDocs.Signature"
  features:
    # feature loop
    - title: "Nhúng chữ ký vào tài liệu"
      content: "Nhúng chữ ký văn bản, hình ảnh, mã vạch, QR-Code hoặc con dấu một cách chính xác trên bất kỳ trang nào của tài liệu được hỗ trợ. Bạn cũng có thể thêm hoặc chỉnh sửa siêu dữ liệu ẩn, như EXIF, trong hình ảnh và hầu hết các loại tệp. Đảm bảo tính toàn vẹn của nội dung tài liệu của bạn với chữ ký số."

    # feature loop
    - title: "Tìm kiếm và xác minh chữ ký"
      content: "Xử lý sau khi ký mang lại rất nhiều khả năng. Xác minh rằng các tài liệu đã ký của bạn đã được xử lý đúng cách. Để kiểm soát tốt hơn, hãy lấy danh sách toàn diện của tất cả chữ ký thông qua chức năng tìm kiếm."

    # feature loop
    - title: "Chỉnh sửa chữ ký"
      content: "Hầu hết các loại chữ ký đều có thể chỉnh sửa hoàn toàn. Bạn có thể linh hoạt điều chỉnh văn bản, thay đổi vị trí các phần tử, thay đổi màu sắc, thay đổi kích thước và nhiều hơn nữa."

    # feature loop
    - title: "Xóa chữ ký không cần thiết"
      content: "Giải pháp của chúng tôi cung cấp các thao tác CRUD hoàn chỉnh cho các chữ ký. Nếu cần thiết, bạn có thể xóa nhiều loại chữ ký, bao gồm cả chứng chỉ số, khỏi tài liệu của bạn."
      
  code_samples:
    # code sample loop
    - title: "Bảo mật tài liệu bằng chữ ký số"
      content: |
        Khám phá cách ngăn chặn sự thay đổi tài liệu bằng cách sử dụng chữ ký số.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        // Cung cấp tài liệu cần ký
        using (Signature signature = new Signature("input.pdf"))
        {
            // Sử dụng một chứng chỉ số hợp lệ với mật khẩu tương ứng
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // Chỉ định bất kỳ thông tin văn bản bổ sung nào
                Reason = "Security issue",
                Contact = "John Smith",
                Location = "Office D.W.",

                // Nhúng một hình ảnh và các tùy chọn khác để đại diện hình ảnh
                ImageFilePath = "image.png",
                AllPages = true,
                VerticalAlignment = VerticalAlignment.Center,
                HorizontalAlignment = HorizontalAlignment.Left,
                Width = 60,
                Height = 80,

                Margin = new Padding() {  Bottom = 10, Right = 10 }
            };

            // Lưu tài liệu đã được bảo mật tại một vị trí đã chỉ định
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```
        {{< /landing/code >}}


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
    title: "Xem các tính năng nổi bật của chúng tôi"
    exclude: "digital"
    description: "Chúng tôi cung cấp đa dạng các định dạng chữ ký và các thao tác mạnh mẽ"
    items: 
          
        # operation loop 1
        - name: "Chữ ký điện tử"
          operation: "esign"
          link: "/signature/net/esign/pdf/"
          description: "Thêm các loại chữ ký khác nhau vào các định dạng tệp được hỗ trợ"

        # operation loop 2
        - name: "Thêm văn bản vào tài liệu"
          operation: "text"
          link: "/signature/net/text/pdf/"
          description: "Nâng cao nội dung tài liệu với các chữ ký văn bản tùy chỉnh"

        # operation loop 3
        - name: "Chữ ký hình ảnh"
          operation: "image"
          link: "/signature/net/image/pdf/"
          description: "Đặt bất kỳ hình ảnh nào ở bất kỳ vị trí nào trong tài liệu"

        # operation loop 4
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/signature/net/barcode/pdf/"
          description: "Tạo và chèn các mã vạch khác nhau vào các tài liệu được hỗ trợ"

        # operation loop 5
        - name: "Tạo mã QR"
          operation: "qrcode"
          link: "/signature/net/qrcode/pdf/"
          description: "Tạo mã QR, bao gồm mã QR, để ký tài liệu"
          
        # operation loop 6
        - name: "Chứng chỉ số"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "Bảo mật doanh nghiệp và ký các tài liệu bằng chứng chỉ số"

        # operation loop 7
        - name: "Chữ ký đóng dấu"
          operation: "stamp"
          link: "/signature/net/stamp/pdf/"
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
    title: "Ký tài liệu trong nhiều định dạng"
    exclude: "PDF"
    description: "API .NET giúp bạn xử lý hơn 60 định dạng khác nhau. Bạn có thể dễ dàng tạo và nhúng nhiều chữ ký trên bất kỳ trang nào, áp dụng chứng chỉ số để bảo mật nội dung và quản lý hiệu quả các chữ ký hiện có trong tài liệu."
    items: 
          
        # format loop 1
        - name: "Bảo vệ PDF"
          format: "PDF"
          link: "/signature/net/digital/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Bảo vệ DOCX"
          format: "DOCX"
          link: "/signature/net/digital/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Bảo vệ PPTX"
          format: "PPTX"
          link: "/signature/net/digital/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 4
        - name: "Bảo vệ XLSX"
          format: "XLSX"
          link: "/signature/net/digital/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---