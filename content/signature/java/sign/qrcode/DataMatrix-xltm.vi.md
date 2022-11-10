---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: Data Matrix
fileformat: Xltm
productName: Java
lang: vi
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on Xltm for Java

############################# Head ############################
head_title: "eSign Xltm tài liệu với Data Matrix Mã QR trong Java"
head_description: "Tạo Mã QR Data Matrix và đặt nó vào tệp Xltm bằng cách sử dụng Java với một đoạn mã Java ngắn. Sử dụng API chữ ký tài liệu GroupDocs để ký điện tử các tài liệu và tệp doanh nghiệp của bạn bằng Mã QR."

############################# Header ############################
title: "Tạo chữ ký Mã QR Data Matrix cho tài liệu Xltm trong Java"
description: "eSign các tài liệu và hợp đồng Xltm của bạn bằng Mã QR Data Matrix. Tạo chữ ký Mã QR nhanh chóng và dễ dàng."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Giới thiệu về GroupDocs.Signature for Java API chữ ký mã QR"
    content: |
        [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) là một API hoàn thiện để tạo và tạo chữ ký Mã QR cho tài liệu. Người dùng có thể tạo chữ ký Mã QR cung cấp văn bản để tải xuống hoặc chia sẻ trên phương tiện truyền thông xã hội dưới dạng hình ảnh. Tài liệu đã ký có thể được quét bằng API hoặc đơn giản qua camera di động! Ký điện tử các hợp đồng kinh doanh và tài liệu chính thức của bạn bằng cách thêm chữ ký Mã QR và thao tác với nó. Bất kỳ chữ ký Mã QR nào cũng sẽ chứa thông tin tùy chỉnh duy nhất để xác định người ký hoặc ủy quyền tài liệu. Hơn nữa, nội dung Mã QR có thể được mã hóa và giải mã bằng các khóa cá nhân theo lập trình. Điều đó mở ra nhiều khả năng chia sẻ dữ liệu nhạy cảm bên trong các tài liệu công khai. Sau khi ký, người dùng có thể cập nhật, xác minh, xóa, xem trước hoặc tìm kiếm Mã QR trong các tệp PDF, tài liệu MS Word, sổ làm việc MS Excel, bản trình bày MS PowerPoint, tệp Adobe Photoshop và các định dạng hình ảnh khác nhau. Mã QR có thể được tùy chỉnh bổ sung.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Các bước để đăng nhập Xltm bằng Qrcode trong Java"
    content_left: |
        [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) cung cấp khả năng ký các tài liệu Xltm bằng chữ ký Qrcode một cách nhanh chóng và dễ dàng.
        
        * Tạo một phiên bản của lớp Chữ ký cung cấp tệp Xltm phải ký dưới dạng đường dẫn hoặc luồng bộ nhớ
        * Khởi tạo lớp SignOptions và thiết lập tất cả dữ liệu được yêu cầu.
        * Gọi phương thức Signature.Sign () chuyển đầu ra tệp Xltm hoặc luồng bộ nhớ

    title_right: " yêu cầu hệ thống"
    content_right: |
        GroupDocs.Signature for Java được hỗ trợ trên tất cả các nền tảng và hệ điều hành chính. Trước khi thực hiện mã bên dưới, hãy đảm bảo rằng bạn đã cài đặt các điều kiện tiên quyết sau trên hệ thống của mình.

        * Hệ điều hành: Microsoft Windows, Linux, MacOS
        * Môi trường phát triển: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Nhận GroupDocs.Signature for Java mới nhất từ ​​[Maven] (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xltm file
        String filePath = "input.xltm";
        // Set up output file
        String outputFilePath = "output.xltm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(QrCodeTypes.Data Matrix);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Xltm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ký tài liệu Xltm bằng Qrcode Live Demo"
    content: |
       Ký tệp Xltm bằng nhiều chữ ký ngay bây giờ bằng cách truy cập trang web [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). Bản demo trực tuyến miễn phí đang chờ bạn.

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Data Matrix QrCode"
          content: |
            Ma trận dữ liệu là một mã hai chiều bao gồm các 'ô' hoặc chấm màu đen và trắng được sắp xếp theo hình vuông hoặc hình chữ nhật, còn được gọi là ma trận. Thông tin được mã hóa có thể là dữ liệu văn bản hoặc số.
          characterset: |
             Hỗ trợ tất cả 256 ký tự ASCII, tất cả các ký tự ISO và tất cả các ký tự Mã trao đổi thập phân được mã hóa nhị phân mở rộng (EBCDIC).
          textcapacity: |
             Lên đến 3116 ký tự số hoặc 2335 ký tự số alpha hoặc 1556 ký tự nhị phân.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Các chữ ký Qrcode được hỗ trợ khác cho Java"
    content: |
        "Bạn cũng có thể ký Xltm bằng các loại chữ ký khác. Vui lòng xem danh sách bên dưới."
    format: 
        
       
back_to_top:
    enable: true
---