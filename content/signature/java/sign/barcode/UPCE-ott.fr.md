---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: UPCE
fileformat: Ott
productName: Java
lang: fr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Ott for Java

############################# Head ############################
head_title: "eSign Ott document avec UPCE Barcode in Java"
head_description: "Créez UPCE Barcode Signature et placez-le sur le document Ott avec Java en utilisant quelques lignes de code. Utilisez l'API GroupDocs Document Signature pour signer divers formats de fichiers."

############################# Header ############################
title: "Générer la signature de code-barres UPCE pour le document Ott dans Java"
description: "Signez électroniquement vos documents commerciaux Ott avec UPCE Barcode. Générez une signature de code-barres rapidement et facilement avec quelques lignes de code pour configurer les options de signature."
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
    title: "À propos de l'API de signatures de code-barres GroupDocs.Signature for Java."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) est une API simple et rapide pour gérer la signature électronique de documents numériques à l'aide de types de codes-barres tels que UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 et bien d'autres. Les clients peuvent créer facilement des codes-barres fournissant le texte requis et les placer sur des fichiers PDF, des documents Microsoft Office Words, des classeurs Microsoft Office Excel, des présentations MS PowerPoint, des fichiers Adobe Photoshop et divers formats d'image. Les codes-barres placés dans les documents peuvent être mis à jour, recherchés, vérifiés, supprimés ou prévisualisés. De plus, la personnalisation des codes-barres est prise en charge.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Étapes pour signer Ott avec Barcode dans Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) permet de signer rapidement et facilement des documents Ott avec des signatures Barcode.
        
        * Créez une instance de la classe Signature fournissant le fichier Ott censé signer en tant que chemin ou flux de mémoire
        * Instanciez la classe SignOptions et définissez toutes les données demandées.
        * Appelez la méthode Signature.Sign() en transmettant le fichier de sortie Ott ou le flux de mémoire

    title_right: " Configuration requise"
    content_right: |
        GroupDocs.Signature for Java sont pris en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obtenez le dernier GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ott file
        String filePath = "input.ott";
        // Set up output file
        String outputFilePath = "output.ott";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.UPCE);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Ott document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signature de documents Ott avec Barcode Live Demo"
    content: |
       Signez dès maintenant le fichier Ott avec différentes signatures en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Une démo en ligne gratuite vous attend.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About UPCE Barcode"
          content: |
            Le code produit universel est une symbologie de code-barres largement utilisée dans le monde entier pour suivre les articles commerciaux dans les magasins. UPCE est une variation à 8 chiffres si UPC.
          characterset: |
             Prend en charge uniquement les chiffres numériques (0-9).
          textcapacity: |
             Capacité du texte codé : exactement 7 chiffres + 1 chiffre de contrôle.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAEAAAABjCAYAAAArUQZGAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAUTSURBVHhe7ZBBqmQBCAP7/pfuMUwXyMcIkuV7BRK1wIWf78N5H/DLx/I+4JeP5X3ALx/L+oDP57/+m0I9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE548xDeB/zysbwP+OVjefgDvt9/E/iHbcwlZ5QAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Autres signatures Barcode prises en charge pour Java"
    content: |
        "Vous pouvez également signer Ott avec d'autres types de signature. Veuillez consulter la liste ci-dessous."
    format: 
        
       
back_to_top:
    enable: true
---