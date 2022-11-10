---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Pptx
productName: Java
lang: vi
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Pptx for Java

############################# Head ############################
head_title: "Nối chữ ký điện tử Siêu dữ liệu vào tài liệu Pptx qua Java"
head_description: "Sử dụng Siêu dữ liệu làm chữ ký điện tử ẩn bên trong tài liệu Pptx của bạn bằng cách sử dụng một vài dòng mã Java. Sử dụng API chữ ký tài liệu GroupDocs để ký điện tử các tài liệu và tệp kinh doanh của bạn bằng thông tin Siêu dữ liệu."

############################# Header ############################
title: "Chữ ký điện tử siêu dữ liệu cho tài liệu Pptx qua Java rất đơn giản và dễ sử dụng!"
description: "eSign các tài liệu và hợp đồng Pptx của bạn bằng các mục nhập Siêu dữ liệu ẩn. Tạo Siêu dữ liệu cho các tệp PDF, tài liệu MS Word, sổ làm việc MS Excel, bản trình bày MS PowerPoint và các định dạng hình ảnh khác nhau mà không gặp sự cố và phải viết mã bổ sung."
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
    title: "Giới thiệu về GroupDocs.Signature for Java API chữ ký siêu dữ liệu"
    content: |
        [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) là một API phổ biến cho ký điện tử tài liệu kỹ thuật số. Các chữ ký như văn bản, hình ảnh, chứng chỉ kỹ thuật số, mã vạch, mã QR, tem hoặc siêu dữ liệu đều có sẵn. Chữ ký có thể được đặt trên các tệp PDF, tài liệu MS Word, sổ làm việc MS Excel, bản trình bày MS PowerPoint, tệp Adobe Photoshop và các định dạng hình ảnh khác nhau. Khách hàng có thể ký vào tài liệu của họ và cập nhật, tìm kiếm, xác minh, xóa hoặc xem trước các chữ ký điện tử đã được đưa vào các tài liệu đó. Hơn nữa, rất nhiều khả năng tùy chỉnh chữ ký được cung cấp.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Các bước để đăng nhập Pptx bằng Metadata trong Java"
    content_left: |
        [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) cung cấp khả năng ký các tài liệu Pptx bằng chữ ký Metadata một cách nhanh chóng và dễ dàng.
        
        * Tạo một phiên bản của lớp Chữ ký cung cấp tệp Pptx phải ký dưới dạng đường dẫn hoặc luồng bộ nhớ
        * Khởi tạo lớp SignOptions và thiết lập tất cả dữ liệu được yêu cầu.
        * Gọi phương thức Signature.Sign () chuyển đầu ra tệp Pptx hoặc luồng bộ nhớ

    title_right: " yêu cầu hệ thống"
    content_right: |
        GroupDocs.Signature for Java được hỗ trợ trên tất cả các nền tảng và hệ điều hành chính. Trước khi thực hiện mã bên dưới, hãy đảm bảo rằng bạn đã cài đặt các điều kiện tiên quyết sau trên hệ thống của mình.

        * Hệ điều hành: Microsoft Windows, Linux, MacOS
        * Môi trường phát triển: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Nhận GroupDocs.Signature for Java mới nhất từ ​​[Maven] (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pptx file
        String filePath = "input.pptx";
        // Set up output file
        String outputFilePath = "output.pptx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Pptx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ký tài liệu Pptx bằng Metadata Live Demo"
    content: |
       Ký tệp Pptx bằng nhiều chữ ký ngay bây giờ bằng cách truy cập trang web [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). Bản demo trực tuyến miễn phí đang chờ bạn.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Các chữ ký Metadata được hỗ trợ khác cho Java"
    content: |
        "Bạn cũng có thể ký Pptx bằng các loại chữ ký khác. Vui lòng xem danh sách bên dưới."
    format: 
       
       
back_to_top:
    enable: true
---