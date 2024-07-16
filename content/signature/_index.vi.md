---
############################# Static ############################
layout: "family"
date:  2024-07-16T12:27:51
draft: false

product: "Signature"
product_tag: "signature"

lang: vi

############################# Head ############################
head_title: "Ứng dụng chữ ký số C# .NET, Java, Node.js"
head_description: "Tích hợp chữ ký điện tử trong các ứng dụng .NET, Java hoặc Node.js với GroupDocs.Signature. Ký các định dạng tài liệu kinh doanh phổ biến."

############################# Header ############################
title: "Giải pháp ký điện tử tài liệu"
description:  |
  Ký các tài liệu và hình ảnh kỹ thuật số trên bất kỳ nền tảng nào bằng cách sử dụng API linh hoạt và các giải pháp dựa trên ứng dụng của chúng tôi dành cho lập trình viên và người dùng cuối.

  Tìm kiếm và sửa đổi chữ ký đã thêm trước đó bằng các phương pháp nâng cao.

  Bảo vệ tài liệu khỏi những thay đổi bằng chứng chỉ kỹ thuật số và kiểm soát siêu dữ liệu ẩn.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Chọn nền tảng của bạn"
  title: "Nền tảng độc lập"
  description: "Thư viện GroupDocs.Signature hỗ trợ các hệ điều hành và khung sau:"
  details_link_title: "Tìm hiểu thêm"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Signature .NET 
      color: "blue"
      tag: "net"
      link: "/signature/net/"
      features_link: "https://docs.groupdocs.com/signature/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.6.2 or higher <br> .NET Core 3.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS <br> Microsoft Azure
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Signature Java
      color: "red"
      tag: "java"
      link: "/signature/java/"
      features_link: "https://docs.groupdocs.com/signature/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 8 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Signature Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/signature/nodejs-java/"
      features_link: "https://docs.groupdocs.com/signature/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Bất kỳ trình soạn thảo văn bản nào khác
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

