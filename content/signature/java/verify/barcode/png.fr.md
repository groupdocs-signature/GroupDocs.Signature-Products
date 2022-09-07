---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Barcode
fileformat: Png
productName: Java
lang: fr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Barcode signature on Png for Java

############################# Head ############################
head_title: "Vérification des signatures Barcode pour les fichiers Png via Java"
head_description: "Utilisez seulement quelques lignes de code Java pour vérifier les documents Png et leurs signatures Barcode."

############################# Header ############################
title: "Vérification des signatures Barcode pour les fichiers Png"
description: "L'API pour Java offre la possibilité de vérifier les signatures Barcode sur les documents Png. La vérification des signatures électroniques dans vos documents Png peut être effectuée rapidement et facilement."
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
    title: "Découvrez les nouvelles fonctionnalités de l'API GroupDocs.Signature for Java"
    content: |
        L'API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) offre un large éventail de façons de traiter de nombreux formats de documents à l'aide de signatures électroniques. De nombreux types de signatures numériques tels que textes, images, certificats numériques, codes-barres, codes QR, tampons ou métadonnées sont pris en charge. Les clients peuvent ajouter, supprimer, modifier, valider ou rechercher des signatures numériques dans des fichiers PDF, des documents MS Word, des classeurs MS Excel, des présentations MS PowerPoint, des fichiers Adobe Photoshop et divers formats d'image. Un nombre étonnant de fonctionnalités et de paramètres supplémentaires sont disponibles.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Comment valider les signatures Barcode dans votre document Png"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) inclut des fonctionnalités utiles telles que la vérification des signatures Barcode placées sur les documents Png. Utilisez cette opportunité sans implémenter de code supplémentaire.
        
        * Tout d'abord, instanciez la classe Signature en fournissant comme paramètre de constructeur le chemin d'accès à un document censé être vérifié.
        * Deuxièmement, créez un nouvel objet VerifyOptions et configurez toutes les propriétés requises.
        * Enfin, appelez la méthode Verify de l'objet Signature en passant l'instance VerifyOptions.
        * Traiter ensuite les résultats de la vérification.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java sont pris en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Téléchargez la dernière version de GroupDocs.Signature for Java depuis [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Png file
        String filePath = "input.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        BarcodeVerifyOptions options = new BarcodeVerifyOptions();

        // process only specified page 
        options.setPageNumber(2);
        options.setAllPages(false);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Special signature");
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signer avec Barcode signatures Démo en direct"
    content: |
       Ajoutez dès maintenant diverses signatures électroniques au fichier Png en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Vérifiez les autres signatures Barcode à l'aide de Java"
    content: |
        "Vérification des signatures électroniques apposées dans divers documents. Vérifiez la qualité des signatures dans les formats de fichiers populaires comme indiqué ci-dessous."
    format: 
       
       
back_to_top:
    enable: true
---