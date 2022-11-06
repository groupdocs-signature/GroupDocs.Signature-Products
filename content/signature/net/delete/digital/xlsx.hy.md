---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Xlsx
productName: .NET
lang: hy
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xlsx for C#

############################# Head ############################
head_title: "Ջնջել Digital ստորագրությունները Xlsx ֆայլերից C#-ի միջոցով"
head_description: "Ստորագրված Xlsx փաստաթղթերից որոշակի Digital ստորագրությունների ջնջումը կարող է հեշտությամբ իրականացվել կարճ .NET կոդով:"

############################# Header ############################
title: "Հեռացրեք Digital ստորագրությունները, որոնք տեղադրված են Xlsx ֆայլերում"
description: "Ջնջել տարբեր Digital ստորագրությունները Xlsx փաստաթղթերից: Digital ստորագրությունները հեռացնելու համար անհրաժեշտ է պարզ C# կոդ:"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Ստացեք տեղեկություններ GroupDocs.Signature for .NET API-ի առանձնահատկությունների մասին"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API-ն ապահովում է ձեր փաստաթղթերը էլեկտրոնային ստորագրությունների միջոցով մշակելու բազմաթիվ եղանակներ: Հասանելի են թվային ստորագրություններ, ինչպիսիք են տեքստերը, պատկերները, թվային վկայագրերը, շտրիխ կոդերը, QR-կոդերը, նամականիշերը կամ մետատվյալները: Հաճախորդները հնարավորություն ունեն ավելացնել, ջնջել, թարմացնել, ստուգել կամ որոնել թվային ստորագրություններ PDF ֆայլերում, MS Word փաստաթղթերում, MS Excel աշխատանքային գրքույկներում, MS PowerPoint շնորհանդեսներում, Adobe Photoshop ֆայլերում և տարբեր պատկերների ձևաչափերում: Տրամադրված են մեծ թվով օգտակար գործառույթներ և կարգավորումներ:
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Ինչպես հեռացնել Digital ստորագրությունները ձեր Xlsx փաստաթղթից"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) օգտակար հատկություն է տրամադրում Xlsx փաստաթղթերը Digital ստորագրություններից մի քանի տող կոդով մաքրելու համար:
        
        * Նախ, որպես կոնստրուկտորի պարամետր, օրինականացրեք Signature օբյեկտը, որն անցնում է ձեր փաստաթղթի ուղին:
        * Այնուհետև ստեղծեք համապատասխան ստորագրության օբյեկտ և ստեղծեք դրա եզակի նույնացուցիչը:
        * Դրանից հետո կանչեք Delete մեթոդը, որն անցնում է ստորագրության օբյեկտ, որը պետք է ջնջվի:
        * Վերջապես, գործընթացի գործողության արդյունքները:

    title_right: "Համակարգի պահանջները"
    content_right: |
        GroupDocs.Signature for .NET-ն աջակցվում է բոլոր հիմնական հարթակներում և օպերացիոն համակարգերում: Նախքան ստորև նշված կոդը գործարկելը, խնդրում ենք համոզվել, որ ձեր համակարգում տեղադրված են հետևյալ նախադրյալները.

        * Օպերացիոն համակարգեր՝ Microsoft Windows, Linux, MacOS
        * Մշակման միջավայրեր՝ Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Ներբեռնեք GroupDocs.Signature for .NET-ի վերջին տարբերակը [Nuget]-ից (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xlsx file
        string filePath = "input.xlsx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "a01e1940-997a-444b-89af-9309a2d559a5";

                // provide signature features to delete
                // set up particular signature id
                DigitalSignature signatureToDelete = new DigitalSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ստորագրում Digital ստորագրություններով Live Demo"
    content: |
       Ավելացրեք տարբեր էլեկտրոնային ստորագրություններ Xlsx ֆայլին հենց հիմա՝ այցելելով [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) կայքը:          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ջնջեք ձեր Digital ստորագրությունները C#-ով"
    content: |
        "Էլեկտրոնային ստորագրությունների ջնջում, որոնք ավելացվել են փաստաթղթերի տարբեր ձևաչափերում: Հեռացրեք ստորագրությունները արագ առանց լրացուցիչ կոդի:"
    format: 
       
       
back_to_top:
    enable: true
---