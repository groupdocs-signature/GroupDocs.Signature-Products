---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Zip
productName: Java
lang: hy
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Zip for Java

############################# Head ############################
head_title: "Digital ստորագրությունների ստուգում Zip ֆայլերի համար Java-ի միջոցով"
head_description: "Օգտագործեք Java կոդի ընդամենը մի քանի տող Zip փաստաթղթերը և դրանց Digital ստորագրությունները ստուգելու համար:"

############################# Header ############################
title: "Digital ստորագրությունների ստուգում Zip ֆայլերի համար"
description: "Java-ի API-ն հնարավորություն է տալիս ստուգել Digital ստորագրությունները Zip փաստաթղթերում: Ձեր Zip փաստաթղթերում էլեկտրոնային ստորագրությունների ստուգումը կարող է իրականացվել արագ և հեշտությամբ:"
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
    title: "Բացահայտեք GroupDocs.Signature for Java API-ի նոր հնարավորությունները"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API-ն ապահովում է բազմաթիվ փաստաթղթերի ձևաչափեր մշակելու եղանակների լայն շրջանակ՝ օգտագործելով էլեկտրոնային ստորագրությունները: Աջակցվում են թվային ստորագրությունների բազմաթիվ տեսակներ, ինչպիսիք են տեքստերը, պատկերները, թվային վկայագրերը, շտրիխ կոդերը, QR-կոդերը, նամականիշերը կամ մետատվյալները: Հաճախորդները կարող են ավելացնել, հեռացնել, խմբագրել, վավերացնել կամ որոնել թվային ստորագրություններ PDF ֆայլերում, MS Word փաստաթղթերում, MS Excel աշխատանքային գրքույկներում, MS PowerPoint շնորհանդեսներում, Adobe Photoshop ֆայլերում և պատկերի տարբեր ձևաչափերում: Հասանելի են ապշեցուցիչ թվով լրացուցիչ հնարավորություններ և կարգավորումներ:
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Ինչպես վավերացնել Digital ստորագրությունները ձեր Zip փաստաթղթում"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ներառում է օգտակար գործառույթներ, ինչպիսիք են Digital ստորագրությունները, որոնք տեղադրված են Zip փաստաթղթերում: Օգտվե՛ք այս հնարավորությունից՝ առանց լրացուցիչ կոդի ներդրման։
        
        * Նախ, ակնարկեք Signature դասը, որն ապահովում է որպես կոնստրուկտորի պարամետրի ուղի դեպի փաստաթուղթ, որը պետք է ստուգվի:
        * Երկրորդ, ստեղծեք նոր VerifyOptions օբյեկտ և կարգավորեք բոլոր անհրաժեշտ հատկությունները:
        * Վերջապես, կանչեք Signature's object Verify մեթոդը՝ անցնելով VerifyOptions օրինակը:
        * Այնուհետև մշակեք ստուգման արդյունքները:

    title_right: "Համակարգի պահանջները"
    content_right: |
        GroupDocs.Signature for Java-ն աջակցվում է բոլոր հիմնական հարթակներում և օպերացիոն համակարգերում: Նախքան ստորև նշված կոդը գործարկելը, խնդրում ենք համոզվել, որ ձեր համակարգում տեղադրված են հետևյալ նախադրյալները.

        * Օպերացիոն համակարգեր՝ Microsoft Windows, Linux, MacOS
        * Մշակման միջավայրեր՝ NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Ներբեռնեք GroupDocs.Signature for Java-ի վերջին տարբերակը [Maven]-ից (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Zip file
        String filePath = "input.zip";

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
    title: "Ստորագրում Digital ստորագրություններով Live Demo"
    content: |
       Ավելացրեք տարբեր էլեկտրոնային ստորագրություններ Zip ֆայլին հենց հիմա՝ այցելելով [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) կայքը:          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ստուգեք այլ Digital ստորագրությունները՝ օգտագործելով Java"
    content: |
        "Տարբեր փաստաթղթերում տեղադրված էլեկտրոնային ստորագրությունների ստուգում. Ստուգեք ստորագրությունների որակը հանրաճանաչ ֆայլերի ձևաչափերում, ինչպես ցույց է տրված ստորև:"
    format: 
       
       
back_to_top:
    enable: true
---