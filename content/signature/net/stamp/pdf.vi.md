



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:47
draft: false
lang: vi
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tem nhãn tròn và vuông PDF qua C#"
head_description: "Sử dụng GroupDocs.Signature for .NET để tạo và nhúng các tem cá nhân hóa vào các tệp PDF."

############################# Header ############################
title: "Tạo tem cho các tệp PDF" 
description: "Tích hợp liền mạch các tem thiết kế tùy chỉnh vào bất kỳ phần nào của tài liệu của bạn bằng cách sử dụng GroupDocs.Signature for .NET, cung cấp sự linh hoạt tối đa cho vị trí và cấu hình tem nhằm đáp ứng nhu cầu kinh doanh của bạn."
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
    title: "Tổng quan về GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) là một công cụ đa năng cho phép chèn nhiều loại chữ ký vào tài liệu, bao gồm cả tem có thể tùy chỉnh. Hỗ trợ hơn 60 định dạng tệp, từ PDF và tài liệu Word đến hình ảnh và tệp ZIP, bạn có thể làm phong phú tài liệu của mình với văn bản, hình ảnh, mã vạch, siêu dữ liệu, chứng chỉ số và tem. Hơn nữa, bạn có toàn quyền tìm kiếm, xác thực, sửa đổi hoặc loại bỏ bất kỳ chữ ký nào đã áp dụng cho tệp của bạn.

