---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Ppsx
productName: .NET
lang: ka
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Ppsx for C#

############################# Head ############################
head_title: "მეტამონაცემების ელექტრონული ხელმოწერების დამატება Ppsx დოკუმენტებზე C#-ის მეშვეობით"
head_description: "გამოიყენეთ მეტამონაცემები, როგორც ფარული ელექტრონული ხელმოწერები თქვენს {{ფაილის ფორმატში}} დოკუმენტებში C# კოდის რამდენიმე სტრიქონის გამოყენებით. გამოიყენეთ GroupDocs Document Signature API თქვენი ბიზნეს დოკუმენტებისა და ფაილების ელექტრონული ხელმოწერისთვის მეტამონაცემების ინფორმაციით."

############################# Header ############################
title: "მეტამონაცემების ელექტრონული ხელმოწერები Ppsx დოკუმენტისთვის .NET-ის მეშვეობით მარტივი და მარტივი გამოსაყენებელია!"
description: "მოაწერეთ თქვენი {{ფაილის ფორმატი}} დოკუმენტები და კონტრაქტები ფარული მეტამონაცემების ჩანაწერებით. შექმენით მეტამონაცემები PDF-ებისთვის, MS Word დოკუმენტებისთვის, MS Excel სამუშაო წიგნებისთვის, MS PowerPoint პრეზენტაციებისთვის და სხვადასხვა გამოსახულების ფორმატებისთვის უპრობლემოდ და დამატებითი კოდირების გარეშე."
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
    title: "GroupDocs.Signature for .NET მეტამონაცემების ხელმოწერების API-ს შესახებ"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) არის პოპულარული API ციფრული დოკუმენტების ელექტრონული ხელმოწერისთვის. ხელმოწერები, როგორიცაა ტექსტები, სურათები, ციფრული სერთიფიკატები, შტრიხკოდები, QR-კოდები, შტამპები ან მეტამონაცემები ხელმისაწვდომია. ხელმოწერები შეიძლება განთავსდეს PDF-ებზე, MS Word დოკუმენტებზე, MS Excel სამუშაო წიგნებზე, MS PowerPoint პრეზენტაციებზე, Adobe Photoshop ფაილებსა და გამოსახულების სხვადასხვა ფორმატებზე. კლიენტებს შეუძლიათ ხელი მოაწერონ თავიანთ დოკუმენტს და განაახლონ, მოძებნონ, გადაამოწმონ, წაშალონ ან გადახედონ ამ დოკუმენტებზე განთავსებული ელექტრონული ხელმოწერების. უფრო მეტიც, გათვალისწინებულია ხელმოწერების პერსონალიზაციის უამრავი შესაძლებლობა.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Ppsx-ით ხელმოწერის ნაბიჯები Metadata-ით C#-ში"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) იძლევა შესაძლებლობას მოაწეროთ Ppsx დოკუმენტები Metadata ხელმოწერებით სწრაფად და მარტივად.
        
        * შექმენით ხელმოწერის კლასის მაგალითი, რომელიც უზრუნველყოფს {{ფაილის ფორმატი}} ფაილს, რომელიც უნდა მოაწეროს ხელი, როგორც გზა ან მეხსიერების ნაკადი
        * Instantate SignOptions კლასი და დააყენეთ ყველა მოთხოვნილი მონაცემი.
        * გამოიძახეთ Signature.Sign() მეთოდი, რომელიც გადასცემს გამომავალ {{ფაილის ფორმატი}} ფაილს ან მეხსიერების ნაკადს

    title_right: " სისტემის მოთხოვნები"
    content_right: |
        GroupDocs.Signature for .NET მხარდაჭერილია ყველა ძირითად პლატფორმაზე და ოპერაციულ სისტემაზე. ქვემოთ მოცემული კოდის შესრულებამდე, დარწმუნდით, რომ თქვენს სისტემაში დაინსტალირებული გაქვთ შემდეგი წინაპირობები.

        * ოპერაციული სისტემები: Microsoft Windows, Linux, MacOS
        * განვითარების გარემო: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * მიიღეთ უახლესი GroupDocs.Signature for .NET [Nuget]-ისგან (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Ppsx file
        string filePath = "input.ppsx";
        // Set up output file
        string outputFilePath = "output.ppsx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Ppsx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "დოკუმენტების {{ფაილის ფორმატი}} ხელმოწერა Metadata Live Demo-ით"
    content: |
       მოაწერეთ {{ფაილის ფორმატი}} ფაილი სხვადასხვა ხელმოწერებით ახლავე, ეწვიეთ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ვებსაიტს. უფასო ონლაინ დემო გელოდებათ.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "სხვა მხარდაჭერილი Metadata ხელმოწერები C#-ისთვის"
    content: |
        "თქვენ ასევე შეგიძლიათ მოაწეროთ {{ფაილის ფორმატი}} ხელმოწერის სხვა ტიპებით. გთხოვთ იხილოთ სია ქვემოთ."
    format: 
       
       
back_to_top:
    enable: true
---