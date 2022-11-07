---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Xltx
productName: .NET
lang: vi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Xltx for C#

############################# Head ############################
head_title: "Thêm chữ ký Image vào tệp Xltx bằng C#"
head_description: "Đặt Image Chữ ký trên tệp Xltx cho .NET bằng cách sử dụng một vài dòng mã. Sử dụng API chữ ký tài liệu GroupDocs để ký hàng chục định dạng tệp."

############################# Header ############################
title: "Ký các tệp Xltx bằng chữ ký Image trong C#"
description: "Cách thêm Chữ ký Image bằng một vài dòng mã .NET"
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
    title: "Giới thiệu về GroupDocs.Signature for .NET API chữ ký hình ảnh"
    content: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) là một API phổ biến cho ký điện tử tài liệu kỹ thuật số. Các chữ ký như văn bản, hình ảnh, chứng chỉ kỹ thuật số, mã vạch, mã QR, tem hoặc siêu dữ liệu đều có sẵn. Chữ ký có thể được đặt trên các tệp PDF, tài liệu MS Word, sổ làm việc MS Excel, bản trình bày MS PowerPoint, tệp Adobe Photoshop và các định dạng hình ảnh khác nhau. Khách hàng có thể ký vào tài liệu của họ và cập nhật, tìm kiếm, xác minh, xóa hoặc xem trước các chữ ký điện tử đã được đưa vào các tài liệu đó. Hơn nữa, rất nhiều khả năng tùy chỉnh chữ ký được cung cấp.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Các bước để đăng nhập Xltx bằng Image trong C#"
    content_left: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) cung cấp khả năng ký các tài liệu Xltx bằng chữ ký Image một cách nhanh chóng và dễ dàng.
        
        * Tạo một phiên bản của lớp Chữ ký cung cấp tệp Xltx phải ký dưới dạng đường dẫn hoặc luồng bộ nhớ
        * Khởi tạo lớp SignOptions và thiết lập tất cả dữ liệu được yêu cầu.
        * Gọi phương thức Signature.Sign () chuyển đầu ra tệp Xltx hoặc luồng bộ nhớ

    title_right: " yêu cầu hệ thống"
    content_right: |
        GroupDocs.Signature for .NET được hỗ trợ trên tất cả các nền tảng và hệ điều hành chính. Trước khi thực hiện mã bên dưới, hãy đảm bảo rằng bạn đã cài đặt các điều kiện tiên quyết sau trên hệ thống của mình.

        * Hệ điều hành: Microsoft Windows, Linux, MacOS
        * Môi trường phát triển: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Nhận GroupDocs.Signature for .NET mới nhất từ ​​[Nuget] (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xltx file
        string filePath = "input.xltx";
        // Set up output file
        string outputFilePath = "output.xltx";
        // Provide image file
        string imageFilePath = "image.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
            //Provide sign options
            ImageSignOptions options = new ImageSignOptions(imageFilePath)
            {
                // set signature position
                Left = 50,
                Top = 200
            };

            // sign Xltx document
            SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ký tài liệu Xltx bằng Image Live Demo"
    content: |
       Ký tệp Xltx bằng nhiều chữ ký ngay bây giờ bằng cách truy cập trang web [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). Bản demo trực tuyến miễn phí đang chờ bạn.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Các chữ ký Image được hỗ trợ khác cho C#"
    content: |
        "Bạn cũng có thể ký Xltx bằng các loại chữ ký khác. Vui lòng xem danh sách bên dưới."
    format: 
       
       
back_to_top:
    enable: true
---