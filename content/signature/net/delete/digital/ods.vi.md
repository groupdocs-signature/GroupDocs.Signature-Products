---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Ods
productName: .NET
lang: vi
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ods for C#

############################# Head ############################
head_title: "Xóa chữ ký Digital khỏi tệp Ods qua C#"
head_description: "Việc xóa các chữ ký Digital cụ thể khỏi các tài liệu Ods đã ký có thể được thực hiện dễ dàng với mã .NET ngắn."

############################# Header ############################
title: "Xóa các chữ ký Digital được đặt trong các tệp Ods"
description: "Xóa các chữ ký Digital khác nhau khỏi tài liệu Ods. Việc xóa chữ ký Digital yêu cầu mã C# đơn giản."
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
    title: "Nhận thông tin về các tính năng của API GroupDocs.Signature for .NET"
    content: |
        API [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) cung cấp nhiều cách để xử lý tài liệu của bạn bằng chữ ký điện tử. Có sẵn chữ ký điện tử như văn bản, hình ảnh, chứng chỉ kỹ thuật số, mã vạch, mã QR, tem hoặc siêu dữ liệu. Khách hàng có thể thêm, xóa, cập nhật, xác minh hoặc tìm kiếm chữ ký điện tử ở các tệp PDF, tài liệu MS Word, sổ làm việc MS Excel, bản trình bày MS PowerPoint, tệp Adobe Photoshop và các định dạng hình ảnh khác nhau. Một số lượng lớn các tính năng và cài đặt hữu ích được cung cấp.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cách xóa chữ ký Digital khỏi tài liệu Ods của bạn"
    content_left: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) cung cấp tính năng hữu ích để xóa các tài liệu Ods có chữ ký Digital bằng một vài dòng mã.
        
        * Đầu tiên, khởi tạo đối tượng Chữ ký truyền đường dẫn đến tài liệu của bạn dưới dạng tham số phương thức khởi tạo.
        * Sau đó, tạo một đối tượng chữ ký thích hợp và thiết lập mã định danh duy nhất của nó.
        * Sau đó, gọi phương thức Delete truyền đối tượng chữ ký phải được xóa.
        * Cuối cùng là kết quả hoạt động xử lý.

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
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "a01e1940-997a-444b-89af-9309a2d559a5";

                // provide signature features to delete
                // set up particular signature id
                DigitalSignature signatureToDelete = new DigitalSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ký bằng chữ ký Digital Demo trực tiếp"
    content: |
       Thêm nhiều chữ ký điện tử khác nhau vào tệp Ods ngay bây giờ bằng cách truy cập trang web [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Xóa chữ ký Digital của bạn bằng C#"
    content: |
        "Xóa chữ ký điện tử đã được thêm vào các định dạng tài liệu khác nhau. Xóa chữ ký nhanh chóng mà không cần thêm mã."
    format: 
       
       
back_to_top:
    enable: true
---