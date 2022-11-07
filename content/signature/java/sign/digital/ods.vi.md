---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Ods
productName: Java
lang: vi
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ods for Java

############################# Head ############################
head_title: "Thêm chữ ký điện tử kỹ thuật số vào tệp Ods với Java"
head_description: "Đặt Chữ ký số vào tệp Ods cho Java bằng cách sử dụng một vài dòng mã. Sử dụng API chữ ký tài liệu GroupDocs để ký hàng chục định dạng tệp."

############################# Header ############################
title: "eSign các tệp Ods có chữ ký Digital trong Java"
description: "Cách thêm chữ ký Digital với một vài dòng mã Java"
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
    title: "Giới thiệu về GroupDocs.Signature for Java API chữ ký điện tử"
    content: |
        [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) là một API phổ biến để ký kết tài liệu bằng chữ ký điện tử kỹ thuật số, với chứng chỉ kỹ thuật số. Đối với API chữ ký điện tử, sử dụng tệp chứng chỉ PFX để ký kết tài liệu bằng khóa riêng và khóa công khai được bảo vệ bằng mật khẩu. Chữ ký điện tử có thể được sử dụng để xác nhận các tài liệu kinh doanh với trang eSign PDF cụ thể, xác nhận toàn bộ tài liệu Microsoft Office như tệp Words, Excel, Powerpoint và tài liệu Open Office. Khách hàng có thể dễ dàng thao tác trên chữ ký như chỉnh sửa, xóa bỏ, điều chỉnh. API cung cấp một cách để tìm kiếm và xác minh chữ ký. Hơn nữa, rất nhiều khả năng tùy chỉnh chữ ký được cung cấp.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Các bước để đăng nhập Ods bằng Digital trong Java"
    content_left: |
        [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) cung cấp khả năng ký các tài liệu Ods bằng chữ ký Digital một cách nhanh chóng và dễ dàng.
        
        * Tạo một phiên bản của lớp Chữ ký cung cấp tệp Ods phải ký dưới dạng đường dẫn hoặc luồng bộ nhớ
        * Khởi tạo lớp SignOptions và thiết lập tất cả dữ liệu được yêu cầu.
        * Gọi phương thức Signature.Sign () chuyển đầu ra tệp Ods hoặc luồng bộ nhớ

    title_right: " yêu cầu hệ thống"
    content_right: |
        GroupDocs.Signature for Java được hỗ trợ trên tất cả các nền tảng và hệ điều hành chính. Trước khi thực hiện mã bên dưới, hãy đảm bảo rằng bạn đã cài đặt các điều kiện tiên quyết sau trên hệ thống của mình.

        * Hệ điều hành: Microsoft Windows, Linux, MacOS
        * Môi trường phát triển: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Nhận GroupDocs.Signature for Java mới nhất từ ​​[Maven] (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ods file
        String filePath = "input.ods";
        // Set up output file
        String outputFilePath = "output.ods";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Ods document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ký tài liệu Ods bằng Digital Live Demo"
    content: |
       Ký tệp Ods bằng nhiều chữ ký ngay bây giờ bằng cách truy cập trang web [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). Bản demo trực tuyến miễn phí đang chờ bạn.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Các chữ ký Digital được hỗ trợ khác cho Java"
    content: |
        "Bạn cũng có thể ký Ods bằng các loại chữ ký khác. Vui lòng xem danh sách bên dưới."
    format: 
       
       
back_to_top:
    enable: true
---