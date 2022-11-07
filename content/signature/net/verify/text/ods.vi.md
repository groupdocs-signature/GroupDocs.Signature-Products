---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Text
fileformat: Ods
productName: .NET
lang: vi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Ods for C#

############################# Head ############################
head_title: "Xác minh chữ ký Text cho tệp Ods qua C#"
head_description: "Chỉ sử dụng một vài dòng mã .NET để xác minh tài liệu Ods và chữ ký Text của chúng."

############################# Header ############################
title: "Xác minh chữ ký Text cho các tệp Ods"
description: "API cho .NET cung cấp cơ hội xác minh chữ ký Text tại tài liệu Ods. Việc xác minh chữ ký điện tử bên trong tài liệu Ods của bạn có thể được thực hiện nhanh chóng và dễ dàng."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Khám phá các tính năng mới của API GroupDocs.Signature for .NET"
    content: |
        API [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) cung cấp nhiều cách để xử lý nhiều định dạng tài liệu bằng cách sử dụng chữ ký điện tử. Nhiều loại chữ ký điện tử như văn bản, hình ảnh, chứng chỉ kỹ thuật số, mã vạch, mã QR, tem hoặc siêu dữ liệu được hỗ trợ. Khách hàng có thể thêm, bớt, chỉnh sửa, xác thực hoặc tìm kiếm chữ ký điện tử tại các tệp PDF, tài liệu MS Word, sổ làm việc MS Excel, bản trình bày MS PowerPoint, tệp Adobe Photoshop và các định dạng hình ảnh khác nhau. Có sẵn một số tính năng và cài đặt bổ sung đáng kinh ngạc.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cách xác thực chữ ký Text trong tài liệu Ods của bạn"
    content_left: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) bao gồm các tính năng hữu ích như xác minh chữ ký Text được đặt trong tài liệu Ods. Sử dụng cơ hội này mà không cần triển khai thêm mã.
        
        * Thứ nhất, khởi tạo lớp Chữ ký cung cấp như một đường dẫn tham số phương thức khởi tạo đến một tài liệu được cho là đã được xác minh.
        * Thứ hai, tạo một đối tượng VerifyOptions mới và thiết lập tất cả các thuộc tính cần thiết.
        * Cuối cùng, gọi phương thức Verify đối tượng của Signature thông qua cá thể VerifyOptions.
        * Sau đó xử lý kết quả xác minh.

    title_right: "yêu cầu hệ thống"
    content_right: |
        GroupDocs.Signature for .NET được hỗ trợ trên tất cả các nền tảng và hệ điều hành chính. Trước khi thực hiện mã bên dưới, hãy đảm bảo rằng bạn đã cài đặt các điều kiện tiên quyết sau trên hệ thống của mình.

        * Hệ điều hành: Microsoft Windows, Linux, MacOS
        * Môi trường phát triển: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Tải xuống phiên bản mới nhất của GroupDocs.Signature for .NET từ [Nuget] (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ods file
        string filePath = "input.ods";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                TextVerifyOptions options = new TextVerifyOptions()
                {
                    // Process all pages 
                    AllPages = true,
                    // set up text match type
                    MatchType = TextMatchType.Exact,
                    // specify text pattern to search
                    Text = "Very important signature",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ký bằng chữ ký Text Demo trực tiếp"
    content: |
       Thêm nhiều chữ ký điện tử khác nhau vào tệp Ods ngay bây giờ bằng cách truy cập trang web [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Xác minh các chữ ký Text khác bằng C#"
    content: |
        "Xác minh chữ ký điện tử được đặt trong các tài liệu khác nhau. Kiểm tra chất lượng chữ ký ở các định dạng tệp phổ biến như được tiết lộ bên dưới."
    format: 
       
       
back_to_top:
    enable: true
---