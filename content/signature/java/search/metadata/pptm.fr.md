---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Pptm
productName: Java
lang: fr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Pptm with Java

############################# Head ############################
head_title: "Rechercher les signatures Metadata dans le fichier Pptm dans Java"
head_description: "Utilisez Java pour rechercher des signatures Metadata dans des fichiers Pptm en utilisant quelques lignes de code."

############################# Header ############################
title: "Rechercher les signatures Metadata dans le fichier Pptm"
description: "L'API native Java permet de rechercher des signatures Metadata dans des fichiers Pptm déjà signés. Effectuez une recherche avancée de signature électronique dans vos documents Pptm en utilisant quelques lignes de code."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "À propos de l'API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) fournit l'API Java pour le traitement de documents à l'aide de divers types de signature tels que des textes, des images, des certificats numériques, des codes-barres, des codes QR, des tampons ou des métadonnées. Les utilisateurs peuvent ajouter, supprimer, mettre à jour, vérifier ou rechercher des signatures électroniques dans des fichiers PDF, des documents MS Word, des classeurs MS Excel, des présentations MS PowerPoint, des fichiers Adobe Photoshop et divers formats d'image, avec une prise en charge supplémentaire pour la personnalisation des propriétés des signatures selon les besoins.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Comment rechercher des signatures Metadata dans Pptm"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) permet aux développeurs de Java de rechercher plus facilement des signatures Metadata dans des fichiers Pptm à partir de leurs applications en mettant en œuvre quelques étapes simples.
        
        * Créez une nouvelle instance de la classe Signature et transmettez le chemin du document source en tant que paramètre du constructeur.
        * Instanciez l'objet SearchOptions selon vos besoins et spécifiez les options de recherche.
        * Appelez la méthode Search de l'instance de classe Signature et transmettez-lui SearchOptions.
        * Traitez les résultats de recherche en fonction de vos demandes.

    title_right: "Configuration requise"
    content_right: |
        GroupDocs.Signature for Java sont pris en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Téléchargez la dernière version de GroupDocs.Signature for Java depuis [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
        
        // Set up input Pptm file
        String filePath = "input.pptm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // search for Metadata signatures in Pptm document
        List<PresentationMetadataSignature> signatures = signature.search(PresentationMetadataSignature.class, SignatureType.Metadata);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));


        ```

############################# Demos ############################
demos:
    enable: true
    title: "Rechercher Metadata signatures électroniques Démo en direct"
    content: |
       Recherchez dès maintenant dans le document diverses signatures électroniques dans des fichiers Pptm en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Rechercher d'autres signatures Metadata à l'aide de Java"
    content: |
        "Recherche de signatures électroniques dans divers documents. Trouvez des signatures à partir de l'un des formats de fichiers populaires, comme indiqué ci-dessous."
    format: 
           
       
back_to_top:
    enable: true
---