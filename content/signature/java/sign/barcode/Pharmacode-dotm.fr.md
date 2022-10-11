---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Dotm
productName: Java
lang: fr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Dotm for Java

############################# Head ############################
head_title: "eSign Dotm document avec Pharmacode Barcode in Java"
head_description: "Créez Pharmacode Barcode Signature et placez-le sur le document Dotm avec Java en utilisant quelques lignes de code. Utilisez l'API GroupDocs Document Signature pour signer divers formats de fichiers."

############################# Header ############################
title: "Générer la signature de code-barres Pharmacode pour le document Dotm dans Java"
description: "Signez électroniquement vos documents commerciaux Dotm avec Pharmacode Barcode. Générez une signature de code-barres rapidement et facilement avec quelques lignes de code pour configurer les options de signature."
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
    title_left: "Étapes pour signer Dotm avec Barcode dans Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) permet de signer rapidement et facilement des documents Dotm avec des signatures Barcode.
        
        * Créez une instance de la classe Signature fournissant le fichier Dotm censé signer en tant que chemin ou flux de mémoire
        * Instanciez la classe SignOptions et définissez toutes les données demandées.
        * Appelez la méthode Signature.Sign() en transmettant le fichier de sortie Dotm ou le flux de mémoire

    title_right: " Configuration requise"
    content_right: |
        GroupDocs.Signature for Java sont pris en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obtenez le dernier GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dotm file
        String filePath = "input.dotm";
        // Set up output file
        String outputFilePath = "output.dotm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Pharmacode);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Dotm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signature de documents Dotm avec Barcode Live Demo"
    content: |
       Signez dès maintenant le fichier Dotm avec différentes signatures en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Une démo en ligne gratuite vous attend.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            Pharmacode, également connu sous le nom de Pharmaceutical Binary Code, est une norme de code à barres, utilisée dans l'industrie pharmaceutique comme système de contrôle d'emballage.
          characterset: |
             Chiffres numériques (0-9).
          textcapacity: |
             Représente un seul entier compris entre 3 et 131070.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Autres signatures Barcode prises en charge pour Java"
    content: |
        "Vous pouvez également signer Dotm avec d'autres types de signature. Veuillez consulter la liste ci-dessous."
    format: 
        
       
back_to_top:
    enable: true
---