---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Code39
fileformat: Odp
productName: Java
lang: ka
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Odp for Java

############################# Head ############################
head_title: "eSign Odp დოკუმენტი Code39 შტრიხკოდით Java-ში"
head_description: "შექმენით Code39 შტრიხკოდის ხელმოწერა და განათავსეთ იგი Odp დოკუმენტზე Java კოდის რამდენიმე ხაზის გამოყენებით. გამოიყენეთ GroupDocs Document Signature API სხვადასხვა ფაილის ფორმატების ხელმოწერისთვის."

############################# Header ############################
title: "შექმენით Code39 შტრიხკოდის ხელმოწერა Odp დოკუმენტისთვის Java-ში"
description: "მოაწერეთ თქვენი {{ფაილის ფორმატი}} ბიზნეს დოკუმენტები Code39 შტრიხკოდით. შექმენით შტრიხკოდის ხელმოწერა სწრაფად და მარტივად რამდენიმე ხაზის კოდით ხელმოწერის ვარიანტების დასაყენებლად."
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
    title: "GroupDocs.Signature for Java შტრიხკოდის ხელმოწერების API-ს შესახებ."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) არის სწრაფი და მარტივი API ციფრული დოკუმენტების ელექტრონული ხელმოწერის სამართავად შტრიხკოდების ტიპების გამოყენებით, როგორიცაა UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN. , ITF14 და მრავალი სხვა. მომხმარებლებს შეუძლიათ მარტივად შექმნან შტრიხკოდები, რომლებიც უზრუნველყოფენ საჭირო ტექსტს და განათავსონ ისინი PDF, Microsoft Office Words დოკუმენტები, Microsoft Office Excel სამუშაო წიგნები, MS PowerPoint პრეზენტაციები, Adobe Photoshop ფაილები და გამოსახულების სხვადასხვა ფორმატში. დოკუმენტებში განთავსებული შტრიხკოდების განახლება, ძებნა, შემოწმება, წაშლა ან წინასწარი ნახვა შესაძლებელია. უფრო მეტიც, შტრიხკოდების პერსონალიზაცია მხარდაჭერილია.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Odp-ით ხელმოწერის ნაბიჯები Barcode-ით Java-ში"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) იძლევა შესაძლებლობას მოაწეროთ Odp დოკუმენტები Barcode ხელმოწერებით სწრაფად და მარტივად.
        
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
                
        // Set up input Odp file
        String filePath = "input.odp";
        // Set up output file
        String outputFilePath = "output.odp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Code39);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Odp document
        SignResult result = signature.sign(outputFilePath, options);

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
          title: "About Code39 Barcode"
          content: |
            კოდი 39 (ასევე ცნობილი როგორც Alpha39, Code 3 of 9, Code 3/9, Type 39, USS Code 39, ან USD-3) არის ცვლადი სიგრძის, დისკრეტული შტრიხკოდის სიმბოლიკა.
          characterset: |
             რიცხვითი ციფრები (0-9) და დიდი ასოები (A-Z) და სპეციალური სიმბოლოების რაოდენობა (-, ., $, /, +, %, და სივრცე).
          textcapacity: |
             არანაირი კონკრეტული შეზღუდვა.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "სხვა მხარდაჭერილი Barcode ხელმოწერები Java-ისთვის"
    content: |
        "თქვენ ასევე შეგიძლიათ მოაწეროთ {{ფაილის ფორმატი}} ხელმოწერის სხვა ტიპებით. გთხოვთ იხილოთ სია ქვემოთ."
    format: 
        
       
back_to_top:
    enable: true
---