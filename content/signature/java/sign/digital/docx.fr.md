---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Docx
productName: Java
lang: fr
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Docx for Java

############################# Head ############################
head_title: "Ajout de signatures Digital au fichier Docx avec Java"
head_description: "Mettez Digital Signature sur le fichier Docx pour Java en utilisant quelques lignes de code. Utilisez l'API GroupDocs Document Signature pour signer des dizaines de formats de fichiers."

############################# Header ############################
title: "Signez des fichiers Docx avec des signatures Digital en Java"
description: "Comment ajouter Digital Signature avec quelques lignes de code Java"
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
    title_left: "Étapes pour signer Docx avec Digital dans Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) permet de signer rapidement et facilement des documents Docx avec des signatures Digital.
        
        * Créez une instance de la classe Signature fournissant le fichier Docx censé signer en tant que chemin ou flux de mémoire
        * Instanciez la classe SignOptions et définissez toutes les données demandées.
        * Appelez la méthode Signature.Sign() en transmettant le fichier de sortie Docx ou le flux de mémoire

    title_right: "System Requirements"
    content_right: |
        La signature de documents avec GroupDocs.Signature for Java peut être effectuée en quelques étapes simples. Nos API sont prises en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obtenez le dernier GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Docx file
        String filePath = "input.docx";
        // Set up output file
        String outputFilePath = "output.docx";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Docx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signature de documents Docx avec Digital Live Demo"
    content: |
       Signez dès maintenant le fichier Docx avec différentes signatures en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Une démo en ligne gratuite vous attend.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Autres signatures Digital prises en charge pour Java"
    content: |
        "Vous pouvez également signer Docx avec d'autres types de signature. Veuillez consulter la liste ci-dessous."
    format: 
       
       
back_to_top:
    enable: true
---