############################# Features ###############################
features:
  enable: true
  title: "Các tính năng chính của GroupDocs.Signature"
  description: "Giải pháp của chúng tôi được thiết kế để thêm nhiều loại chữ ký khác nhau vào các định dạng tài liệu và tệp phổ biến. Làm phong phú quy trình kinh doanh của bạn một cách dễ dàng."

  items:
    # items loop
    - icon: "additional"
      title: "Làm phong phú dữ liệu của bạn bằng chữ ký"
      content: "Nối văn bản, hình ảnh, hình mờ, v.v. vào tài liệu kinh doanh của bạn."

    # items loop
    - icon: "protect"
      title: "Bảo vệ nội dung tài liệu"
      content: "Cấm thay đổi tài liệu bằng cách niêm phong nó bằng chứng chỉ kỹ thuật số."

    # items loop
    - icon: "search"
      title: "Thêm dữ liệu ẩn và mã vạch"
      content: "Sử dụng siêu dữ liệu để lưu trữ thông tin vô hình hoặc đặt mã vạch tùy chỉnh trên các trang."

    # items loop
    - icon: "manipulate"
      title: "Thao tác chữ ký"
      content: "Tìm kiếm, cập nhật hoặc xóa tất cả chữ ký đã được thêm trước đó."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Bảo vệ tập tin của bạn bằng chữ ký"
  description: "Ví dụ về mã GroupDocs.Signature"
  items:
    # code sample loop
    - title: "Tạo và thêm mã QR"
      content: |
       GroupDocs.Signature cho phép chúng tôi tạo và thêm mã QR vào tài liệu có định dạng được hỗ trợ. Cung cấp đường dẫn đến tài liệu phải được ký và thiết lập các tùy chọn văn bản và hình ảnh mong muốn của mã QR. Bạn có thể đặt hình ảnh mã QR đã tạo trên bất kỳ khu vực nào của bất kỳ trang tài liệu nào.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Chỉ định tài liệu để ký
            using (Signature signature = new Signature("source.docx"))
            {
                // Tạo tùy chọn ký hiệu mã QR
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // Đặt tùy chọn mã QR
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150,
                };

                // Ký và lưu tập tin đã xử lý
                SignResult result = signature.Sign("result.docx", options);
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Chỉ định tài liệu để ký
            Signature signature = new Signature("source.docx");

            // Tạo tùy chọn ký hiệu mã QR
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith");

            // Đặt tùy chọn mã QR
            options.setEncodeType(QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Ký và lưu tập tin đã xử lý
            signature.sign("result.docx", options);
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            const signatureLib = require('@groupdocs/groupdocs.signature')

            // Chỉ định tài liệu để ký
            const signature = new signatureLib.Signature('source.docx');

            // Tạo tùy chọn ký hiệu mã QR
            const options = new signatureLib.QrCodeSignOptions('JohnSmith');

            // Đặt tùy chọn mã QR
            options.setEncodeType(signatureLib.QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Ký và lưu tập tin đã xử lý
            signature.sign('result.docx', options);
            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "Hơn 60 định dạng tệp được hỗ trợ"
  description: "GroupDocs.Signature hỗ trợ hầu hết các định dạng tệp phổ biến"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Dữ liệu thống kê thư viện của chúng tôi"
  description: "Kiểm tra các số liệu sản phẩm chính, tiết lộ thông tin chuyên sâu về thành tựu, tác động và sự phát triển của chúng tôi"

  items:
    # items loop
    - number: "50+"
      title: "Các định dạng được hỗ trợ"
      content: "Ký hơn 60 định dạng tệp kinh doanh phổ biến nhất."

    # items loop
    - number: "500k"
      title: "Tải xuống NuGet"
      content: "GroupDocs.Signature cho .NET là thư viện phổ biến với hơn 550.000 lượt tải xuống trên NuGet."

    # items loop
    - number: "15k"
      title: "Tải xuống Maven"
      content: "Các nhà phát triển Java đã tải xuống GroupDocs.Signature trên Maven hơn 15 nghìn lần."

    # items loop
    - number: "140+"
      title: "Khách hàng hạnh phúc"
      content: "Các nhà phát triển cá nhân và các công ty hàng đầu trên toàn thế giới sử dụng sản phẩm của chúng tôi để xây dựng các giải pháp sáng tạo."


############################# Customers ###############################
customers:
  enable: true
  title: "Khách hàng hạnh phúc của chúng tôi"
  description: "Thư viện GroupDocs được các thương hiệu nổi tiếng và nổi tiếng trên toàn thế giới sử dụng"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Sẵn sàng để bắt đầu?"
  description: "Dùng thử miễn phí các tính năng của GroupDocs.Signature trên nền tảng của bạn"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/signature/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/signature/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/signature/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "Các câu hỏi thường gặp"
  description: "Khám phá các câu hỏi thường gặp của chúng tôi"

  items:
    # items loop
    - question: "GroupDocs.Signature có cần thư viện bên ngoài nào để ký tài liệu không?"
      answer: "Không, GroupDocs.Signature hoạt động độc lập. Không có sự phụ thuộc của bên thứ ba như Adobe Acrobat, Microsoft Office, v.v."

    # items loop
    - question: "Có thể thử nghiệm các tính năng của GroupDocs.Signature trước khi mua không?"
      answer: "Tuyệt đối! GroupDocs.Signature cung cấp bản dùng thử miễn phí. Hãy cài đặt nó và khám phá các tính năng của nó. Lưu ý rằng các phiên bản dùng thử sẽ thêm 'huy hiệu dùng thử' vào tài liệu của bạn và chỉ xử lý 3 trang đầu tiên. Để có trải nghiệm đầy đủ, hãy nhận giấy phép tạm thời 30 ngày miễn phí để truy cập tất cả các chức năng. Xem chi tiết trong [giấy phép tạm thời](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Những loại giấy phép nào được cung cấp?"
      answer: "Bạn đang tìm giấy phép GroupDocs.Signature? Chúng tôi cung cấp nhiều lựa chọn khác nhau phù hợp với nhu cầu của bạn. Chọn dựa trên quy mô nhóm, địa điểm triển khai (văn phòng đơn lẻ hoặc nơi làm việc từ xa) và liệu việc phân phối cho khách hàng cuối có yêu cầu chia sẻ SDK/API với khách hàng hay không. Ngoài ra, hãy chọn giấy phép sử dụng hàng tháng với các gói có đồng hồ đo—chỉ trả tiền cho những gì bạn sử dụng. Khám phá lựa chọn phù hợp nhất với bạn trong [giá](https://purchase.groupdocs.com/pricing/signature/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "API mã thấp GroupDocs.Signature"
  description: "Ký các tệp bằng ứng dụng của bạn thông qua API REST dựa trên đám mây của chúng tôi."
  
  items:
    # items loop
    - title: "GroupDocs.Signature Cloud for cURL"
      content: "Sử dụng cURL RESTful API để đặt chữ ký trên PDF, Word, Excel, PowerPoint, JPEG và nhiều định dạng tệp khác."
      icon: "groupdocs_signature-for-curl"
      link: "https://products.groupdocs.cloud/signature/curl"

    # items loop
    - title: "GroupDocs.Signature Cloud for .NET"
      content: "Làm phong phú thêm các ứng dụng .NET của bạn bằng cách ký tài liệu qua Cloud SDK. Bảo vệ tài liệu kinh doanh theo cách riêng của bạn."
      icon: "groupdocs_signature-for-net"
      link: "https://products.groupdocs.cloud/signature/net"

    # items loop
    - title: "GroupDocs.Signature Cloud for Java"
      content: "SDK GroupDocs.Signature cấp quyền truy cập vào nhiều khả năng khác nhau để ứng dụng Java của bạn ký bất kỳ tệp nào."
      icon: "groupdocs_signature-for-java"
      link: "https://products.groupdocs.cloud/signature/java"

############################# App links ###############################
app_links:
  enable: true
  title: "Ứng dụng web GroupDocs.Signature"
  description: "GroupDocs.Signature giới thiệu một ứng dụng web miễn phí nơi bạn có thể ký tài liệu. Hơn 60 định dạng tệp phổ biến có thể được ký MIỄN PHÍ thông qua trình duyệt yêu thích của bạn."

  items:
    # items loop
    - title: "GroupDocs.Signature Total"
      content: "Công cụ trực tuyến để đặt chữ ký trên tài liệu từ mọi thiết bị."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/signature/total"

    # items loop
    - title: "GroupDocs.Signature DOCX"
      content: "Ký MS Word DOCX trực tuyến."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/signature/docx"

    # items loop
    - title: "GroupDocs.Signature PDF"
      content: "Bảo vệ tài liệu PDF trực tuyến."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/signature/pdf"


      


---