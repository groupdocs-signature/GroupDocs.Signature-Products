---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Bmp
productName: .NET
lang: ca
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Bmp for C#

############################# Head ############################
head_title: "Afegint Image signatures al fitxer Bmp amb C#"
head_description: "Poseu la signatura Image al fitxer Bmp per a .NET utilitzant unes quantes línies de codi. Utilitzeu l'API de signatura de documents de GroupDocs per signar desenes de formats de fitxer."

############################# Header ############################
title: "Signa fitxers Bmp amb signatures Image a C#"
description: "Com afegir la signatura Image amb unes poques línies de codi .NET"
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
    title: "Sobre l'API de signatures d'imatge de GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) és una API popular per a la signatura electrònica de documents digitals. Hi ha signatures com textos, imatges, certificats digitals, codis de barres, codis QR, segells o metadades. Les signatures es poden col·locar en PDF, documents MS Word, llibres de treball de MS Excel, presentacions de MS PowerPoint, fitxers Adobe Photoshop i diversos formats d'imatge. Els clients poden signar el seu document i actualitzar, cercar, verificar, suprimir o previsualitzar les signatures electròniques que es van posar en aquests documents. A més, es proporcionen moltes capacitats per a la personalització de signatures.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Passos per signar Bmp amb Image a C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ofereix la possibilitat de signar documents Bmp amb signatures Image de manera ràpida i senzilla.
        
        * Creeu una instància de la classe Signature que proporcioni el fitxer Bmp que s'ha de signar com a camí o flux de memòria
        * Instancieu la classe SignOptions i configureu totes les dades sol·licitades.
        * Invoqueu el mètode Signature.Sign() passant el fitxer de sortida Bmp o el flux de memòria

    title_right: " Requisits del sistema"
    content_right: |
        GroupDocs.Signature for .NET són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.

        * Sistemes operatius: Microsoft Windows, Linux, MacOS
        * Entorns de desenvolupament: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Obteniu l'últim GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Bmp file
        string filePath = "input.bmp";
        // Set up output file
        string outputFilePath = "output.bmp";
        // Provide image file
        string imageFilePath = "image.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
            //Provide sign options
            ImageSignOptions options = new ImageSignOptions(imageFilePath)
            {
                // set signature position
                Left = 50,
                Top = 200
            };

            // sign Bmp document
            SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signant documents de Bmp amb Image Demostració en directe"
    content: |
       Signa el fitxer Bmp amb diverses signatures ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demostració gratuïta en línia esperant-te.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altres signatures admeses de Image per a C#"
    content: |
        "També podeu signar Bmp amb altres tipus de signatura. Si us plau, consulteu la llista a continuació."
    format: 
       
       
back_to_top:
    enable: true
---