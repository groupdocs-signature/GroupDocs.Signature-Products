---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Xlsx
productName: Java
lang: ka
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Xlsx for Java

############################# Head ############################
head_title: "Image ხელმოწერების დამატება Xlsx ფაილში Java-ით"
head_description: "განათავსეთ Image ხელმოწერა Xlsx ფაილზე Java კოდის რამდენიმე ხაზის გამოყენებით. გამოიყენეთ GroupDocs Document Signature API ათობით ფაილის ფორმატის ხელმოწერისთვის."

############################# Header ############################
title: "შედით Xlsx ფაილებში Image ხელმოწერებით Java-ში"
description: "როგორ დავამატოთ Image ხელმოწერა Java კოდის რამდენიმე ხაზით"
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
    title: "შესახებ GroupDocs.Signature for Java Image signatures API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) არის პოპულარული API ციფრული დოკუმენტების ელექტრონული ხელმოწერისთვის. ხელმოწერები, როგორიცაა ტექსტები, სურათები, ციფრული სერთიფიკატები, შტრიხკოდები, QR-კოდები, შტამპები ან მეტამონაცემები ხელმისაწვდომია. ხელმოწერები შეიძლება განთავსდეს PDF-ებზე, MS Word დოკუმენტებზე, MS Excel სამუშაო წიგნებზე, MS PowerPoint პრეზენტაციებზე, Adobe Photoshop ფაილებსა და გამოსახულების სხვადასხვა ფორმატებზე. კლიენტებს შეუძლიათ ხელი მოაწერონ თავიანთ დოკუმენტს და განაახლონ, მოძებნონ, გადაამოწმონ, წაშალონ ან გადახედონ ამ დოკუმენტებზე განთავსებული ელექტრონული ხელმოწერების. უფრო მეტიც, გათვალისწინებულია ხელმოწერების პერსონალიზაციის უამრავი შესაძლებლობა.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Xlsx-ით ხელმოწერის ნაბიჯები Image-ით Java-ში"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) იძლევა შესაძლებლობას მოაწეროთ Xlsx დოკუმენტები Image ხელმოწერებით სწრაფად და მარტივად.
        
        * შექმენით ხელმოწერის კლასის მაგალითი, რომელიც უზრუნველყოფს {{ფაილის ფორმატი}} ფაილს, რომელიც უნდა მოაწეროს ხელი, როგორც გზა ან მეხსიერების ნაკადი
        * Instantate SignOptions კლასი და დააყენეთ ყველა მოთხოვნილი მონაცემი.
        * გამოიძახეთ Signature.Sign() მეთოდი, რომელიც გადასცემს გამომავალ {{ფაილის ფორმატი}} ფაილს ან მეხსიერების ნაკადს

    title_right: " სისტემის მოთხოვნები"
    content_right: |
        GroupDocs.Signature for Java მხარდაჭერილია ყველა ძირითად პლატფორმაზე და ოპერაციულ სისტემაზე. ქვემოთ მოცემული კოდის შესრულებამდე, დარწმუნდით, რომ თქვენს სისტემაში დაინსტალირებული გაქვთ შემდეგი წინაპირობები.

        * ოპერაციული სისტემები: Microsoft Windows, Linux, MacOS
        * განვითარების გარემო: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * მიიღეთ უახლესი GroupDocs.Signature for Java [Maven]-ისგან (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsx file
        String filePath = "input.xlsx";
        // Set up output file
        String outputFilePath = "output.xlsx";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Xlsx document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "დოკუმენტების {{ფაილის ფორმატი}} ხელმოწერა Image Live Demo-ით"
    content: |
       მოაწერეთ {{ფაილის ფორმატი}} ფაილი სხვადასხვა ხელმოწერებით ახლავე, ეწვიეთ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ვებსაიტს. უფასო ონლაინ დემო გელოდებათ.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "სხვა მხარდაჭერილი Image ხელმოწერები Java-ისთვის"
    content: |
        "თქვენ ასევე შეგიძლიათ მოაწეროთ {{ფაილის ფორმატი}} ხელმოწერის სხვა ტიპებით. გთხოვთ იხილოთ სია ქვემოთ."
    format: 
       
       
back_to_top:
    enable: true
---