---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:23
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: vi
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, API đám mây & Ứng dụng chữ ký tài liệu trực tuyến"
head_description: "Sở hữu giải pháp chữ ký điện tử tất cả trong một cho các ứng dụng .NET, Java và đám mây. Ký các định dạng tài liệu phổ biến trực tuyến bằng tính năng kéo và thả đơn giản"

############################# Header ############################
title: "Ký văn bản<br>thông qua API .NET"
description: "Ký các tài liệu và hình ảnh kỹ thuật số trên bất kỳ nền tảng nào bằng cách sử dụng các giải pháp dựa trên ứng dụng và API linh hoạt của chúng tôi dành cho lập trình viên và người dùng cuối."
words:
  for: "vì"

actions:
  main: "Tải xuống NuGet miễn phí"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Cấp phép"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Sẵn sàng để bắt đầu?"
  description: "Dùng thử miễn phí các tính năng của GroupDocs.Signature hoặc yêu cầu giấy phép"

release:
  title: "Đã phát hành phiên bản {0}"
  notes: "Xem có gì mới"
  downloads: "Tải xuống"

code:
  title: "Ký tệp PDF trong C#"
  more: "Thêm ví dụ"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Chọn tài liệu PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Cung cấp văn bản
        var options = new TextSignOptions("John Smith")
        {
            // Đặt màu
            ForeColor = Color.Red
        };
        // Ký tài liệu và lưu vào tập tin
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Tổng quan về GroupDocs.Signature"
  description: "API để thực hiện ký tài liệu và các hoạt động liên quan trong ứng dụng .NET"
  features:
    # feature loop
    - title: "Thêm chữ ký vào tài liệu kinh doanh trong C#"
      content: "Ký tài liệu: Với GroupDocs.Signature cho .NET, bạn có thể thêm nhiều loại chữ ký khác nhau, chẳng hạn như văn bản, hình ảnh, mã vạch và chứng chỉ kỹ thuật số vào tài liệu PDF và Office. API này cho phép bạn ký tài liệu của mình với hầu hết mọi loại dữ liệu, bao gồm cả siêu dữ liệu ẩn."

    # feature loop
    - title: "Xử lý văn bản đã ký"
      content: "Xử lý bổ sung: Bạn có thể thực hiện các thao tác mạnh mẽ trên các tài liệu đã ký bằng GroupDocs.Signature. Điều này bao gồm tìm kiếm chữ ký hiện có trong tài liệu kinh doanh và xác minh chúng bằng các tiêu chí cụ thể. Ngoài ra, bạn có thể truy xuất thông tin tài liệu và xem trước các trang thông qua API .NET này."

    # feature loop
    - title: "Tùy chỉnh kết quả"
      content: "GroupDocs.Signature cho .NET cung cấp các tùy chọn tùy chỉnh mở rộng. Bạn có thể định vị chính xác chữ ký ở bất kỳ đâu trên trang tài liệu và điều chỉnh giao diện của chúng bằng nhiều cài đặt khác nhau. Hơn nữa, API này hỗ trợ lưu các tài liệu đã xử lý ở nhiều định dạng được hỗ trợ."

############################# Platforms ############################
platforms:
  enable: true
  title: "Nền tảng độc lập"
  description: "GroupDocs.Signature cho .NET hỗ trợ các hệ điều hành, khung và trình quản lý gói sau"
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
    GroupDocs.Signature cho .NET hỗ trợ các thao tác với [định dạng tệp](https://docs.groupdocs.com/signature/net/supported-document-formats/) sau.
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
  title: "Tính năng GroupDocs.Signature"
  description: "Ký các tệp PDF, Tài liệu Office và Hình ảnh nhanh chóng và chính xác"

  items:
    # feature loop
    - icon: "sign"
      title: "Ký tài liệu"
      content: "Thêm một hoặc nhiều loại chữ ký được hỗ trợ một cách chính xác tại bất kỳ vị trí nào được chỉ định trên tài liệu kinh doanh."

    # feature loop
    - icon: "custom"
      title: "Tùy chỉnh chữ ký"
      content: "Sử dụng các tính năng như màu sắc, phông chữ, đường viền, xoay, v.v. để định cấu hình giao diện của chữ ký."

    # feature loop
    - icon: "password"
      title: "Bảo vệ mật khẩu tài liệu"
      content: "Bảo mật một số loại tài liệu nhất định bằng cách đặt mật khẩu sau khi ký."

    # feature loop
    - icon: "protect"
      title: "Bảo vệ khỏi những thay đổi"
      content: "Ngăn chặn những thay đổi đối với các tài liệu kinh doanh quan trọng sau khi thêm chữ ký bằng chứng chỉ số."

    # feature loop
    - icon: "convert"
      title: "Chuyển đổi tập tin đã ký sang các định dạng khác"
      content: "Chuyển đổi các tệp đã ký sang các định dạng mong muốn, chẳng hạn như lưu tài liệu Word dưới dạng PDF."

    # feature loop
    - icon: "preview"
      title: "Trích xuất bản xem trước trang"
      content: "Trích xuất các trang từ tài liệu đã ký dưới dạng hình ảnh riêng lẻ để xử lý trong tương lai."

    # feature loop
    - icon: "search"
      title: "Tìm kiếm chữ ký trong tài liệu"
      content: "Truy xuất thông tin về chữ ký đã thêm trước đó trong các tài liệu cụ thể."

    # feature loop
    - icon: "validate"
      title: "Xác thực các tài liệu đã ký"
      content: "Xác minh việc ký tài liệu phù hợp bằng cách sử dụng các tính năng xác thực."

    # feature loop
    - icon: "update"
      title: "Cập nhật hoặc xóa chữ ký"
      content: "Dễ dàng định vị lại các chữ ký cụ thể trên một trang, sửa đổi văn bản hoặc xóa chúng mà không gặp bất kỳ sự cố nào."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mẫu mã"
  description: "Một số trường hợp sử dụng GroupDocs.Signature điển hình cho các hoạt động .NET"
  items:
    # code sample loop
    - title: "Thêm mã QR vào PDF"
      content: |
        Việc thêm [mã QR](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) vào các trang cụ thể của tài liệu PDF có thể nâng cao quy trình kinh doanh. Dưới đây là ví dụ về cách thêm mã QR bằng GroupDocs.Signature.
        {{< landing/code title="Cách đặt mã QR vào PDF.">}}
        ```csharp {style=abap}
        // Tải tài liệu để ký
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Tạo tùy chọn mã QR với văn bản được xác định trước
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Định cấu hình loại và vị trí mã hóa mã QR trên trang
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Ký tài liệu và lưu nó dưới dạng tệp kết quả
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Bảo vệ tài liệu DOCX bằng chứng chỉ kỹ thuật số"
      content: |
        Bạn có thể [Bảo vệ tài liệu](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) bằng chữ ký cá nhân hoặc công ty được lưu trữ dưới dạng chứng chỉ kỹ thuật số. Những tài liệu được bảo vệ như vậy không thể được sửa đổi nếu không làm mất hiệu lực chữ ký.
        {{< landing/code title="Đây là cách đảm bảo tính toàn vẹn của tài liệu.">}}
        ```csharp {style=abap}   
        // Tải tài liệu cần được ký điện tử
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Chỉ định các tùy chọn ký kỹ thuật số và cung cấp đường dẫn đến tệp chứng chỉ
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Đặt mật khẩu chứng chỉ
                Password = "1234567890"
            };
            // Ký tài liệu và lưu nó vào đường dẫn mong muốn
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