############################# Steps ############################
steps:
    enable: true
    title: "Cách nhúng tem vào PDF bằng C#"
    content: |
      [GroupDocs.Signature](/signature/net/) cung cấp tính năng tạo tem mạnh mẽ, lý tưởng cho việc nâng cao ứng dụng .NET. Tận dụng công cụ này để thiết kế và triển khai các tem tùy chỉnh cao trên các trang tài liệu của bạn.
      
      1. Cung cấp tài liệu PDF cần có tem.
      2. Sử dụng StampSignOptions để cấu hình cẩn thận tất cả các tham số cần thiết.
      3. Thêm nhiều dòng tem theo yêu cầu của bạn.
      4. Áp dụng tem đã cấu hình và lưu tài liệu đã sửa đổi.
   
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
        // Tích hợp đường dẫn tài liệu với thể hiện Signature
        using (Signature signature = new Signature("input.pdf"))
        {
            // Khởi tạo StampSignOptions với nội dung chữ ký cần thiết
            StampSignOptions options = new StampSignOptions();
            options.Height = 180;
            options.Width = 180;

            // Kết hợp một hoặc nhiều dòng tem
            options.OuterLines.Add(
                new StampLine()
                {
                    Text = "* The Best Company *",
                    TextRepeatType = StampTextRepeatType.FullTextRepeat,
                    Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                    Height = 22,
                    TextBottomIntent = 6,
                    TextColor = Color.WhiteSmoke,
                    BackgroundColor = Color.DarkSlateBlue
                }
            );

            // Lưu trữ tài liệu với tem đã áp dụng
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tận dụng chữ ký để bảo vệ và nâng cao tính toàn vẹn tài liệu"
  description: "Với thư viện GroupDocs.Signature for .NET, bạn có thể tích hợp chức năng chữ ký vào tài liệu của mình. Lấp đầy dễ dàng các tem tùy chỉnh và các loại chữ ký khác, mang lại sự linh hoạt và độ chính xác cho việc quản lý tài liệu an toàn."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Chữ ký tem được cung cấp bởi GroupDocs.Signature"
  features:
    # feature loop
    - title: "Ký tài liệu toàn diện"
      content: "Nâng cao tài liệu của bạn bằng cách đặt chữ ký, bao gồm văn bản, hình ảnh, mã vạch, mã QR và tem, ở bất kỳ vị trí hoặc trang nào trong tệp. Ngoài ra, quản lý siêu dữ liệu nhúng và áp dụng chứng chỉ số để bảo vệ chống lại những thay đổi trái phép."

    # feature loop
    - title: "Tìm kiếm và xác thực chữ ký hiệu quả"
      content: "Sau khi ký, xác minh tính xác thực và tính toàn vẹn của chữ ký tài liệu. Sử dụng chức năng tìm kiếm nâng cao để truy xuất và quản lý tất cả dữ liệu chữ ký được nhúng trong tài liệu."

    # feature loop
    - title: "Sửa đổi và tùy chỉnh chữ ký"
      content: "Điều chỉnh các chữ ký đã được chèn trước đó một cách dễ dàng. Cho dù bạn cần thay đổi nội dung, vị trí, kích thước hay màu sắc, giải pháp của chúng tôi cung cấp sự linh hoạt tối đa cho việc sửa đổi chữ ký."

    # feature loop
    - title: "Dễ dàng xóa chữ ký"
      content: "Khi cần xóa chữ ký, GroupDocs.Signature for .NET cung cấp một bộ công cụ hoàn chỉnh để xóa bất kỳ loại chữ ký nào, bao gồm tem, chứng chỉ số và nhiều hơn nữa, đảm bảo tài liệu của bạn luôn được cập nhật và tuân thủ."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Triển khai tem tùy chỉnh trong tài liệu"
      content: |
        Khám phá cách tạo và tích hợp các tem tùy chỉnh với các chi tiết văn bản quan trọng vào tài liệu của bạn.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Cung cấp tài liệu cần có tem
          using (Signature signature = new Signature("input.pdf"))
          {
              // Khởi tạo các tùy chọn tem với các cấu hình mong muốn
              StampSignOptions options = new StampSignOptions()
              {
                    // Định nghĩa kích thước và vị trí của tem trên trang
                    Height = 200,
                    Width = 200,
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,
                    AllPages = true
              };

              // Kết hợp các đường tròn bên ngoài với văn bản
              options.OuterLines.Add(
                    new StampLine()
                    {
                        Text = "* The best  choice *",
                        TextRepeatType = StampTextRepeatType.FullTextRepeat,
                        Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                        Height = 22,
                        TextBottomIntent = 6,
                        TextColor = Color.WhiteSmoke,
                        BackgroundColor = Color.DarkSlateBlue
                    }
              );

              // Tích hợp các đường vuông bên trong nếu cần
              options.InnerLines.Add(
                    new StampLine()
                    { 
                        Text = "Company #1",
                        TextColor = Color.MediumVioletRed,
                        Font = new SignatureFont() { Size = 20, Bold = true },
                        Height = 40
                    }
              );

              // Hoàn thành và lưu tài liệu đã có tem
              SignResult result = signature.Sign("output.pdf", options);
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
            link: "/examples/signature/formats/signature_stamp.pdf"
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
    title: "Khám phá chức năng cơ bản"
    exclude: "stamp"
    description: "Khám phá nhiều lựa chọn để tạo, quản lý và xóa các loại chữ ký khác nhau, đảm bảo khả năng kiểm soát toàn diện đối với quy trình tài liệu của bạn."
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
    title: "Áp dụng tem trên nhiều định dạng tài liệu khác nhau"
    exclude: "PDF"
    description: "API GroupDocs.Signature cho phép bạn nhúng tem vào hơn 60 loại tệp tiêu chuẩn trong ngành. Áp dụng các tem tùy chỉnh vào bất kỳ vị trí nào trong tài liệu của bạn, giúp tăng cường theo dõi và cá nhân hóa tài liệu."
    items: 
          
        # format loop 1
        - name: "Đóng dấu PDF"
          format: "PDF"
          link: "/signature/net/stamp/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Đóng dấu DOCX"
          format: "DOCX"
          link: "/signature/net/stamp/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Đóng dấu JPEG"
          format: "JPEG"
          link: "/signature/net/stamp/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Đóng dấu PPTX"
          format: "PPTX"
          link: "/signature/net/stamp/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Đóng dấu XLSX"
          format: "XLSX"
          link: "/signature/net/stamp/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---