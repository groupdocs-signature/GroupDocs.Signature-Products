---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Docx
productName: .NET
lang: ka
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Docx for C#

############################# Head ############################
head_title: "eSign Docx დოკუმენტი Pharmacode შტრიხკოდით C#-ში"
head_description: "შექმენით Pharmacode შტრიხკოდის ხელმოწერა და განათავსეთ იგი Docx დოკუმენტზე .NET კოდის რამდენიმე ხაზის გამოყენებით. გამოიყენეთ GroupDocs Document Signature API სხვადასხვა ფაილის ფორმატების ხელმოწერისთვის."

############################# Header ############################
title: "შექმენით Pharmacode შტრიხკოდის ხელმოწერა Docx დოკუმენტისთვის C#-ში"
description: "მოაწერეთ თქვენი {{ფაილის ფორმატი}} ბიზნეს დოკუმენტები Pharmacode შტრიხკოდით. შექმენით შტრიხკოდის ხელმოწერა სწრაფად და მარტივად რამდენიმე ხაზის კოდით ხელმოწერის ვარიანტების დასაყენებლად."
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
    title: "GroupDocs.Signature for .NET შტრიხკოდის ხელმოწერების API-ს შესახებ."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) არის სწრაფი და მარტივი API ციფრული დოკუმენტების ელექტრონული ხელმოწერის სამართავად შტრიხკოდების ტიპების გამოყენებით, როგორიცაა UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN. , ITF14 და მრავალი სხვა. მომხმარებლებს შეუძლიათ მარტივად შექმნან შტრიხკოდები, რომლებიც უზრუნველყოფენ საჭირო ტექსტს და განათავსონ ისინი PDF, Microsoft Office Words დოკუმენტები, Microsoft Office Excel სამუშაო წიგნები, MS PowerPoint პრეზენტაციები, Adobe Photoshop ფაილები და გამოსახულების სხვადასხვა ფორმატში. დოკუმენტებში განთავსებული შტრიხკოდების განახლება, ძებნა, შემოწმება, წაშლა ან წინასწარი ნახვა შესაძლებელია. უფრო მეტიც, შტრიხკოდების პერსონალიზაცია მხარდაჭერილია.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Docx-ით ხელმოწერის ნაბიჯები Barcode-ით C#-ში"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) იძლევა შესაძლებლობას მოაწეროთ Docx დოკუმენტები Barcode ხელმოწერებით სწრაფად და მარტივად.
        
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
        
        // Set up input Docx file
        string filePath = "input.docx";
        // Set up output file
        string outputFilePath = "output.docx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Pharmacode,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Docx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "დოკუმენტების {{ფაილის ფორმატი}} ხელმოწერა Barcode Live Demo-ით"
    content: |
       მოაწერეთ {{ფაილის ფორმატი}} ფაილი სხვადასხვა ხელმოწერებით ახლავე, ეწვიეთ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ვებსაიტს. უფასო ონლაინ დემო გელოდებათ.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            ფარმაკოდი, რომელიც ასევე ცნობილია როგორც ფარმაცევტული ორობითი კოდი, არის შტრიხკოდების სტანდარტი, რომელიც გამოიყენება ფარმაცევტულ ინდუსტრიაში, როგორც შეფუთვის კონტროლის სისტემა.
          characterset: |
             რიცხვითი ციფრები (0-9).
          textcapacity: |
             წარმოადგენს მხოლოდ ერთ მთელ რიცხვს 3-დან 131070-მდე.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "სხვა მხარდაჭერილი Barcode ხელმოწერები C#-ისთვის"
    content: |
        "თქვენ ასევე შეგიძლიათ მოაწეროთ {{ფაილის ფორმატი}} ხელმოწერის სხვა ტიპებით. გთხოვთ იხილოთ სია ქვემოთ."
    format: 
        
       
back_to_top:
    enable: true
---