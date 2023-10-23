---
############################# Static ############################
layout: "landing"
date: 2023-10-23T14:58:09
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
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, API đám mây & Ứng dụng chữ ký tài liệu trực tuyến"
head_description: "Sở hữu giải pháp chữ ký điện tử tất cả trong một cho các ứng dụng .NET, Java và đám mây. Ký các định dạng tài liệu phổ biến trực tuyến bằng tính năng kéo và thả đơn giản"

############################# Header ############################
title: "Ký văn bản<br>thông qua API Java"
description: "Ký các tài liệu và hình ảnh kỹ thuật số trên bất kỳ nền tảng nào bằng cách sử dụng các giải pháp dựa trên ứng dụng và API linh hoạt của chúng tôi dành cho lập trình viên và người dùng cuối."
words:
  for: "vì"

actions:
  main: "Tải xuống Maven miễn phí"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Cấp phép"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Sẵn sàng để bắt đầu?"
  description: "Dùng thử miễn phí các tính năng của GroupDocs.Signature hoặc yêu cầu giấy phép"

release:
  title: "Đã phát hành phiên bản {0}"
  notes: "Xem có gì mới"
  downloads: "Tải xuống"

code:
  title: "Ký các tệp PDF trong Java"
  more: "Thêm ví dụ"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Chọn tài liệu PDF
    Signature signature = new Signature("sample.pdf");
    
    // Cung cấp văn bản
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Ký tài liệu và lưu vào tập tin
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Tổng quan về GroupDocs.Signature"
  description: "API để thực hiện ký tài liệu và các hoạt động liên quan trong ứng dụng Java"
  features:
    # feature loop
    - title: "Tài liệu kinh doanh được cải thiện với chữ ký số trong Java"
      content: "Ký nhanh chóng và có thể tùy chỉnh: GroupDocs.Signature cho Java cung cấp nhiều tùy chọn chữ ký số cho tệp PDF, hình ảnh và tài liệu Office. Bạn có thể sử dụng văn bản, mã vạch, mã QR, chứng chỉ kỹ thuật số, hình ảnh hoặc siêu dữ liệu ẩn. Quá trình xử lý tài liệu nhanh chóng và hiệu quả."

    # feature loop
    - title: "Thao tác các tài liệu đã ký"
      content: "Xử lý tài liệu nâng cao bao gồm các thao tác mạnh mẽ trên các tài liệu đã ký bằng GroupDocs.Signature cho Java. Bạn có thể tìm kiếm và xác thực chữ ký đã được thêm vào tài liệu kinh doanh bằng nhiều tiêu chí hữu ích khác nhau. Ngoài ra, bạn có thể truy cập thông tin chi tiết về tài liệu hoặc lấy hình ảnh xem trước của các trang trong tài liệu."

    # feature loop
    - title: "Sự lựa chọn đầu ra đa dạng"
      content: "Các tùy chọn ký mạnh mẽ cho phép bạn tùy chỉnh đầu ra cho các tài liệu được ký bằng GroupDocs.Signature cho Java. Bạn có thể định vị chính xác bất kỳ chữ ký nào trên bất kỳ trang tài liệu nào và định cấu hình giao diện của nó theo nhiều cách khác nhau. API Java hỗ trợ lưu các tài liệu kinh doanh đã ký ở nhiều định dạng được hỗ trợ và cung cấp các tùy chọn để bảo mật chúng bằng mật khẩu."

