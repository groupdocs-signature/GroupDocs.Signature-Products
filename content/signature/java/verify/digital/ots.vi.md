---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Ots
productName: Java
lang: vi
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ots for Java

############################# Head ############################
head_title: "Xác minh chữ ký Digital cho tệp Ots qua Java"
head_description: "Chỉ sử dụng một vài dòng mã Java để xác minh tài liệu Ots và chữ ký Digital của chúng."

############################# Header ############################
title: "Xác minh chữ ký Digital cho các tệp Ots"
description: "API cho Java cung cấp cơ hội xác minh chữ ký Digital tại tài liệu Ots. Việc xác minh chữ ký điện tử bên trong tài liệu Ots của bạn có thể được thực hiện nhanh chóng và dễ dàng."
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
    title: "Khám phá các tính năng mới của API GroupDocs.Signature for Java"
    content: |
        API [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) cung cấp nhiều cách để xử lý nhiều định dạng tài liệu bằng cách sử dụng chữ ký điện tử. Nhiều loại chữ ký điện tử như văn bản, hình ảnh, chứng chỉ kỹ thuật số, mã vạch, mã QR, tem hoặc siêu dữ liệu được hỗ trợ. Khách hàng có thể thêm, bớt, chỉnh sửa, xác thực hoặc tìm kiếm chữ ký điện tử tại các tệp PDF, tài liệu MS Word, sổ làm việc MS Excel, bản trình bày MS PowerPoint, tệp Adobe Photoshop và các định dạng hình ảnh khác nhau. Có sẵn một số tính năng và cài đặt bổ sung đáng kinh ngạc.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cách xác thực chữ ký Digital trong tài liệu Ots của bạn"
    content_left: |
        [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) bao gồm các tính năng hữu ích như xác minh chữ ký Digital được đặt trong tài liệu Ots. Sử dụng cơ hội này mà không cần triển khai thêm mã.
        
        * Thứ nhất, khởi tạo lớp Chữ ký cung cấp như một đường dẫn tham số phương thức khởi tạo đến một tài liệu được cho là đã được xác minh.
        * Thứ hai, tạo một đối tượng VerifyOptions mới và thiết lập tất cả các thuộc tính cần thiết.
        * Cuối cùng, gọi phương thức Verify đối tượng của Signature thông qua cá thể VerifyOptions.
        * Sau đó xử lý kết quả xác minh.

    title_right: "yêu cầu hệ thống"
    content_right: |
        GroupDocs.Signature for Java được hỗ trợ trên tất cả các nền tảng và hệ điều hành chính. Trước khi thực hiện mã bên dưới, hãy đảm bảo rằng bạn đã cài đặt các điều kiện tiên quyết sau trên hệ thống của mình.

        * Hệ điều hành: Microsoft Windows, Linux, MacOS
        * Môi trường phát triển: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Tải xuống phiên bản mới nhất của GroupDocs.Signature for Java từ [Maven] (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ots file
        String filePath = "input.ots";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2020, 12, 12));
        options.setSignDateTimeTo(new Date(2022, 12, 12));
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ký bằng chữ ký Digital Demo trực tiếp"
    content: |
       Thêm nhiều chữ ký điện tử khác nhau vào tệp Ots ngay bây giờ bằng cách truy cập trang web [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Xác minh các chữ ký Digital khác bằng Java"
    content: |
        "Xác minh chữ ký điện tử được đặt trong các tài liệu khác nhau. Kiểm tra chất lượng chữ ký ở các định dạng tệp phổ biến như được tiết lộ bên dưới."
    format: 
       
       
back_to_top:
    enable: true
---