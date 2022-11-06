---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Potx
productName: .NET
lang: ka
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Potx with C#

############################# Head ############################
head_title: "მოძებნეთ Metadata ხელმოწერები Potx ფაილში C#"
head_description: "გამოიყენეთ .NET Metadata ხელმოწერების მოსაძიებლად Potx ფაილებში კოდის რამდენიმე ხაზის გამოყენებით."

############################# Header ############################
title: "მოძებნეთ Metadata ხელმოწერები Potx ფაილში"
description: ".NET მშობლიური API საშუალებას გაძლევთ მოძებნოთ Metadata ხელმოწერები უკვე ხელმოწერილ Potx ფაილებში. განახორციელეთ ელექტრონული ხელმოწერის გაფართოებული ძიება თქვენს {{ფაილის ფორმატში}} დოკუმენტებში კოდის რამდენიმე ხაზის გამოყენებით."
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
    title: "GroupDocs.Signature for .NET API-ს შესახებ"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) უზრუნველყოფს .NET API-ს დოკუმენტების დასამუშავებლად ხელმოწერის სხვადასხვა ტიპების გამოყენებით, როგორიცაა ტექსტები, სურათები, ციფრული სერთიფიკატები, შტრიხკოდები, QR-კოდები, შტამპები ან მეტამონაცემები. მომხმარებლებს შეუძლიათ დაამატონ, წაშალონ, განაახლონ, გადაამოწმონ ან მოძებნონ ელექტრონული ხელმოწერები PDF ფაილებში, MS Word დოკუმენტებში, MS Excel სამუშაო წიგნებში, MS PowerPoint პრეზენტაციებში, Adobe Photoshop ფაილებში და გამოსახულების სხვადასხვა ფორმატში, საჭიროების შემთხვევაში ხელმოწერების თვისებების მორგების დამატებითი მხარდაჭერით.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "როგორ მოძებნოთ Metadata ხელმოწერები Potx-ში"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) აადვილებს .NET დეველოპერებს აპლიკაციებიდან ფაილებში Metadata ხელმოწერების ძიებას რამდენიმე მარტივი ნაბიჯის განხორციელებით.
        
        * შექმენით Signature კლასის ახალი ეგზემპლარი და გადაიტანეთ წყარო დოკუმენტის გზა კონსტრუქტორის პარამეტრად.
        * შექმენით SearchOptions ობიექტი თქვენი მოთხოვნების შესაბამისად და მიუთითეთ ძიების ვარიანტები.
        * გამოიძახეთ Signature კლასის ინსტანციის ძიების მეთოდი და გადასცეთ მას SearchOptions.
        * დაამუშავეთ ძიების შედეგები თქვენი მოთხოვნების შესაბამისად.

    title_right: "სისტემის მოთხოვნები"
    content_right: |
        GroupDocs.Signature for .NET მხარდაჭერილია ყველა ძირითად პლატფორმაზე და ოპერაციულ სისტემაზე. ქვემოთ მოცემული კოდის შესრულებამდე, დარწმუნდით, რომ თქვენს სისტემაში დაინსტალირებული გაქვთ შემდეგი წინაპირობები.

        * ოპერაციული სისტემები: Microsoft Windows, Linux, MacOS
        * განვითარების გარემო: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * ჩამოტვირთეთ GroupDocs.Signature for .NET-ის უახლესი ვერსია [Nuget]-დან (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Potx file
        string filePath = "input.potx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // search for Metadata signatures in Potx document
                List<PresentationMetadataSignature> signatures = signature.Search<PresentationMetadataSignature>(SignatureType.Metadata);

                // process signatures which were found 
                foreach (PresentationMetadataSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "მოძებნეთ Metadata ელექტრონული ხელმოწერების ცოცხალი დემო"
    content: |
       მოძებნეთ დოკუმენტი Potx ფაილების სხვადასხვა ელექტრონული ხელმოწერებისთვის ახლავე, ეწვიეთ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ვებსაიტს.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "მოძებნეთ სხვა Metadata ხელმოწერები C#-ის გამოყენებით"
    content: |
        "ელექტრონული ხელმოწერების ძიება სხვადასხვა დოკუმენტში. იპოვეთ ხელმოწერები ფაილის ერთ-ერთი პოპულარული ფორმატიდან, როგორც ეს ნაჩვენებია ქვემოთ."
    format: 
           
       
back_to_top:
    enable: true
---