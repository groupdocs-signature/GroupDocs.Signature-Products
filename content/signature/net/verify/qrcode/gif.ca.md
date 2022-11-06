---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Gif
productName: .NET
lang: ca
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Gif for C#

############################# Head ############################
head_title: "Verificació de signatures de Qrcode per a fitxers Gif mitjançant C#"
head_description: "Utilitzeu només unes poques línies de codi .NET per verificar els documents Gif i les seves signatures Qrcode."

############################# Header ############################
title: "Qrcode verificació de signatures per a fitxers Gif"
description: "L'API per a .NET ofereix l'oportunitat de verificar les signatures de Qrcode als documents Gif. La verificació de les signatures electròniques dins dels vostres documents Gif es pot fer de manera ràpida i senzilla."
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
    title: "Descobriu noves funcions de l'API de GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API ofereix una àmplia gamma de maneres de processar nombrosos formats de documents mitjançant signatures electròniques. S'admeten molts tipus de signatures digitals com textos, imatges, certificats digitals, codis de barres, codis QR, segells o metadades. Els clients poden afegir, eliminar, editar, validar o cercar signatures digitals en PDF, documents MS Word, llibres de treball de MS Excel, presentacions MS PowerPoint, fitxers Adobe Photoshop i diversos formats d'imatge. Hi ha disponibles un nombre sorprenent de funcions i configuracions addicionals.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Com validar les signatures de Qrcode al vostre document Gif"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) inclou funcions útils com la verificació de les signatures de Qrcode col·locades als documents de Gif. Aprofiteu aquesta oportunitat sense implementar codi addicional.
        
        * En primer lloc, instanciïu la classe Signature proporcionant com a paràmetre de constructor la ruta d'accés a un document que se suposa que s'ha de verificar.
        * En segon lloc, creeu un nou objecte VerifyOptions i configureu totes les propietats necessàries.
        * Finalment, invoqueu el mètode Verify de l'objecte de Signature passant la instància VerifyOptions.
        * A continuació, processeu els resultats de la verificació.

    title_right: "Requisits del sistema"
    content_right: |
        GroupDocs.Signature for .NET són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.

        * Sistemes operatius: Microsoft Windows, Linux, MacOS
        * Entorns de desenvolupament: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Baixeu la darrera versió de GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Gif file
        string filePath = "input.gif";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                QrCodeVerifyOptions options = new QrCodeVerifyOptions()
                {
                    // process only first page
                    PagesSetup = new PagesSetup() { FirstPage = true },
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.StartsWith,
                    // specify text pattern to search
                    Text = "QrCode text",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signant amb Qrcode signatures Demostració en directe"
    content: |
       Afegiu diverses signatures electròniques al fitxer Gif ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verifiqueu altres signatures de Qrcode mitjançant C#"
    content: |
        "Verificació de signatures electròniques col·locades en diversos documents. Comproveu la qualitat de les signatures en els formats de fitxer populars, tal com es mostra a continuació."
    format: 
       
       
back_to_top:
    enable: true
---