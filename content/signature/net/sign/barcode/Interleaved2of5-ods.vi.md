---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Ods
productName: .NET
lang: vi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Ods for C#

############################# Head ############################
head_title: "eSign Ods tài liệu với Interleaved2of5 Mã vạch trong C#"
head_description: "Tạo Chữ ký Mã vạch Interleaved2of5 và đưa nó vào tài liệu Ods với .NET bằng cách sử dụng một vài dòng mã. Sử dụng API Chữ ký Tài liệu GroupDocs để ký các định dạng tệp khác nhau."

############################# Header ############################
title: "Tạo Interleaved2of5 Chữ ký mã vạch cho tài liệu Ods trong C#"
description: "eSign các tài liệu kinh doanh Ods của bạn bằng Mã vạch Interleaved2of5. Tạo chữ ký mã vạch nhanh chóng và dễ dàng với một vài dòng mã để thiết lập các tùy chọn ký."
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
    title: "Giới thiệu về GroupDocs.Signature for .NET API chữ ký mã vạch."
    content: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) là một API nhanh chóng và dễ dàng để quản lý các tài liệu kỹ thuật số ký điện tử bằng cách sử dụng các loại Mã vạch như UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 và nhiều người khác. Khách hàng có thể dễ dàng tạo Mã vạch cung cấp văn bản cần thiết và đưa chúng vào PDF, Tài liệu Microsoft Office Words, sổ làm việc Microsoft Office Excel, bản trình bày MS PowerPoint, tệp Adobe Photoshop và các định dạng hình ảnh khác nhau. Mã vạch được đặt trong tài liệu có thể được cập nhật, tìm kiếm, xác minh, xóa hoặc xem trước. Hơn nữa, tùy chỉnh mã vạch được hỗ trợ.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Các bước để đăng nhập Ods bằng Barcode trong C#"
    content_left: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) cung cấp khả năng ký các tài liệu Ods bằng chữ ký Barcode một cách nhanh chóng và dễ dàng.
        
        * Tạo một phiên bản của lớp Chữ ký cung cấp tệp Ods phải ký dưới dạng đường dẫn hoặc luồng bộ nhớ
        * Khởi tạo lớp SignOptions và thiết lập tất cả dữ liệu được yêu cầu.
        * Gọi phương thức Signature.Sign () chuyển đầu ra tệp Ods hoặc luồng bộ nhớ

    title_right: " yêu cầu hệ thống"
    content_right: |
        GroupDocs.Signature for .NET được hỗ trợ trên tất cả các nền tảng và hệ điều hành chính. Trước khi thực hiện mã bên dưới, hãy đảm bảo rằng bạn đã cài đặt các điều kiện tiên quyết sau trên hệ thống của mình.

        * Hệ điều hành: Microsoft Windows, Linux, MacOS
        * Môi trường phát triển: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Nhận GroupDocs.Signature for .NET mới nhất từ ​​[Nuget] (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Ods file
        string filePath = "input.ods";
        // Set up output file
        string outputFilePath = "output.ods";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Interleaved2of5,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Ods document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ký tài liệu Ods bằng Barcode Live Demo"
    content: |
       Ký tệp Ods bằng nhiều chữ ký ngay bây giờ bằng cách truy cập trang web [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). Bản demo trực tuyến miễn phí đang chờ bạn.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Xen kẽ 2 trong 5 (ITF) là một chữ số mã hóa mã vạch mã vạch hai chiều rộng liên tục. Nó được sử dụng cho mục đích thương mại trên phim 135, cho mã vạch ITF-14, và trên thùng giấy của một số sản phẩm, trong khi các sản phẩm bên trong được dán nhãn UPC hoặc EAN.
          characterset: |
             Chữ số (0-9).
          textcapacity: |
             Chiều dài thay đổi.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Các chữ ký Barcode được hỗ trợ khác cho C#"
    content: |
        "Bạn cũng có thể ký Ods bằng các loại chữ ký khác. Vui lòng xem danh sách bên dưới."
    format: 
        
       
back_to_top:
    enable: true
---