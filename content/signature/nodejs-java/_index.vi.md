---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: vi
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET, Java, API đám mây & Ứng dụng chữ ký tài liệu trực tuyến"
head_description: "Sở hữu giải pháp chữ ký điện tử tất cả trong một cho các ứng dụng .NET, Java và đám mây. Ký các định dạng tài liệu phổ biến trực tuyến bằng tính năng kéo và thả đơn giản"

############################# Header ############################
title: "Ký văn bản<br>với API Node.js"
description: "Ký các tài liệu và hình ảnh kỹ thuật số trên bất kỳ nền tảng nào bằng cách sử dụng các giải pháp dựa trên ứng dụng và API linh hoạt của chúng tôi dành cho lập trình viên và người dùng cuối."
words:
  for: "vì"

actions:
  main: "Tải xuống từ NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Cấp phép"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Sẵn sàng để bắt đầu?"
  description: "Dùng thử miễn phí các tính năng của GroupDocs.Signature hoặc yêu cầu giấy phép"

release:
  title: "Đã phát hành phiên bản {0}"
  notes: "Xem có gì mới"
  downloads: "Tải xuống"

code:
  title: "Ký tệp PDF bằng Node.js"
  more: "Thêm ví dụ"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Chọn tài liệu PDF
    let signature = new Signature("sample.pdf");
    
    // Cung cấp văn bản
    let options = new TextSignOptions("John Smith");
    
    // Đặt màu
    options.ForeColor = Color.Red;
    
    // Ký tài liệu và lưu vào tập tin
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Tổng quan về GroupDocs.Signature"
  description: "Thư viện ký tài liệu đã sẵn sàng để sử dụng trong các ứng dụng Node.js"
  features:
    # feature loop
    - title: "Giải pháp chữ ký số cho tài liệu doanh nghiệp với Node.js"
      content: "GroupDocs.Signature for Node.js via Java cung cấp một bộ tùy chọn chữ ký số toàn diện cho tài liệu PDF, Office và hình ảnh. Văn bản, mã vạch, hình ảnh, chứng chỉ kỹ thuật số và siêu dữ liệu đều có sẵn. Xử lý tài liệu hợp lý đảm bảo hiệu quả."

    # feature loop
    - title: "Thao tác nâng cao của các tài liệu đã ký"
      content: "GroupDocs.Signature trao quyền cho bạn xử lý các tài liệu đã ký. Tìm kiếm và xác thực chữ ký bằng nhiều tiêu chí khác nhau. Ngoài ra, trích xuất thông tin tài liệu chi tiết hoặc tạo hình ảnh xem trước của các trang."

    # feature loop
    - title: "Định dạng đầu ra đa dạng"
      content: "Giải pháp của chúng tôi cung cấp khả năng kiểm soát rộng rãi đối với định dạng đầu ra của tài liệu đã ký. Định vị chính xác chữ ký trên bất kỳ trang nào và tùy chỉnh giao diện của chúng. Lưu tài liệu đã ký ở nhiều định dạng được hỗ trợ và tùy chọn bảo mật chúng bằng mật khẩu."

