---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Pptm
productName: .NET
lang: ka
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pptm for C#

############################# Head ############################
head_title: "Digital ხელმოწერების დადასტურება Pptm ფაილებისთვის C#-ით"
head_description: "გამოიყენეთ .NET კოდის მხოლოდ რამდენიმე ხაზი Pptm დოკუმენტებისა და მათი Digital ხელმოწერების დასადასტურებლად."

############################# Header ############################
title: "Digital ხელმოწერების დადასტურება Pptm ფაილებისთვის"
description: "API .NET-ისთვის იძლევა შესაძლებლობას გადაამოწმოთ Digital ხელმოწერები Pptm დოკუმენტებში. თქვენი {{ფაილის ფორმატი}} დოკუმენტებში ელექტრონული ხელმოწერების დადასტურება შეიძლება სწრაფად და მარტივად განხორციელდეს."
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
    title: "აღმოაჩინეთ ახალი GroupDocs.Signature for .NET API ფუნქციები"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API გთავაზობთ მრავალი დოკუმენტის ფორმატის დამუშავების გზებს ელექტრონული ხელმოწერების გამოყენებით. მხარდაჭერილია მრავალი სახის ციფრული ხელმოწერა, როგორიცაა ტექსტები, სურათები, ციფრული სერთიფიკატები, შტრიხკოდები, QR-კოდები, შტამპები ან მეტამონაცემები. კლიენტებს შეუძლიათ დაამატონ, წაშალონ, შეცვალონ, დაადასტურონ ან მოძებნონ ციფრული ხელმოწერები PDF ფაილებში, MS Word დოკუმენტებში, MS Excel სამუშაო წიგნებში, MS PowerPoint პრეზენტაციებში, Adobe Photoshop ფაილებსა და გამოსახულების სხვადასხვა ფორმატებში. გასაოცარი რაოდენობის დამატებითი ფუნქციები და პარამეტრები ხელმისაწვდომია.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "როგორ გადავამოწმოთ Digital ხელმოწერები თქვენს Pptm დოკუმენტში"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) შეიცავს სასარგებლო ფუნქციებს, როგორიცაა Digital ხელმოწერების დადასტურება, რომლებიც განთავსებულია Pptm დოკუმენტებზე. გამოიყენეთ ეს შესაძლებლობა დამატებითი კოდის განხორციელების გარეშე.
        
        * უპირველეს ყოვლისა, შექმენით Signature კლასი, რომელიც უზრუნველყოფს როგორც კონსტრუქტორის პარამეტრის გზას დოკუმენტში, რომელიც უნდა იყოს გადამოწმებული.
        * მეორეც, შექმენით ახალი VerifyOptions ობიექტი და დააყენეთ ყველა საჭირო თვისება.
        * და ბოლოს, გამოიძახეთ Signature-ის ობიექტი Verify მეთოდი VerifyOptions ინსტანციის გავლით.
        * შემდეგ დაამუშავეთ გადამოწმების შედეგები.

    title_right: "სისტემის მოთხოვნები"
    content_right: |
        GroupDocs.Signature for .NET მხარდაჭერილია ყველა ძირითად პლატფორმაზე და ოპერაციულ სისტემაზე. ქვემოთ მოცემული კოდის შესრულებამდე, დარწმუნდით, რომ თქვენს სისტემაში დაინსტალირებული გაქვთ შემდეგი წინაპირობები.

        * ოპერაციული სისტემები: Microsoft Windows, Linux, MacOS
        * განვითარების გარემო: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * ჩამოტვირთეთ GroupDocs.Signature for .NET-ის უახლესი ვერსია [Nuget]-დან (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pptm file
        string filePath = "input.pptm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                DigitalVerifyOptions options = new DigitalVerifyOptions()
                {
                    // Digital signature comment
                    Comments = "Approved by co-owner",
                    // specify period of signatures
                    SignDateTimeFrom = new DateTime(year: 2021, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2022, month: 12, day: 31)
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
    title: "ხელმოწერა Digital ხელმოწერებით Live Demo"
    content: |
       დაამატეთ სხვადასხვა ელექტრონული ხელმოწერები Pptm ფაილს ახლავე, ეწვიეთ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ვებსაიტს.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "დაადასტურეთ სხვა Digital ხელმოწერები C#-ის გამოყენებით"
    content: |
        "სხვადასხვა დოკუმენტებში განთავსებული ელექტრონული ხელმოწერების შემოწმება. შეამოწმეთ ხელმოწერების ხარისხი პოპულარული ფაილის ფორმატებში, როგორც ეს ნაჩვენებია ქვემოთ."
    format: 
       
       
back_to_top:
    enable: true
---