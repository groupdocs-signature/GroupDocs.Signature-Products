---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Text
fileformat: Dotm
productName: .NET
lang: ka
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Text signatures at Dotm with C#

############################# Head ############################
head_title: "მოძებნეთ Text ხელმოწერები Dotm ფაილში C#"
head_description: "გამოიყენეთ .NET Text ხელმოწერების მოსაძიებლად Dotm ფაილებში კოდის რამდენიმე ხაზის გამოყენებით."

############################# Header ############################
title: "მოძებნეთ Text ხელმოწერები Dotm ფაილში"
description: ".NET მშობლიური API საშუალებას გაძლევთ მოძებნოთ Text ხელმოწერები უკვე ხელმოწერილ Dotm ფაილებში. განახორციელეთ ელექტრონული ხელმოწერის გაფართოებული ძიება თქვენს {{ფაილის ფორმატში}} დოკუმენტებში კოდის რამდენიმე ხაზის გამოყენებით."
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
    title_left: "როგორ მოძებნოთ Text ხელმოწერები Dotm-ში"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) აადვილებს .NET დეველოპერებს აპლიკაციებიდან ფაილებში Text ხელმოწერების ძიებას რამდენიმე მარტივი ნაბიჯის განხორციელებით.
        
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
                
        // Set up input Dotm file
        string filePath = "input.dotm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                TextSearchOptions options = new TextSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // specify text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature"
                };

                // search for Text signatures in Dotm document
                List<TextSignature> signatures = signature.Search<TextSignature>(options);

                // process signatures which were found                
                foreach (TextSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "მოძებნეთ Text ელექტრონული ხელმოწერების ცოცხალი დემო"
    content: |
       მოძებნეთ დოკუმენტი Dotm ფაილების სხვადასხვა ელექტრონული ხელმოწერებისთვის ახლავე, ეწვიეთ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ვებსაიტს.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "მოძებნეთ სხვა Text ხელმოწერები C#-ის გამოყენებით"
    content: |
        "ელექტრონული ხელმოწერების ძიება სხვადასხვა დოკუმენტში. იპოვეთ ხელმოწერები ფაილის ერთ-ერთი პოპულარული ფორმატიდან, როგორც ეს ნაჩვენებია ქვემოთ."
    format: 
           
       
back_to_top:
    enable: true
---