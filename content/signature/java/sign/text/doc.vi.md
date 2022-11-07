---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Doc
productName: Java
lang: vi
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Doc for Java

############################# Head ############################
head_title: "Tạo chữ ký điện tử Văn bản vào tệp Doc với Java"
head_description: "Đặt Text eSignature vào tệp Doc cho Java bằng cách sử dụng một vài dòng mã. Sử dụng API chữ ký tài liệu GroupDocs để ký hàng chục định dạng tệp."

############################# Header ############################
title: "Ký các tệp Doc bằng chữ ký Text trong Java"
description: "Cách thêm Chữ ký Text bằng một vài dòng mã Java"
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
    title: "Giới thiệu về API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) là một API phổ biến cho ký điện tử tài liệu kỹ thuật số. Các chữ ký như văn bản, hình ảnh, chứng chỉ kỹ thuật số, mã vạch, mã QR, tem hoặc siêu dữ liệu đều có sẵn. Chữ ký có thể được đặt trên các tệp PDF, tài liệu MS Word, sổ làm việc MS Excel, bản trình bày MS PowerPoint, tệp Adobe Photoshop và các định dạng hình ảnh khác nhau. Khách hàng có thể ký vào tài liệu của họ và cập nhật, tìm kiếm, xác minh, xóa hoặc xem trước các chữ ký điện tử đã được đưa vào các tài liệu đó. Hơn nữa, rất nhiều khả năng tùy chỉnh chữ ký được cung cấp.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Các bước để đăng nhập Doc bằng Text trong Java"
    content_left: |
        [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) cung cấp khả năng ký các tài liệu Doc bằng chữ ký Text một cách nhanh chóng và dễ dàng.
        
        * Tạo một phiên bản của lớp Chữ ký cung cấp tệp Doc phải ký dưới dạng đường dẫn hoặc luồng bộ nhớ
        * Khởi tạo lớp SignOptions và thiết lập tất cả dữ liệu được yêu cầu.
        * Gọi phương thức Signature.Sign () chuyển đầu ra tệp Doc hoặc luồng bộ nhớ

    title_right: " yêu cầu hệ thống"
    content_right: |
        GroupDocs.Signature for Java được hỗ trợ trên tất cả các nền tảng và hệ điều hành chính. Trước khi thực hiện mã bên dưới, hãy đảm bảo rằng bạn đã cài đặt các điều kiện tiên quyết sau trên hệ thống của mình.

        * Hệ điều hành: Microsoft Windows, Linux, MacOS
        * Môi trường phát triển: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Nhận GroupDocs.Signature for Java mới nhất từ ​​[Maven] (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Doc file
        String filePath = "input.doc";
        // Set up output file
        String outputFilePath = "output.doc";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Doc document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ký tài liệu Doc bằng Text Live Demo"
    content: |
       Ký tệp Doc bằng nhiều chữ ký ngay bây giờ bằng cách truy cập trang web [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). Bản demo trực tuyến miễn phí đang chờ bạn.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Các chữ ký Text được hỗ trợ khác cho Java"
    content: |
        "Bạn cũng có thể ký Doc bằng các loại chữ ký khác. Vui lòng xem danh sách bên dưới."
    format: 
       
       
back_to_top:
    enable: true
---