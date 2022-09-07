---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Docx
productName: Java
lang: fr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Docx for Java

############################# Head ############################
head_title: "Ajouter des signatures électroniques de métadonnées aux documents Docx via Java"
head_description: "Utilisez les métadonnées comme signatures électroniques cachées dans vos documents Docx en utilisant quelques lignes de code Java. Utilisez l'API GroupDocs Document Signature pour signer électroniquement vos documents et fichiers commerciaux avec des informations de métadonnées."

############################# Header ############################
title: "Les signatures électroniques de métadonnées pour le document Docx via Java sont simples et faciles à utiliser !"
description: "Signez électroniquement vos documents et contrats Docx avec des entrées de métadonnées masquées. Générez des métadonnées pour les fichiers PDF, les documents MS Word, les classeurs MS Excel, les présentations MS PowerPoint et divers formats d'image sans problème et avec un codage supplémentaire."
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
    title_left: "Étapes pour signer Docx avec Metadata dans Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) permet de signer rapidement et facilement des documents Docx avec des signatures Metadata.
        
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

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        WordProcessingMetadataSignature mdSign_Author = new WordProcessingMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        WordProcessingMetadataSignature mdSign_DocData = new WordProcessingMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        WordProcessingMetadataSignature mdSign_DocId = new WordProcessingMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Docx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signature de documents Docx avec Metadata Live Demo"
    content: |
       Signez dès maintenant le fichier Docx avec différentes signatures en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Une démo en ligne gratuite vous attend.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Autres signatures Metadata prises en charge pour Java"
    content: |
        "Vous pouvez également signer Docx avec d'autres types de signature. Veuillez consulter la liste ci-dessous."
    format: 
       
       
back_to_top:
    enable: true
---