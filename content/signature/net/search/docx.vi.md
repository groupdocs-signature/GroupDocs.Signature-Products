



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:32
draft: false
lang: vi
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tìm kiếm chữ ký điện tử trong DOCX với C#"
head_description: "Sử dụng khả năng của API GroupDocs.Signature for .NET để tìm kiếm các chữ ký nhúng trong PDF, Word, Excel, Bài thuyết trình và Hình ảnh."

############################# Header ############################
title: "Tìm kiếm chữ ký số trong DOCX" 
description: "Trích xuất liệt kê đầy đủ các chữ ký điện tử nhúng trong nhiều định dạng như PDF, Word, Excel, Bài thuyết trình và Hình ảnh, tất cả được hỗ trợ bởi GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Bắt đầu tải xuống miễn phí của bạn"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Khám phá khả năng của GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) cung cấp chức năng hiện đại cho việc ký tài liệu số. Với hỗ trợ cho hơn 60 định dạng tệp, bao gồm PDF, tài liệu MS Office, Hình ảnh và tệp ZIP, nó cho phép bạn thêm, tìm kiếm, xác minh, sửa đổi hoặc xóa nhiều chữ ký khác nhau, chẳng hạn như văn bản, hình ảnh, mã vạch, mã QR, chứng chỉ số và con dấu.

