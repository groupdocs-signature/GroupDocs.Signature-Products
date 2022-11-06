---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Xltx
productName: .NET
lang: ka
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Xltx with C#

############################# Head ############################
head_title: "მოძებნეთ Image ხელმოწერები Xltx ფაილში C#"
head_description: "გამოიყენეთ .NET Image ხელმოწერების მოსაძიებლად Xltx ფაილებში კოდის რამდენიმე ხაზის გამოყენებით."

############################# Header ############################
title: "მოძებნეთ Image ხელმოწერები Xltx ფაილში"
description: ".NET მშობლიური API საშუალებას გაძლევთ მოძებნოთ Image ხელმოწერები უკვე ხელმოწერილ Xltx ფაილებში. განახორციელეთ ელექტრონული ხელმოწერის გაფართოებული ძიება თქვენს {{ფაილის ფორმატში}} დოკუმენტებში კოდის რამდენიმე ხაზის გამოყენებით."
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
    title_left: "როგორ მოძებნოთ Image ხელმოწერები Xltx-ში"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) აადვილებს .NET დეველოპერებს აპლიკაციებიდან ფაილებში Image ხელმოწერების ძიებას რამდენიმე მარტივი ნაბიჯის განხორციელებით.
        
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
                
        // Set up input Xltx file
        string filePath = "input.xltx";

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

                // search for Image signatures in Xltx document
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
    title: "მოძებნეთ Image ელექტრონული ხელმოწერების ცოცხალი დემო"
    content: |
       მოძებნეთ დოკუმენტი Xltx ფაილების სხვადასხვა ელექტრონული ხელმოწერებისთვის ახლავე, ეწვიეთ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ვებსაიტს.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "მოძებნეთ სხვა Image ხელმოწერები C#-ის გამოყენებით"
    content: |
        "ელექტრონული ხელმოწერების ძიება სხვადასხვა დოკუმენტში. იპოვეთ ხელმოწერები ფაილის ერთ-ერთი პოპულარული ფორმატიდან, როგორც ეს ნაჩვენებია ქვემოთ."
    format: 
           
       
back_to_top:
    enable: true
---