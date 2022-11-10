---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Pptm
productName: Java
lang: ka
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pptm for Java

############################# Head ############################
head_title: "Digital ხელმოწერების დადასტურება Pptm ფაილებისთვის Java-ით"
head_description: "გამოიყენეთ Java კოდის მხოლოდ რამდენიმე ხაზი Pptm დოკუმენტებისა და მათი Digital ხელმოწერების დასადასტურებლად."

############################# Header ############################
title: "Digital ხელმოწერების დადასტურება Pptm ფაილებისთვის"
description: "API Java-ისთვის იძლევა შესაძლებლობას გადაამოწმოთ Digital ხელმოწერები Pptm დოკუმენტებში. თქვენი Pptm დოკუმენტებში ელექტრონული ხელმოწერების დადასტურება შეიძლება სწრაფად და მარტივად განხორციელდეს."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "აღმოაჩინეთ ახალი GroupDocs.Signature for Java API ფუნქციები"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API გთავაზობთ მრავალი დოკუმენტის ფორმატის დამუშავების გზებს ელექტრონული ხელმოწერების გამოყენებით. მხარდაჭერილია მრავალი სახის ციფრული ხელმოწერა, როგორიცაა ტექსტები, სურათები, ციფრული სერთიფიკატები, შტრიხკოდები, QR-კოდები, შტამპები ან მეტამონაცემები. კლიენტებს შეუძლიათ დაამატონ, წაშალონ, შეცვალონ, დაადასტურონ ან მოძებნონ ციფრული ხელმოწერები PDF ფაილებში, MS Word დოკუმენტებში, MS Excel სამუშაო წიგნებში, MS PowerPoint პრეზენტაციებში, Adobe Photoshop ფაილებსა და გამოსახულების სხვადასხვა ფორმატებში. გასაოცარი რაოდენობის დამატებითი ფუნქციები და პარამეტრები ხელმისაწვდომია.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "როგორ გადავამოწმოთ Digital ხელმოწერები თქვენს Pptm დოკუმენტში"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) შეიცავს სასარგებლო ფუნქციებს, როგორიცაა Digital ხელმოწერების დადასტურება, რომლებიც განთავსებულია Pptm დოკუმენტებზე. გამოიყენეთ ეს შესაძლებლობა დამატებითი კოდის განხორციელების გარეშე.
        
        * უპირველეს ყოვლისა, შექმენით Signature კლასი, რომელიც უზრუნველყოფს როგორც კონსტრუქტორის პარამეტრის გზას დოკუმენტში, რომელიც უნდა იყოს გადამოწმებული.
        * მეორეც, შექმენით ახალი VerifyOptions ობიექტი და დააყენეთ ყველა საჭირო თვისება.
        * და ბოლოს, გამოიძახეთ Signature-ის ობიექტი Verify მეთოდი VerifyOptions ინსტანციის გავლით.
        * შემდეგ დაამუშავეთ გადამოწმების შედეგები.

    title_right: "სისტემის მოთხოვნები"
    content_right: |
        GroupDocs.Signature for Java მხარდაჭერილია ყველა ძირითად პლატფორმაზე და ოპერაციულ სისტემაზე. ქვემოთ მოცემული კოდის შესრულებამდე, დარწმუნდით, რომ თქვენს სისტემაში დაინსტალირებული გაქვთ შემდეგი წინაპირობები.

        * ოპერაციული სისტემები: Microsoft Windows, Linux, MacOS
        * განვითარების გარემო: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * ჩამოტვირთეთ GroupDocs.Signature for Java-ის უახლესი ვერსია [Maven]-დან (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pptm file
        String filePath = "input.pptm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2020, 12, 12));
        options.setSignDateTimeTo(new Date(2022, 12, 12));
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
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
    title: "დაადასტურეთ სხვა Digital ხელმოწერები Java-ის გამოყენებით"
    content: |
        "სხვადასხვა დოკუმენტებში განთავსებული ელექტრონული ხელმოწერების შემოწმება. შეამოწმეთ ხელმოწერების ხარისხი პოპულარული ფაილის ფორმატებში, როგორც ეს ნაჩვენებია ქვემოთ."
    format: 
       
       
back_to_top:
    enable: true
---