############################# Steps ############################
steps:
    enable: true
    title: "Cách tìm kiếm chữ ký DOCX bằng C#"
    content: |
      [GroupDocs.Signature](/signature/net/) cung cấp một công cụ mạnh mẽ để xác định vị trí chữ ký số trong các tệp DOCX. Các nhà phát triển .NET có thể dễ dàng nâng cao ứng dụng của họ bằng giải pháp của chúng tôi.
      
      1. Cung cấp đường dẫn tệp DOCX để tìm kiếm chữ ký.
      2. Sử dụng SearchOptions để tinh chỉnh tiêu chí tìm kiếm.
      3. Gọi phương thức Search để lấy kết quả.
      4. Đánh giá danh sách các chữ ký đã xác định.
   
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
        // Khởi tạo một đối tượng Signature với đường dẫn tài liệu đã xác định
        using (Signature signature = new Signature("input.docx"))
        {
            // Tạo một phiên bản của TextSearchOptions để bao gồm tất cả các trang
            TextSearchOptions options = new TextSearchOptions()
            {
                AllPages = true
            };

            // Thực hiện tìm kiếm để xác định bất kỳ chữ ký văn bản nào trong tài liệu
            List<TextSignature> signatures = signature.Search<TextSignature>(options);
            Console.WriteLine($"\nSource document contains following text signature(s).");

            // Lập danh sách các chữ ký đã phát hiện để kiểm tra chi tiết               
            foreach (TextSignature textSignature in signatures)
            {
                Console.WriteLine($"Found Text signature at page {textSignature.PageNumber} with type
                    [{textSignature.SignatureImplementation}] and text '{textSignature.Text}'.");
            }
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Hệ sinh thái ký tài liệu hoàn chỉnh"
  description: "Khám phá một giải pháp ký tài liệu tiên tiến, giàu tính năng, được thiết kế đặc biệt để cải thiện và bảo mật tài liệu của bạn với nhiều loại chữ ký trên các định dạng khác nhau."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Tìm kiếm và quản lý chữ ký"
  features:
    # feature loop
    - title: "Ký và bảo mật tài liệu kinh doanh"
      content: "Thêm chữ ký số vào bất kỳ vị trí nào trong tài liệu. GroupDocs.Signature hỗ trợ nhiều loại chữ ký, bao gồm văn bản, hình ảnh, mã vạch, siêu dữ liệu, con dấu và chứng chỉ số, đảm bảo tính xác thực và tuân thủ của tài liệu."

    # feature loop
    - title: "Quản lý chữ ký toàn diện"
      content: "Sau khi ký, tận dụng tính năng tìm kiếm để lấy tất cả các chữ ký nhúng. Sửa đổi hoặc xóa chữ ký khi cần, mang lại cho bạn quyền kiểm soát hoàn toàn đối với tính toàn vẹn của tài liệu."

    # feature loop
    - title: "Bảo vệ tính toàn vẹn của tài liệu"
      content: "Sử dụng các công cụ tiên tiến để quản lý siêu dữ liệu ẩn bên trong tài liệu. Thêm hoặc xóa các mục siêu dữ liệu và áp dụng chứng chỉ số doanh nghiệp để bảo vệ khỏi các chỉnh sửa trái phép và đảm bảo tính xác thực của tài liệu."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tìm kiếm chữ ký hình ảnh"
      content: |
        Ví dụ này minh họa quy trình phát hiện một chữ ký hình ảnh trong một tài liệu đã xác định.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Cung cấp tài liệu nguồn làm đối số cho bộ khởi tạo
          using (Signature signature = new Signature("input.docx"))
          {
              // Tìm kiếm bất kỳ chữ ký nào thuộc loại văn bản
              List<ImageSignature> signatures = signature.Search<ImageSignature>(SignatureType.Image);
              Console.WriteLine($"\nSource document contains following image signature(s).");

              // Trình bày kết quả với các thuộc tính chi tiết của các chữ ký đã xác định
              foreach (ImageSignature imageSignature in signatures)
              {
                    Console.WriteLine($"Found Image signature at page {imageSignature.PageNumber} 
                    and size {imageSignature.Size}.");
              }
          }
          ```
        platform: "net"
        copy_title: "Sao chép"
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
    title: "Chức năng cốt lõi"
    exclude: "search"
    description: "API của chúng tôi cung cấp sự linh hoạt rộng rãi, cho phép người dùng ký tài liệu và thực hiện các hoạt động sau khi ký một cách toàn diện, chẳng hạn như tìm kiếm, xác minh và sửa đổi chữ ký."
    items: 
          
        # operation loop 1
        - name: "Chữ ký điện tử"
          operation: "esign"
          link: "/signature/net/esign/docx/"
          description: "Thêm các loại chữ ký khác nhau vào các định dạng tệp được hỗ trợ"

        # operation loop 2
        - name: "Thêm văn bản vào tài liệu"
          operation: "text"
          link: "/signature/net/text/docx/"
          description: "Nâng cao nội dung tài liệu với các chữ ký văn bản tùy chỉnh"

        # operation loop 3
        - name: "Chữ ký hình ảnh"
          operation: "image"
          link: "/signature/net/image/docx/"
          description: "Đặt bất kỳ hình ảnh nào ở bất kỳ vị trí nào trong tài liệu"

        # operation loop 4
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/signature/net/barcode/docx/"
          description: "Tạo và chèn các mã vạch khác nhau vào các tài liệu được hỗ trợ"

        # operation loop 5
        - name: "Tạo mã QR"
          operation: "qrcode"
          link: "/signature/net/qrcode/docx/"
          description: "Tạo mã QR, bao gồm mã QR, để ký tài liệu"
          
        # operation loop 6
        - name: "Chứng chỉ số"
          operation: "digital"
          link: "/signature/net/digital/docx/"
          description: "Bảo mật doanh nghiệp và ký các tài liệu bằng chứng chỉ số"

        # operation loop 7
        - name: "Chữ ký đóng dấu"
          operation: "stamp"
          link: "/signature/net/stamp/docx/"
          description: "Sử dụng Trình tạo đóng dấu để tạo các dấu tròn hoặc vuông tùy chỉnh"
          
        # operation loop 8
        - name: "Tìm kiếm chữ ký"
          operation: "search"
          link: "/signature/net/search/docx/"
          description: "Tìm bất kỳ chữ ký nào đã được thêm trước đó trong tài liệu"
          
        # operation loop 9
        - name: "Xác minh chữ ký"
          operation: "verify"
          link: "/signature/net/verify/docx/"
          description: "Xác minh tính xác thực của chữ ký sau khi đã được áp dụng"
          
        # operation loop 10
        - name: "Chỉnh sửa chữ ký"
          operation: "modify"
          link: "/signature/net/modify/docx/"
          description: "Chỉnh sửa dễ dàng nhiều loại chữ ký trong một tài liệu"
          
        # operation loop 11
        - name: "Xóa chữ ký"
          operation: "delete"
          link: "/signature/net/delete/docx/"
          description: "Xóa một loạt các chữ ký đã được áp dụng trước đó"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Lấy chữ ký từ nhiều định dạng tệp khác nhau"
    exclude: "DOCX"
    description: "API GroupDocs.Signature for .NET giúp bạn trích xuất và quản lý chữ ký từ nhiều loại tài liệu khác nhau. Dễ dàng lấy chữ ký nhúng từ tất cả các định dạng tệp chính để phân tích hoặc xử lý thêm."
    items: 
          
        # format loop 1
        - name: "Tìm chữ ký trong PDF"
          format: "PDF"
          link: "/signature/net/search/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Tìm chữ ký trong DOCX"
          format: "DOCX"
          link: "/signature/net/search/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Tìm chữ ký trong PPTX"
          format: "PPTX"
          link: "/signature/net/search/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 4
        - name: "Tìm chữ ký trong XLSX"
          format: "XLSX"
          link: "/signature/net/search/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---