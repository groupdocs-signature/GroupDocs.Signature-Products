---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Tiff
productName: Java
lang: hy
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Tiff for Java

############################# Head ############################
head_title: "Կցեք մետատվյալների էլեկտրոնային ստորագրությունները Tiff փաստաթղթերին Java-ի միջոցով"
head_description: "Օգտագործեք Մետատվյալները որպես թաքնված էլեկտրոնային ստորագրություններ ձեր Tiff փաստաթղթերի ներսում՝ օգտագործելով Java կոդի մի քանի տող: Օգտագործեք GroupDocs Document Signature API-ը՝ ձեր բիզնես փաստաթղթերն ու ֆայլերը մետատվյալներով էլեկտրոնային ստորագրելու համար:"

############################# Header ############################
title: "Tiff փաստաթղթի մետատվյալների էլեկտրոնային ստորագրությունները Java-ի միջոցով պարզ են և հեշտ օգտագործման համար:"
description: "e-ստորագրեք ձեր Tiff փաստաթղթերն ու պայմանագրերը թաքնված մետատվյալների գրառումներով: Ստեղծեք մետատվյալներ PDF ֆայլերի, MS Word փաստաթղթերի, MS Excel աշխատանքային գրքույկների, MS PowerPoint ներկայացումների և պատկերի տարբեր ձևաչափերի համար՝ առանց խնդիրների և լրացուցիչ կոդավորման:"
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
    title: "GroupDocs.Signature for Java Մետատվյալների ստորագրությունների API-ի մասին"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) հայտնի API է թվային փաստաթղթերի էլեկտրոնային ստորագրման համար: Ստորագրություններ, ինչպիսիք են տեքստերը, պատկերները, թվային վկայագրերը, շտրիխ կոդերը, QR-կոդերը, նամականիշերը կամ մետատվյալները հասանելի են: Ստորագրությունները կարող են տեղադրվել PDF ֆայլերի, MS Word փաստաթղթերի, MS Excel աշխատանքային գրքերի, MS PowerPoint ներկայացումների, Adobe Photoshop ֆայլերի և պատկերի տարբեր ձևաչափերի վրա: Հաճախորդները կարող են ստորագրել իրենց փաստաթուղթը և թարմացնել, որոնել, ստուգել, ​​ջնջել կամ նախադիտել այդ փաստաթղթերի վրա դրված էլեկտրոնային ստորագրությունները: Ավելին, տրամադրվում են ստորագրությունների հարմարեցման բազմաթիվ հնարավորություններ։
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Tiff-ը Metadata-ով Java-ով ստորագրելու քայլեր"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) հնարավորություն է տալիս արագ և հեշտությամբ ստորագրել Tiff փաստաթղթերը Metadata ստորագրություններով:
        
        * Ստեղծեք Signature դասի օրինակ, որը տրամադրում է Tiff ֆայլ, որը պետք է ստորագրվի որպես ճանապարհ կամ հիշողության հոսք
        * Տեղադրեք SignOptions դասը և սահմանեք բոլոր պահանջվող տվյալները:
        * Հրավիրեք Signature.Sign() մեթոդը՝ փոխանցելով ելքային Tiff ֆայլը կամ հիշողության հոսքը

    title_right: " Համակարգի պահանջները"
    content_right: |
        GroupDocs.Signature for Java-ն աջակցվում է բոլոր հիմնական հարթակներում և օպերացիոն համակարգերում: Նախքան ստորև նշված կոդը գործարկելը, խնդրում ենք համոզվել, որ ձեր համակարգում տեղադրված են հետևյալ նախադրյալները.

        * Օպերացիոն համակարգեր՝ Microsoft Windows, Linux, MacOS
        * Մշակման միջավայրեր՝ NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Ստացեք վերջին GroupDocs.Signature for Java-ը [Maven]-ից (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Tiff file
        String filePath = "input.tiff";
        // Set up output file
        String outputFilePath = "output.tiff";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Tiff document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Tiff փաստաթղթերի ստորագրում Metadata Live Demo-ով"
    content: |
       Ստորագրեք Tiff ֆայլը տարբեր ստորագրություններով հենց հիմա՝ այցելելով [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) կայքը: Անվճար առցանց ցուցադրություն սպասում է ձեզ:          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Այլ աջակցվող Metadata ստորագրություններ Java-ի համար"
    content: |
        "Դուք կարող եք նաև ստորագրել Tiff ստորագրության այլ տեսակներով: Խնդրում ենք տեսնել ստորև ներկայացված ցուցակը:"
    format: 
       
       
back_to_top:
    enable: true
---