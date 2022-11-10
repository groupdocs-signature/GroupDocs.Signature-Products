---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Csv
productName: .NET
lang: vi
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Csv with C#

############################# Head ############################
head_title: "Tìm kiếm chữ ký Image trong tệp Csv trong C#"
head_description: "Sử dụng .NET để tìm kiếm chữ ký Image trong tệp Csv bằng một vài dòng mã."

############################# Header ############################
title: "Tìm kiếm chữ ký Image trong tệp Csv"
description: "API gốc .NET cho phép tìm kiếm chữ ký Image trong các tệp Csv đã được ký. Thực hiện tìm kiếm chữ ký điện tử nâng cao trong tài liệu Csv của bạn bằng cách sử dụng một vài dòng mã."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Giới thiệu về API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) cung cấp API .NET để xử lý tài liệu bằng nhiều loại chữ ký khác nhau như văn bản, hình ảnh, chứng chỉ kỹ thuật số, mã vạch, mã QR, tem hoặc siêu dữ liệu. Người dùng có thể thêm, xóa, cập nhật, xác minh hoặc tìm kiếm chữ ký điện tử trong tệp PDF, tài liệu MS Word, sổ làm việc MS Excel, bản trình bày MS PowerPoint, tệp Adobe Photoshop và các định dạng hình ảnh khác nhau, với hỗ trợ bổ sung để tùy chỉnh các thuộc tính chữ ký khi cần thiết.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cách tìm kiếm chữ ký Image trong Csv"
    content_left: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) giúp các nhà phát triển .NET tìm kiếm chữ ký Image trong tệp Csv từ ứng dụng của họ dễ dàng hơn bằng cách thực hiện một vài bước đơn giản.
        
        * Tạo một phiên bản mới của lớp Chữ ký và chuyển đường dẫn tài liệu nguồn làm tham số khởi tạo.
        * Khởi tạo đối tượng SearchOptions theo yêu cầu của bạn và chỉ định các tùy chọn tìm kiếm.
        * Gọi phương thức Tìm kiếm của cá thể lớp Chữ ký và chuyển SearchOptions cho nó.
        * Xử lý kết quả tìm kiếm phù hợp với nhu cầu của bạn.

    title_right: "yêu cầu hệ thống"
    content_right: |
        GroupDocs.Signature for .NET được hỗ trợ trên tất cả các nền tảng và hệ điều hành chính. Trước khi thực hiện mã bên dưới, hãy đảm bảo rằng bạn đã cài đặt các điều kiện tiên quyết sau trên hệ thống của mình.

        * Hệ điều hành: Microsoft Windows, Linux, MacOS
        * Môi trường phát triển: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Tải xuống phiên bản mới nhất của GroupDocs.Signature for .NET từ [Nuget] (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Csv file
        string filePath = "input.csv";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                ImageSearchOptions options = new ImageSearchOptions()
                {
                    // set minimum size if needed
                    MinContentSize = 100,
                    // set maximum image size if needed
                    MaxContentSize = 2000,                    
                    // return  Image images for processing
                    ReturnContent = true,
                    // set up type of returned  Image images
                    ReturnContentType = FileType.PNG                                 
                };

                // search for Image signatures in Csv document
                List<ImageSignature> signatures = signature.Search<ImageSignature>(options);

                // process signatures which were found                
                foreach (ImageSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Tìm kiếm chữ ký điện tử Image Demo trực tiếp"
    content: |
       Tìm kiếm tài liệu để tìm các chữ ký điện tử khác nhau cho các tệp Csv ngay bây giờ bằng cách truy cập trang web [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Tìm kiếm các chữ ký Image khác bằng C#"
    content: |
        "Tìm kiếm chữ ký điện tử trong các tài liệu khác nhau. Tìm chữ ký từ một trong những định dạng tệp phổ biến như được hiển thị bên dưới."
    format: 
           
       
back_to_top:
    enable: true
---