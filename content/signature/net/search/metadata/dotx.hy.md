---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Dotx
productName: .NET
lang: hy
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Dotx with C#

############################# Head ############################
head_title: "Որոնեք Metadata ստորագրությունները Dotx ֆայլում C#-ում"
head_description: "Օգտագործեք .NET՝ Metadata ստորագրությունները Dotx ֆայլերում մի քանի տող կոդով որոնելու համար:"

############################# Header ############################
title: "Փնտրեք Metadata ստորագրությունները Dotx ֆայլում"
description: ".NET բնօրինակ API-ն թույլ է տալիս որոնել Metadata ստորագրություններ արդեն ստորագրված Dotx ֆայլերում: Կատարեք էլեկտրոնային ստորագրության առաջադեմ որոնում ձեր Dotx փաստաթղթերում՝ օգտագործելով մի քանի տող կոդ:"
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
    title: "GroupDocs.Signature for .NET API-ի մասին"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) տրամադրում է .NET API փաստաթղթերի մշակման համար՝ օգտագործելով տարբեր տեսակի ստորագրություններ, ինչպիսիք են տեքստերը, պատկերները, թվային վկայագրերը, շտրիխ կոդերը, QR-կոդերը, դրոշմանիշները կամ մետատվյալները: Օգտատերերը կարող են ավելացնել, ջնջել, թարմացնել, հաստատել կամ որոնել էլեկտրոնային ստորագրությունները PDF ֆայլերում, MS Word փաստաթղթերում, MS Excel աշխատանքային գրքույկներում, MS PowerPoint-ի շնորհանդեսներում, Adobe Photoshop ֆայլերում և պատկերի տարբեր ձևաչափերում՝ անհրաժեշտության դեպքում ստորագրությունների հատկությունները հարմարեցնելու համար լրացուցիչ աջակցությամբ:
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Ինչպես որոնել Metadata ստորագրությունները Dotx-ում"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) հեշտացնում է .NET ծրագրավորողների համար որոնել Metadata ստորագրությունները Dotx ֆայլերում իրենց հավելվածներից` իրականացնելով մի քանի հեշտ քայլեր:
        
        * Ստեղծեք Signature դասի նոր օրինակ և փոխանցեք աղբյուրի փաստաթղթի ուղին որպես կոնստրուկտորի պարամետր:
        * Ստեղծեք SearchOptions օբյեկտը ձեր պահանջներին համապատասխան և նշեք որոնման տարբերակները:
        * Զանգահարեք «Signature» դասի օրինակի որոնման մեթոդը և փոխանցեք «SearchOptions»-ը:
        * Որոնման արդյունքները մշակեք ձեր պահանջներին համապատասխան:

    title_right: "Համակարգի պահանջները"
    content_right: |
        GroupDocs.Signature for .NET-ն աջակցվում է բոլոր հիմնական հարթակներում և օպերացիոն համակարգերում: Նախքան ստորև նշված կոդը գործարկելը, խնդրում ենք համոզվել, որ ձեր համակարգում տեղադրված են հետևյալ նախադրյալները.

        * Օպերացիոն համակարգեր՝ Microsoft Windows, Linux, MacOS
        * Մշակման միջավայրեր՝ Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Ներբեռնեք GroupDocs.Signature for .NET-ի վերջին տարբերակը [Nuget]-ից (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Dotx file
        string filePath = "input.dotx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // search for Metadata signatures in Dotx document
                List<WordProcessingMetadataSignature> signatures = signature.Search<WordProcessingMetadataSignature>(SignatureType.Metadata);

                // process signatures which were found 
                foreach (WordProcessingMetadataSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Որոնեք Metadata էլեկտրոնային ստորագրություններ Live Demo"
    content: |
       Փնտրեք փաստաթղթում Dotx ֆայլերի տարբեր էլեկտրոնային ստորագրություններ հենց հիմա՝ այցելելով [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) կայքը:

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Որոնեք այլ Metadata ստորագրություններ՝ օգտագործելով C#"
    content: |
        "Էլեկտրոնային ստորագրությունների որոնում տարբեր փաստաթղթերում: Գտեք ստորագրություններ հանրաճանաչ ֆայլերի ձևաչափերից, ինչպես ցույց է տրված ստորև:"
    format: 
           
       
back_to_top:
    enable: true
---