############################# Platforms ############################
platforms:
  enable: true
  title: "Nền tảng độc lập"
  description: "GroupDocs.Signature cho Java hỗ trợ các hệ điều hành, khung và trình quản lý gói sau"
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Các định dạng tập tin được hỗ trợ"
  description: |
    GroupDocs.Signature cho Java hỗ trợ các thao tác với [định dạng tệp](https://docs.groupdocs.com/signature/java/supported-document-formats/) sau.
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
  description: "Ký các tệp PDF, Tài liệu Office và hình ảnh bằng chữ ký số"

  items:
    # feature loop
    - icon: "sign"
      title: "Thêm chữ ký"
      content: "Ký tài liệu bằng nhiều loại chữ ký được hỗ trợ khác nhau bằng cách đặt chữ ký điện tử chính xác ở bất kỳ vị trí nào trên bất kỳ trang nào."

    # feature loop
    - icon: "custom"
      title: "Tùy chỉnh kết quả"
      content: "Tùy chỉnh giao diện chữ ký bằng cách điều chỉnh màu sắc, phông chữ, đường viền, xoay và các tính năng khác để đạt được kết quả mong muốn."

    # feature loop
    - icon: "password"
      title: "Bảo mật tài liệu bằng mật khẩu"
      content: "Đối với nhiều loại tài liệu được hỗ trợ, bạn có thể bảo vệ tài liệu đã ký bằng mật khẩu."

    # feature loop
    - icon: "protect"
      title: "Ngăn chặn những thay đổi trái phép"
      content: "Bảo vệ các tài liệu kinh doanh quan trọng được ký bằng chứng chỉ kỹ thuật số khỏi những sửa đổi trái phép."

    # feature loop
    - icon: "convert"
      title: "Thu được kết quả ở định dạng mong muốn"
      content: "Dễ dàng có được các tệp kết quả đã ký ở bất kỳ định dạng được hỗ trợ nào. Bạn cũng có thể chuyển đổi tài liệu MS Word sang PDF một cách dễ dàng."

    # feature loop
    - icon: "preview"
      title: "Xem trước tài liệu"
      content: "Lưu bất kỳ trang nào của tài liệu dưới dạng hình ảnh để xử lý trong tương lai."

    # feature loop
    - icon: "search"
      title: "Tìm kiếm chữ ký"
      content: "Có thể lấy thông tin về chữ ký đã thêm trước đó trong các tài liệu cụ thể."

    # feature loop
    - icon: "validate"
      title: "Xác thực tài liệu"
      content: "Xác thực tính chính xác của chữ ký trên bất kỳ tài liệu đã ký nào."

    # feature loop
    - icon: "update"
      title: "Quản lý chữ ký"
      content: "Sau khi chữ ký được đặt trên trang tài liệu, nó có thể bị xóa, di chuyển hoặc cập nhật nếu cần."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mẫu mã"
  description: "Một số trường hợp sử dụng GroupDocs.Signature điển hình cho các hoạt động Java"
  items:
    # code sample loop
    - title: "Nâng cao tài liệu PDF bằng mã QR"
      content: |
        Nâng cao quy trình kinh doanh bằng cách thêm [mã QR](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) vào các trang cụ thể của tài liệu PDF có thể có giá trị. Có một ví dụ về cách thêm mã QR bằng GroupDocs.Signature cho Java.
        {{< landing/code title="Nâng cao tài liệu PDF bằng mã QR">}}
        ```java {style=abap}
        // Tải tài liệu để ký
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Tạo tùy chọn mã QR với văn bản được xác định trước
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Định cấu hình loại và vị trí mã hóa mã QR trên trang
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Ký tài liệu và lưu nó dưới dạng tệp kết quả
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Sử dụng chữ ký số để bảo vệ DOCX"
      content: |
        Bạn có thể [Bảo vệ tài liệu](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) bằng chữ ký cá nhân hoặc công ty được lưu trữ dưới dạng chứng chỉ kỹ thuật số. Các tài liệu được bảo đảm bằng chứng chỉ không thể bị thay đổi nếu không làm mất hiệu lực chữ ký.
        {{< landing/code title="Sử dụng chữ ký số để bảo vệ DOCX">}}
        ```java {style=abap}   
        // Tải tài liệu cần được ký điện tử
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Chỉ định các tùy chọn ký kỹ thuật số và cung cấp đường dẫn đến tệp chứng chỉ
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Đặt mật khẩu chứng chỉ
        options.setPassword("1234567890");

        // Ký tài liệu và lưu nó vào đường dẫn mong muốn
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
