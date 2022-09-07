---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Qrcode
fileformat: Otp
productName: Java
lang: fr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Otp for Java

############################# Head ############################
head_title: "Mettre à jour les signatures Qrcode placées dans les fichiers Otp avec Java"
head_description: "Utilisez le code Java simple et facile à comprendre pour la mise à jour des signatures Qrcode dans les documents signés Otp."

############################# Header ############################
title: "Modifier et mettre à jour les signatures Qrcode placées dans les fichiers Otp"
description: "L'API pour Java fournit des fonctionnalités pour la mise à jour des signatures Qrcode dans les documents Otp. Mettez à jour les signatures électroniques dans vos documents Otp avec quelques lignes de code Java rapidement et facilement."
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
    title: "En savoir plus sur les fonctionnalités de l'API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) La fonctionnalité de l'API contient une vaste sélection de moyens pour traiter les formats de documents à la demande à l'aide de signatures électroniques. Un large éventail de signatures électroniques telles que des textes, des images, des certificats numériques, des codes-barres, des codes QR, des tampons ou des métadonnées sont pris en charge. Les clients peuvent ajouter, supprimer, modifier, valider ou rechercher des signatures numériques dans des fichiers PDF, des documents MS Word, des classeurs MS Excel, des présentations MS PowerPoint, des fichiers Adobe Photoshop et divers formats d'image. De nombreuses fonctionnalités et paramètres utiles sont disponibles.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Comment changer les signatures Qrcode dans votre document Otp"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) inclut des fonctionnalités utiles telles que la mise à jour des signatures Qrcode placées dans les documents Otp. Il permet de modifier les fonctionnalités des signatures sans code supplémentaire.
        
        * Pour commencer, créez un objet Signature passant comme chemin de paramètre constructeur à un document qui est censé être mis à jour.
        * Ensuite, instanciez un objet de signature particulier approprié et configurez son identifiant et ses propriétés qui doivent être modifiées.
        * Enfin, appelez la méthode Update de Signature en passant un objet de signature particulier.
        * Traiter les résultats de mise à jour à votre avis.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java sont pris en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Téléchargez la dernière version de GroupDocs.Signature for Java depuis [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Otp file
        String filePath = "input.otp";
        // Set up output file
        String outputFilePath = "output.otp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to update
        // set up particular signature id
        QrCodeSignature signatureToUpdate = new QrCodeSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(200);
        // specify signature height
        signatureToUpdate.setHeight(200);
        // set left position
        signatureToUpdate.setLeft(120);
        // set top position
        signatureToUpdate.setTop(160);

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signer avec Qrcode signatures Démo en direct"
    content: |
       Ajoutez dès maintenant diverses signatures électroniques au fichier Otp en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Mettre à jour diverses signatures Qrcode via Java"
    content: |
        "Modification des signatures numériques qui sont placées dans divers formats de documents. Mettez à jour les données des signatures sans code supplémentaire."
    format: 
       
       
back_to_top:
    enable: true
---