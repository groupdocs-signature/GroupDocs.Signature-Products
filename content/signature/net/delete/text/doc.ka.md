---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Doc
productName: .NET
lang: ka
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Doc for C#

############################# Head ############################
head_title: "წაშალეთ Text ხელმოწერა Doc ფაილებიდან C#-ით"
head_description: "კონკრეტული Text ხელმოწერების წაშლა ხელმოწერილი Doc დოკუმენტებიდან შეიძლება მარტივად განხორციელდეს მოკლე .NET კოდით."

############################# Header ############################
title: "წაშალეთ Text ხელმოწერები, რომლებიც განთავსებულია Doc ფაილში"
description: "წაშალეთ სხვადასხვა Text ხელმოწერა Doc დოკუმენტებიდან. Text ხელმოწერის ამოღებას სჭირდება მარტივი C# კოდი."
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
    title: "მიიღეთ ინფორმაცია GroupDocs.Signature for .NET API ფუნქციების შესახებ"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API გთავაზობთ მრავალ გზას თქვენი დოკუმენტების ელექტრონული ხელმოწერების გამოყენებით დასამუშავებლად. ხელმისაწვდომია ციფრული ხელმოწერები, როგორიცაა ტექსტები, სურათები, ციფრული სერთიფიკატები, შტრიხკოდები, QR-კოდები, შტამპები ან მეტამონაცემები. მომხმარებელს აქვს შესაძლებლობა დაამატონ, წაშალონ, განაახლონ, გადაამოწმონ ან მოძებნონ ციფრული ხელმოწერები PDF-ებში, MS Word დოკუმენტებში, MS Excel სამუშაო წიგნებში, MS PowerPoint პრეზენტაციებში, Adobe Photoshop ფაილებსა და გამოსახულების სხვადასხვა ფორმატებში. მოწოდებულია სასარგებლო ფუნქციების და პარამეტრების დიდი რაოდენობა.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "როგორ ამოიღოთ Text ხელმოწერა თქვენი Doc დოკუმენტიდან"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) გთავაზობთ სასარგებლო ფუნქციას Doc დოკუმენტების Text ხელმოწერების გასასუფთავებლად რამდენიმე სტრიქონის კოდით.
        
        * უპირველეს ყოვლისა, შექმენით ხელმოწერის ობიექტი, რომელიც გადადის თქვენს დოკუმენტში, როგორც კონსტრუქტორის პარამეტრი.
        * შემდეგ შექმენით შესაბამისი ხელმოწერის ობიექტი და დააყენეთ მისი უნიკალური იდენტიფიკატორი.
        * ამის შემდეგ, გამოიძახეთ Delete მეთოდი, რომელიც გადასცემს ხელმოწერის ობიექტს, რომელიც უნდა წაიშალოს.
        * საბოლოოდ, დაამუშავეთ ოპერაციის შედეგები.

    title_right: "სისტემის მოთხოვნები"
    content_right: |
        GroupDocs.Signature for .NET მხარდაჭერილია ყველა ძირითად პლატფორმაზე და ოპერაციულ სისტემაზე. ქვემოთ მოცემული კოდის შესრულებამდე, დარწმუნდით, რომ თქვენს სისტემაში დაინსტალირებული გაქვთ შემდეგი წინაპირობები.

        * ოპერაციული სისტემები: Microsoft Windows, Linux, MacOS
        * განვითარების გარემო: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * ჩამოტვირთეთ GroupDocs.Signature for .NET-ის უახლესი ვერსია [Nuget]-დან (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to delete
                // set up particular signature id
                TextSignature signatureToDelete = new TextSignature(id);

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
    title: "ხელმოწერა Text ხელმოწერებით Live Demo"
    content: |
       დაამატეთ სხვადასხვა ელექტრონული ხელმოწერები Doc ფაილს ახლავე, ეწვიეთ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ვებსაიტს.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "წაშალეთ თქვენი Text ხელმოწერები C#-ით"
    content: |
        "ელექტრონული ხელმოწერების წაშლა, რომლებიც დაემატა სხვადასხვა დოკუმენტის ფორმატებს. სწრაფად ამოიღეთ ხელმოწერები დამატებითი კოდის გარეშე."
    format: 
       
       
back_to_top:
    enable: true
---