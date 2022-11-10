---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Csv
productName: Java
lang: ka
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Csv for Java

############################# Head ############################
head_title: "მეტამონაცემების ელექტრონული ხელმოწერების დამატება Csv დოკუმენტებზე Java-ის მეშვეობით"
head_description: "გამოიყენეთ მეტამონაცემები, როგორც ფარული ელექტრონული ხელმოწერები თქვენს Csv დოკუმენტებში Java კოდის რამდენიმე სტრიქონის გამოყენებით. გამოიყენეთ GroupDocs Document Signature API თქვენი ბიზნეს დოკუმენტებისა და ფაილების ელექტრონული ხელმოწერისთვის მეტამონაცემების ინფორმაციით."

############################# Header ############################
title: "მეტამონაცემების ელექტრონული ხელმოწერები Csv დოკუმენტისთვის Java-ის მეშვეობით მარტივი და მარტივი გამოსაყენებელია!"
description: "მოაწერეთ თქვენი Csv დოკუმენტები და კონტრაქტები ფარული მეტამონაცემების ჩანაწერებით. შექმენით მეტამონაცემები PDF-ებისთვის, MS Word დოკუმენტებისთვის, MS Excel სამუშაო წიგნებისთვის, MS PowerPoint პრეზენტაციებისთვის და სხვადასხვა გამოსახულების ფორმატებისთვის უპრობლემოდ და დამატებითი კოდირების გარეშე."
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
    title: "GroupDocs.Signature for Java მეტამონაცემების ხელმოწერების API-ს შესახებ"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) არის პოპულარული API ციფრული დოკუმენტების ელექტრონული ხელმოწერისთვის. ხელმოწერები, როგორიცაა ტექსტები, სურათები, ციფრული სერთიფიკატები, შტრიხკოდები, QR-კოდები, შტამპები ან მეტამონაცემები ხელმისაწვდომია. ხელმოწერები შეიძლება განთავსდეს PDF-ებზე, MS Word დოკუმენტებზე, MS Excel სამუშაო წიგნებზე, MS PowerPoint პრეზენტაციებზე, Adobe Photoshop ფაილებსა და გამოსახულების სხვადასხვა ფორმატებზე. კლიენტებს შეუძლიათ ხელი მოაწერონ თავიანთ დოკუმენტს და განაახლონ, მოძებნონ, გადაამოწმონ, წაშალონ ან გადახედონ ამ დოკუმენტებზე განთავსებული ელექტრონული ხელმოწერების. უფრო მეტიც, გათვალისწინებულია ხელმოწერების პერსონალიზაციის უამრავი შესაძლებლობა.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Csv-ით ხელმოწერის ნაბიჯები Metadata-ით Java-ში"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) იძლევა შესაძლებლობას მოაწეროთ Csv დოკუმენტები Metadata ხელმოწერებით სწრაფად და მარტივად.
        
        * შექმენით ხელმოწერის კლასის მაგალითი, რომელიც უზრუნველყოფს Csv ფაილს, რომელიც უნდა მოაწეროს ხელი, როგორც გზა ან მეხსიერების ნაკადი
        * Instantate SignOptions კლასი და დააყენეთ ყველა მოთხოვნილი მონაცემი.
        * გამოიძახეთ Signature.Sign() მეთოდი, რომელიც გადასცემს გამომავალ Csv ფაილს ან მეხსიერების ნაკადს

    title_right: " სისტემის მოთხოვნები"
    content_right: |
        GroupDocs.Signature for Java მხარდაჭერილია ყველა ძირითად პლატფორმაზე და ოპერაციულ სისტემაზე. ქვემოთ მოცემული კოდის შესრულებამდე, დარწმუნდით, რომ თქვენს სისტემაში დაინსტალირებული გაქვთ შემდეგი წინაპირობები.

        * ოპერაციული სისტემები: Microsoft Windows, Linux, MacOS
        * განვითარების გარემო: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * მიიღეთ უახლესი GroupDocs.Signature for Java [Maven]-ისგან (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Csv file
        String filePath = "input.csv";
        // Set up output file
        String outputFilePath = "output.csv";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Csv document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "დოკუმენტების Csv ხელმოწერა Metadata Live Demo-ით"
    content: |
       მოაწერეთ Csv ფაილი სხვადასხვა ხელმოწერებით ახლავე, ეწვიეთ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ვებსაიტს. უფასო ონლაინ დემო გელოდებათ.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "სხვა მხარდაჭერილი Metadata ხელმოწერები Java-ისთვის"
    content: |
        "თქვენ ასევე შეგიძლიათ მოაწეროთ Csv ხელმოწერის სხვა ტიპებით. გთხოვთ იხილოთ სია ქვემოთ."
    format: 
       
       
back_to_top:
    enable: true
---