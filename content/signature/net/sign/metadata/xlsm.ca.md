---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Xlsm
productName: .NET
lang: ca
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Xlsm for C#

############################# Head ############################
head_title: "Afegiu signatures electròniques de metadades als documents Xlsm mitjançant C#"
head_description: "Utilitzeu les metadades com a signatures electròniques amagades dins dels vostres documents Xlsm mitjançant un parell de línies de codi C#. Utilitzeu l'API de signatura de documents de GroupDocs per signar electrònicament els vostres documents i fitxers empresarials amb informació de metadades."

############################# Header ############################
title: "Les signatures electròniques de metadades per al document Xlsm mitjançant .NET són senzilles i fàcils d'utilitzar."
description: "eSign els vostres documents i contractes de Xlsm amb entrades de metadades amagades. Genereu metadades per a PDF, documents de MS Word, llibres de treball de MS Excel, presentacions de MS PowerPoint i diversos formats d'imatge sense problemes i codificació addicional."
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
    title: "Sobre l'API de signatures de metadades de GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) és una API popular per a la signatura electrònica de documents digitals. Hi ha signatures com textos, imatges, certificats digitals, codis de barres, codis QR, segells o metadades. Les signatures es poden col·locar en PDF, documents MS Word, llibres de treball de MS Excel, presentacions de MS PowerPoint, fitxers Adobe Photoshop i diversos formats d'imatge. Els clients poden signar el seu document i actualitzar, cercar, verificar, suprimir o previsualitzar les signatures electròniques que es van posar en aquests documents. A més, es proporcionen moltes capacitats per a la personalització de signatures.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Passos per signar Xlsm amb Metadata a C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ofereix la possibilitat de signar documents Xlsm amb signatures Metadata de manera ràpida i senzilla.
        
        * Creeu una instància de la classe Signature que proporcioni el fitxer Xlsm que s'ha de signar com a camí o flux de memòria
        * Instancieu la classe SignOptions i configureu totes les dades sol·licitades.
        * Invoqueu el mètode Signature.Sign() passant el fitxer de sortida Xlsm o el flux de memòria

    title_right: " Requisits del sistema"
    content_right: |
        GroupDocs.Signature for .NET són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.

        * Sistemes operatius: Microsoft Windows, Linux, MacOS
        * Entorns de desenvolupament: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Obteniu l'últim GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Xlsm file
        string filePath = "input.xlsm";
        // Set up output file
        string outputFilePath = "output.xlsm";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Xlsm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signant documents de Xlsm amb Metadata Demostració en directe"
    content: |
       Signa el fitxer Xlsm amb diverses signatures ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demostració gratuïta en línia esperant-te.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altres signatures admeses de Metadata per a C#"
    content: |
        "També podeu signar Xlsm amb altres tipus de signatura. Si us plau, consulteu la llista a continuació."
    format: 
       
       
back_to_top:
    enable: true
---