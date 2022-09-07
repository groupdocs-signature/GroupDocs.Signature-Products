---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Pptx
productName: .NET
lang: fr
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Pptx for C#

############################# Head ############################
head_title: "eSign Pptx document avec Codabar Barcode in C#"
head_description: "Créez Codabar Barcode Signature et placez-le sur le document Pptx avec .NET en utilisant quelques lignes de code. Utilisez l'API GroupDocs Document Signature pour signer divers formats de fichiers."

############################# Header ############################
title: "Générer la signature de code-barres Codabar pour le document Pptx dans C#"
description: "Signez électroniquement vos documents commerciaux Pptx avec Codabar Barcode. Générez une signature de code-barres rapidement et facilement avec quelques lignes de code pour configurer les options de signature."
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
    title: "À propos de l'API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) est une API populaire pour la signature électronique de documents numériques utilisant de nombreux types de codes-barres tels que UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN, ITF14 et plein d'autres. Les clients peuvent créer facilement des codes-barres fournissant uniquement le texte demandé et les placer sur des fichiers PDF, des documents MS Word, des classeurs MS Excel, des présentations MS PowerPoint, des fichiers Adobe Photoshop et divers formats d'image. Les codes-barres placés dans les documents peuvent être mis à jour, recherchés, vérifiés, supprimés ou prévisualisés. De plus, la personnalisation des codes-barres est prise en charge.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Étapes pour signer Pptx avec Barcode dans C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) permet de signer rapidement et facilement des documents Pptx avec des signatures Barcode.
        
        * Créez une instance de la classe Signature fournissant le fichier Pptx censé signer en tant que chemin ou flux de mémoire
        * Instanciez la classe SignOptions et définissez toutes les données demandées.
        * Appelez la méthode Signature.Sign() en transmettant le fichier de sortie Pptx ou le flux de mémoire

    title_right: "System Requirements"
    content_right: |
        La signature de documents avec GroupDocs.Signature for .NET peut être effectuée en quelques étapes simples. Nos API sont prises en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Obtenez le dernier GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Pptx file
        string filePath = "input.pptx";
        // Set up output file
        string outputFilePath = "output.pptx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Codabar,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Pptx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signature de documents Pptx avec Barcode Live Demo"
    content: |
       Signez dès maintenant le fichier Pptx avec différentes signatures en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Une démo en ligne gratuite vous attend.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar est une symbologie de code-barres linéaire qui a été conçue pour être lue avec précision même lorsqu'elle est imprimée sur des imprimantes matricielles pour les formulaires en plusieurs parties tels que les factures aériennes FedEx et les formulaires de banque de sang.
          characterset: |
             Chiffres numériques (0-9) et caractères spéciaux $/- :+.
          textcapacity: |
             Aucune restriction spécifique.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Autres signatures Barcode prises en charge pour C#"
    content: |
        "Vous pouvez également signer Pptx avec d'autres types de signature. Veuillez consulter la liste ci-dessous."
    format: 
           
       
back_to_top:
    enable: true
---