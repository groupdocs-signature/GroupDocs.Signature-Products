---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Svg
productName: .NET
lang: vi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Svg for C#

############################# Head ############################
head_title: "Nối chữ ký điện tử Siêu dữ liệu vào tài liệu Svg qua C#"
head_description: "Sử dụng Siêu dữ liệu làm chữ ký điện tử ẩn bên trong tài liệu Svg của bạn bằng cách sử dụng một vài dòng mã C#. Sử dụng API chữ ký tài liệu GroupDocs để ký điện tử các tài liệu và tệp kinh doanh của bạn bằng thông tin Siêu dữ liệu."

############################# Header ############################
title: "Chữ ký điện tử siêu dữ liệu cho tài liệu Svg qua .NET rất đơn giản và dễ sử dụng!"
description: "eSign các tài liệu và hợp đồng Svg của bạn bằng các mục nhập Siêu dữ liệu ẩn. Tạo Siêu dữ liệu cho các tệp PDF, tài liệu MS Word, sổ làm việc MS Excel, bản trình bày MS PowerPoint và các định dạng hình ảnh khác nhau mà không gặp sự cố và phải viết mã bổ sung."
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
    title: "Giới thiệu về GroupDocs.Signature for .NET API chữ ký siêu dữ liệu"
    content: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) là một API phổ biến cho ký điện tử tài liệu kỹ thuật số. Các chữ ký như văn bản, hình ảnh, chứng chỉ kỹ thuật số, mã vạch, mã QR, tem hoặc siêu dữ liệu đều có sẵn. Chữ ký có thể được đặt trên các tệp PDF, tài liệu MS Word, sổ làm việc MS Excel, bản trình bày MS PowerPoint, tệp Adobe Photoshop và các định dạng hình ảnh khác nhau. Khách hàng có thể ký vào tài liệu của họ và cập nhật, tìm kiếm, xác minh, xóa hoặc xem trước các chữ ký điện tử đã được đưa vào các tài liệu đó. Hơn nữa, rất nhiều khả năng tùy chỉnh chữ ký được cung cấp.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Các bước để đăng nhập Svg bằng Metadata trong C#"
    content_left: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) cung cấp khả năng ký các tài liệu Svg bằng chữ ký Metadata một cách nhanh chóng và dễ dàng.
        
        * Tạo một phiên bản của lớp Chữ ký cung cấp tệp Svg phải ký dưới dạng đường dẫn hoặc luồng bộ nhớ
        * Khởi tạo lớp SignOptions và thiết lập tất cả dữ liệu được yêu cầu.
        * Gọi phương thức Signature.Sign () chuyển đầu ra tệp Svg hoặc luồng bộ nhớ

    title_right: " yêu cầu hệ thống"
    content_right: |
        GroupDocs.Signature for .NET được hỗ trợ trên tất cả các nền tảng và hệ điều hành chính. Trước khi thực hiện mã bên dưới, hãy đảm bảo rằng bạn đã cài đặt các điều kiện tiên quyết sau trên hệ thống của mình.

        * Hệ điều hành: Microsoft Windows, Linux, MacOS
        * Môi trường phát triển: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Nhận GroupDocs.Signature for .NET mới nhất từ ​​[Nuget] (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Svg file
        string filePath = "input.svg";
        // Set up output file
        string outputFilePath = "output.svg";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                MetadataSignOptions options = new MetadataSignOptions();

                // Specify different Metadata Signatures and add them to options signature collection
                // set start id
                ushort imgsMetadataId = 41996;
                // setup int value
                ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
                options.Signatures.Add(mdSign_DocId);
                // setup Author property
                ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
                options.Signatures.Add(mdSign_Author);
                // setup data of sign date
                ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, DateTime.Now); // DateTime
                options.Signatures.Add(mdSign_Date);
                // setup double
                ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456M); //decimal value
                options.Signatures.Add(mdSign_Amnt);

                // sign Svg document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ký tài liệu Svg bằng Metadata Live Demo"
    content: |
       Ký tệp Svg bằng nhiều chữ ký ngay bây giờ bằng cách truy cập trang web [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). Bản demo trực tuyến miễn phí đang chờ bạn.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Các chữ ký Metadata được hỗ trợ khác cho C#"
    content: |
        "Bạn cũng có thể ký Svg bằng các loại chữ ký khác. Vui lòng xem danh sách bên dưới."
    format: 
       
       
back_to_top:
    enable: true
---