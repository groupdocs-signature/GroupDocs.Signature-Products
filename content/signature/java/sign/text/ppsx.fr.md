---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Ppsx
productName: Java
lang: fr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Ppsx for Java

############################# Head ############################
head_title: "Ajout de signatures Text au fichier Ppsx avec Java"
head_description: "Mettez Text Signature sur le fichier Ppsx pour Java en utilisant quelques lignes de code. Utilisez l'API GroupDocs Document Signature pour signer des dizaines de formats de fichiers."

############################# Header ############################
title: "Signez des fichiers Ppsx avec des signatures Text en Java"
description: "Comment ajouter Text Signature avec quelques lignes de code Java"
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
    title: "À propos de l'API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) est une API populaire pour la signature électronique de documents numériques. Des signatures telles que des textes, des images, des certificats numériques, des codes-barres, des codes QR, des tampons ou des métadonnées sont disponibles. Les signatures peuvent être placées sur des fichiers PDF, des documents MS Word, des classeurs MS Excel, des présentations MS PowerPoint, des fichiers Adobe Photoshop et divers formats d'image. Les clients peuvent signer leur document et mettre à jour, rechercher, vérifier, supprimer ou prévisualiser les signatures électroniques apposées sur ces documents. De plus, de nombreuses capacités de personnalisation des signatures sont fournies.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Étapes pour signer Ppsx avec Text dans Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) permet de signer rapidement et facilement des documents Ppsx avec des signatures Text.
        
        * Créez une instance de la classe Signature fournissant le fichier Ppsx censé signer en tant que chemin ou flux de mémoire
        * Instanciez la classe SignOptions et définissez toutes les données demandées.
        * Appelez la méthode Signature.Sign() en transmettant le fichier de sortie Ppsx ou le flux de mémoire

    title_right: "System Requirements"
    content_right: |
        La signature de documents avec GroupDocs.Signature for Java peut être effectuée en quelques étapes simples. Nos API sont prises en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obtenez le dernier GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ppsx file
        String filePath = "input.ppsx";
        // Set up output file
        String outputFilePath = "output.ppsx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Ppsx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signature de documents Ppsx avec Text Live Demo"
    content: |
       Signez dès maintenant le fichier Ppsx avec différentes signatures en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Une démo en ligne gratuite vous attend.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Autres signatures Text prises en charge pour Java"
    content: |
        "Vous pouvez également signer Ppsx avec d'autres types de signature. Veuillez consulter la liste ci-dessous."
    format: 
       
       
back_to_top:
    enable: true
---