---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Doc
productName: Java
lang: fr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Doc for Java

############################# Head ############################
head_title: "Supprimez les signatures Qrcode des fichiers Doc via Java"
head_description: "La suppression de signatures Qrcode spécifiques à partir de documents Doc signés peut être effectuée facilement avec un code Java court."

############################# Header ############################
title: "Supprimer les signatures Qrcode qui sont placées dans les fichiers Doc"
description: "Supprimez diverses signatures Qrcode des documents Doc. La suppression des signatures Qrcode nécessite un code Java simple."
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
    title: "Obtenir des informations sur les fonctionnalités de l'API GroupDocs.Signature for Java"
    content: |
        L'API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) propose de nombreuses façons de traiter vos documents à l'aide de signatures électroniques. Des signatures numériques telles que des textes, des images, des certificats numériques, des codes-barres, des codes QR, des tampons ou des métadonnées sont disponibles. Les clients ont la possibilité d'ajouter, de supprimer, de mettre à jour, de vérifier ou de rechercher des signatures numériques dans des fichiers PDF, des documents MS Word, des classeurs MS Excel, des présentations MS PowerPoint, des fichiers Adobe Photoshop et divers formats d'image. Un grand nombre de fonctionnalités et de paramètres utiles sont fournis.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Comment supprimer les signatures Qrcode de votre document Doc"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) fournit une fonctionnalité utile pour effacer les documents Doc des signatures Qrcode avec quelques lignes de code.
        
        * Tout d'abord, instanciez l'objet Signature passant le chemin d'accès à votre document en tant que paramètre de constructeur.
        * Ensuite, créez un objet de signature approprié et configurez son identifiant unique.
        * Après cela, appelez la méthode Delete en passant l'objet de signature qui doit être supprimé.
        * Enfin, traiter les résultats de l'opération.

    title_right: "Configuration requise"
    content_right: |
        GroupDocs.Signature for Java sont pris en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.

        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Téléchargez la dernière version de GroupDocs.Signature for Java depuis [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Doc file
        String filePath = "input.doc";
        // Set up output file
        String outputFilePath = "output.doc";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to delete
        QrCodeSignature signatureToDelete = new QrCodeSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signer avec Qrcode signatures Démo en direct"
    content: |
       Ajoutez dès maintenant diverses signatures électroniques au fichier Doc en visitant le site Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Supprimez vos signatures Qrcode avec Java"
    content: |
        "Suppression des signatures électroniques qui ont été ajoutées à divers formats de documents. Supprimez les signatures rapidement sans code supplémentaire."
    format: 
       
       
back_to_top:
    enable: true
---