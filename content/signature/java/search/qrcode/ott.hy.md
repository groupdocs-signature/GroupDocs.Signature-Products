---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Ott
productName: Java
lang: hy
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Ott with Java

############################# Head ############################
head_title: "Որոնեք Qrcode ստորագրությունները Ott ֆայլում Java-ում"
head_description: "Օգտագործեք Java՝ Qrcode ստորագրությունները Ott ֆայլերում մի քանի տող կոդով որոնելու համար:"

############################# Header ############################
title: "Փնտրեք Qrcode ստորագրությունները Ott ֆայլում"
description: "Java բնօրինակ API-ն թույլ է տալիս որոնել Qrcode ստորագրություններ արդեն ստորագրված Ott ֆայլերում: Կատարեք էլեկտրոնային ստորագրության առաջադեմ որոնում ձեր Ott փաստաթղթերում՝ օգտագործելով մի քանի տող կոդ:"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java API-ի մասին"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) տրամադրում է Java API փաստաթղթերի մշակման համար՝ օգտագործելով տարբեր տեսակի ստորագրություններ, ինչպիսիք են տեքստերը, պատկերները, թվային վկայագրերը, շտրիխ կոդերը, QR-կոդերը, դրոշմանիշները կամ մետատվյալները: Օգտատերերը կարող են ավելացնել, ջնջել, թարմացնել, հաստատել կամ որոնել էլեկտրոնային ստորագրությունները PDF ֆայլերում, MS Word փաստաթղթերում, MS Excel աշխատանքային գրքույկներում, MS PowerPoint-ի շնորհանդեսներում, Adobe Photoshop ֆայլերում և պատկերի տարբեր ձևաչափերում՝ անհրաժեշտության դեպքում ստորագրությունների հատկությունները հարմարեցնելու համար լրացուցիչ աջակցությամբ:
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Ինչպես որոնել Qrcode ստորագրությունները Ott-ում"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) հեշտացնում է Java ծրագրավորողների համար որոնել Qrcode ստորագրությունները Ott ֆայլերում իրենց հավելվածներից` իրականացնելով մի քանի հեշտ քայլեր:
        
        * Ստեղծեք Signature դասի նոր օրինակ և փոխանցեք աղբյուրի փաստաթղթի ուղին որպես կոնստրուկտորի պարամետր:
        * Ստեղծեք SearchOptions օբյեկտը ձեր պահանջներին համապատասխան և նշեք որոնման տարբերակները:
        * Զանգահարեք «Signature» դասի օրինակի որոնման մեթոդը և փոխանցեք «SearchOptions»-ը:
        * Որոնման արդյունքները մշակեք ձեր պահանջներին համապատասխան:

    title_right: "Համակարգի պահանջները"
    content_right: |
        GroupDocs.Signature for Java-ն աջակցվում է բոլոր հիմնական հարթակներում և օպերացիոն համակարգերում: Նախքան ստորև նշված կոդը գործարկելը, խնդրում ենք համոզվել, որ ձեր համակարգում տեղադրված են հետևյալ նախադրյալները.

        * Օպերացիոն համակարգեր՝ Microsoft Windows, Linux, MacOS
        * Մշակման միջավայրեր՝ NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Ներբեռնեք GroupDocs.Signature for Java-ի վերջին տարբերակը [Maven]-ից (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ott file
        String filePath = "input.ott";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        QrCodeSearchOptions options = new QrCodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Qrcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Qrcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Qrcode signatures in Ott document
        List<QrCodeSignature> signatures = signature.search(QrCodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Որոնեք Qrcode էլեկտրոնային ստորագրություններ Live Demo"
    content: |
       Փնտրեք փաստաթղթում Ott ֆայլերի տարբեր էլեկտրոնային ստորագրություններ հենց հիմա՝ այցելելով [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) կայքը:

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Որոնեք այլ Qrcode ստորագրություններ՝ օգտագործելով Java"
    content: |
        "Էլեկտրոնային ստորագրությունների որոնում տարբեր փաստաթղթերում: Գտեք ստորագրություններ հանրաճանաչ ֆայլերի ձևաչափերից, ինչպես ցույց է տրված ստորև:"
    format: 
           
       
back_to_top:
    enable: true
---