---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Gif
productName: .NET
lang: fr
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Gif for C#

############################# Head ############################
head_title: "Ajouter des signatures électroniques de métadonnées aux documents Gif via C#"
head_description: "Utilisez les métadonnées comme signatures électroniques cachées dans vos documents Gif en utilisant quelques lignes de code C#. Utilisez l'API GroupDocs Document Signature pour signer électroniquement vos documents et fichiers commerciaux avec des informations de métadonnées."

############################# Header ############################
title: "Les signatures électroniques de métadonnées pour le document Gif via .NET sont simples et faciles à utiliser !"
description: "Signez électroniquement vos documents et contrats Gif avec des entrées de métadonnées masquées. Générez des métadonnées pour les fichiers PDF, les documents MS Word, les classeurs MS Excel, les présentations MS PowerPoint et divers formats d'image sans problème et avec un codage supplémentaire."
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
    title: "{metadata-about.title}"
    content: |
        {metadata-about.content}
    

############################# Steps ############################
steps:
    enable: true
    title_left: "{metadata-steps.title}"
    content_left: |
        {metadata-steps.content.description}
        
        * {metadata-steps.content.step_1}
        * {metadata-steps.content.step_2}
        * {metadata-steps.content.step_3}

    title_right: " {system-requirements.title}"
    content_right: |
        {system-requirements.content.description}

        * {system-requirements.content.step_1}
        * {system-requirements.content.step_2}
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * {system-requirements.content.step_3}
         
    code: |
        ```csharp    
        
        // Set up input Gif file
        string filePath = "input.gif";
        // Set up output file
        string outputFilePath = "output.gif";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                MetadataSignOptions options = new MetadataSignOptions();

                // Specify different Metadata Signatures and add them to options signature collection
                // set start id
                ushort imgsMetadataId = 41996;
                // setup int value
                ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
                options.Signatures.Add(mdSign_DocId);
                // setup Author property
                ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
                options.Signatures.Add(mdSign_Author);
                // setup data of sign date
                ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, DateTime.Now); // DateTime
                options.Signatures.Add(mdSign_Date);
                // setup double
                ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456M); //decimal value
                options.Signatures.Add(mdSign_Amnt);

                // sign Gif document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signature de documents Gif avec Metadata Live Demo"
    content: |
       Signez dès maintenant le fichier Gif avec différentes signatures en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Une démo en ligne gratuite vous attend.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Autres signatures Metadata prises en charge pour C#"
    content: |
        "Vous pouvez également signer Gif avec d'autres types de signature. Veuillez consulter la liste ci-dessous."
    format: 
       
       
back_to_top:
    enable: true
---