############################# Platforms ############################
platforms:
  enable: true
  title: "Nền tảng độc lập"
  description: "GroupDocs.Signature for Node.js via Java thực hiện xử lý tài liệu với nhiều hệ điều hành khác nhau"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Các định dạng tập tin được hỗ trợ"
  description: |
    GroupDocs.Signature for Node.js via Java tạo điều kiện thuận lợi cho hoạt động của [các định dạng tệp phổ biến](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Các định dạng Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Hình ảnh & Định dạng khác
        * **Cầm tay:** PDF
        * **Hình ảnh:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Các dạng văn phòng khác:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Các định dạng khác
        * **Web:** HTML, MHTML
        * **Lưu trữ:** ZIP, TAR, 7Z
        * **Chứng chỉ:** PFX

############################# Features ############################
features:
  enable: true
  title: "Đặc điểm của GroupDocs.Signature"
  description: "Ký các tệp PDF, tài liệu Office và hình ảnh bằng chữ ký số"

  items:
    # feature loop
    - icon: "sign"
      title: "Chữ ký doanh nghiệp"
      content: "Sử dụng nhiều loại chữ ký khác nhau để ký tài liệu. Đặt chữ ký số chính xác trên bất kỳ vị trí trang nào."

    # feature loop
    - icon: "custom"
      title: "Tùy chỉnh giao diện chữ ký"
      content: "Điều chỉnh khía cạnh trực quan của chữ ký bằng cách điều chỉnh màu sắc, phông chữ, đường viền, xoay, v.v. để đạt được kết quả mong muốn."

    # feature loop
    - icon: "password"
      title: "Tài liệu được bảo vệ bằng mật khẩu"
      content: "Đối với nhiều định dạng tài liệu được hỗ trợ, hãy bảo vệ tài liệu đã ký bằng mật khẩu để tăng cường bảo mật."

    # feature loop
    - icon: "protect"
      title: "Ngăn chặn các sửa đổi trái phép"
      content: "Bảo vệ các tài liệu kinh doanh quan trọng được ký bằng chứng chỉ kỹ thuật số khỏi những thay đổi trái phép."

    # feature loop
    - icon: "convert"
      title: "Định dạng đầu ra mong muốn"
      content: "Dễ dàng nhận được tài liệu đã ký ở bất kỳ định dạng được hỗ trợ nào. Chuyển đổi tài liệu MS Word sang định dạng PDF một cách dễ dàng."

    # feature loop
    - icon: "preview"
      title: "Xem trước tài liệu"
      content: "Lưu các trang tài liệu riêng lẻ dưới dạng hình ảnh cho nhu cầu trong tương lai."

    # feature loop
    - icon: "search"
      title: "Tìm kiếm chữ ký"
      content: "Truy xuất thông tin về chữ ký đã thêm trước đó trong tài liệu của bạn."

    # feature loop
    - icon: "validate"
      title: "Xác thực tài liệu"
      content: "Xác minh tính xác thực của chữ ký được trình bày trong bất kỳ tài liệu nào."

    # feature loop
    - icon: "update"
      title: "Quản lý chữ ký"
      content: "Xóa, di chuyển hoặc sửa đổi bất kỳ chữ ký nào được đặt trên bất kỳ trang tài liệu nào."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mẫu mã"
  description: "Các ví dụ minh họa thể hiện các thao tác GroupDocs.Signature for Node.js via Java điển hình"
  items:
    # code sample loop
    - title: "Đánh dấu PDF bằng mã QR"
      content: |
        Việc kết hợp [mã vạch](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) vào các trang tài liệu PDF cụ thể có thể đơn giản hóa quy trình kinh doanh. Phần này cung cấp ví dụ về cách thêm mã QR bằng cách sử dụng GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Cách đặt mã QR vào PDF.">}}
        ```javascript {style=abap}
        // Tải tài liệu để ký
        let signature = new Signature("file_to_sign.pdf");
        
        // Tạo tùy chọn mã QR với văn bản được xác định trước
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Định cấu hình loại và vị trí mã hóa mã QR trên trang
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Ký tài liệu và lưu nó dưới dạng tệp kết quả
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Bảo vệ DOCX bằng chữ ký số"
      content: |
        [Bảo vệ tài liệu của bạn](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) bằng chữ ký dựa trên chứng chỉ kỹ thuật số. Chữ ký số bảo vệ tài liệu kinh doanh của bạn khỏi bị thay đổi nội dung.
        {{< landing/code title="Đây là cách đảm bảo tính toàn vẹn của tài liệu.">}}
        ```javascript {style=abap}   
        // Tải tài liệu cần được ký điện tử
        let signature = new Signature("file_to_sign.docx");
        
        // Chỉ định các tùy chọn ký kỹ thuật số và cung cấp đường dẫn đến tệp chứng chỉ
        let options = new DigitalSignOptions("certificate.pfx");

        // Đặt mật khẩu chứng chỉ
        options.Password = "1234567890";

        // Ký tài liệu và lưu nó vào đường dẫn mong muốn
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
