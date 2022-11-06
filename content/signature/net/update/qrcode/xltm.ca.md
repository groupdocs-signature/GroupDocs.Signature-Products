---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Qrcode
fileformat: Xltm
productName: .NET
lang: ca
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Xltm for C#

############################# Head ############################
head_title: "Actualitza les signatures de Qrcode col·locades als fitxers Xltm amb C#"
head_description: "Utilitzeu el codi .NET senzill i fàcil d'entendre per a l'actualització de signatures de Qrcode en documents de Xltm signats."

############################# Header ############################
title: "Editeu i actualitzeu les signatures Qrcode col·locades als fitxers Xltm"
description: "L'API per a .NET proporciona funcionalitat per a les signatures de Qrcode que s'actualitzen als documents Xltm. Actualitzeu les signatures electròniques dins dels vostres documents Xltm amb un parell de línies de codi C# de manera ràpida i senzilla."
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
    title: "Més informació sobre les funcions de l'API de GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) La funcionalitat de l'API conté una àmplia selecció de mitjans per processar en formats de documents de demanda mitjançant signatures electròniques. S'admet un ampli espectre de signatures electròniques com textos, imatges, certificats digitals, codis de barres, codis QR, segells o metadades. Els clients poden afegir, eliminar, editar, validar o cercar signatures digitals en PDF, documents MS Word, llibres de treball de MS Excel, presentacions MS PowerPoint, fitxers Adobe Photoshop i diversos formats d'imatge. Hi ha disponibles nombroses funcions i configuracions útils.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Com canviar les signatures de Qrcode al vostre document Xltm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) inclou funcions útils com ara l'actualització de signatures de Qrcode col·locades als documents Xltm. Permet canviar les funcions de signatures sense codi addicional.
        
        * Per començar, creeu un objecte Signature passant com a ruta del paràmetre del constructor a un document que se suposa que s'ha d'actualitzar.
        * A continuació, instància un objecte de signatura particular adequat i configureu-ne l'identificador i les propietats que cal canviar.
        * Finalment, truqueu al mètode d'actualització de la signatura passant un objecte de signatura particular.
        * Processa els resultats d'actualització segons el teu avís.

    title_right: "Requisits del sistema"
    content_right: |
        GroupDocs.Signature for .NET són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.

        * Sistemes operatius: Microsoft Windows, Linux, MacOS
        * Entorns de desenvolupament: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Baixeu la darrera versió de GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xltm file
        string filePath = "input.xltm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

                // provide signature features to update
                // set up particular signature id
                QrCodeSignature signatureToUpdate = new QrCodeSignature(id)
                {
                    // specify signature width
                    Width = 200,
                    // specify signature height
                    Height = 200,
                    // set left position
                    Left = 120,
                    // set top position
                    Top = 160
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Actualització de les signatures de Qrcode a les pàgines del document - Demostració en directe"
    content: |
       Editeu diverses signatures electròniques del document Xltm ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Actualitzeu diverses signatures de Qrcode mitjançant C#"
    content: |
        "Edició de signatures digitals que es col·loquen en diferents formats de documents. Actualitza les dades de signatures sense codi addicional."
    format: 
       
       
back_to_top:
    enable: true
---