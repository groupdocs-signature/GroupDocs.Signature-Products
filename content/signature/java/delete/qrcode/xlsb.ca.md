---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Xlsb
productName: Java
lang: ca
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Xlsb for Java

############################# Head ############################
head_title: "Suprimeix les signatures de Qrcode dels fitxers Xlsb mitjançant Java"
head_description: "L'eliminació de signatures específiques de Qrcode dels documents signats Xlsb es pot dur a terme fàcilment amb un codi Java curt."

############################# Header ############################
title: "Elimineu les signatures de Qrcode que es col·loquen als fitxers Xlsb"
description: "Suprimeix diverses signatures de Qrcode dels documents Xlsb. L'eliminació de signatures Qrcode requereix un codi Java senzill."
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
    title: "Obteniu informació sobre les funcions de l'API de GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API ofereix moltes maneres de processar els vostres documents mitjançant signatures electròniques. Hi ha signatures digitals com textos, imatges, certificats digitals, codis de barres, codis QR, segells o metadades. Els clients tenen la possibilitat d'afegir, esborrar, actualitzar, verificar o cercar signatures digitals en PDF, documents MS Word, llibres de treball MS Excel, presentacions MS PowerPoint, fitxers Adobe Photoshop i diversos formats d'imatge. S'ofereixen un gran nombre de funcions i configuracions útils.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Com eliminar les signatures de Qrcode del vostre document Xlsb"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ofereix una funció útil per esborrar documents de Xlsb de signatures de Qrcode amb unes poques línies de codi.
        
        * En primer lloc, instanciïu l'objecte Signature passant el camí al vostre document com a paràmetre de constructor.
        * A continuació, creeu un objecte de signatura adequat i configureu el seu identificador únic.
        * Després d'això, invoqueu el mètode Delete passant l'objecte de signatura que s'ha d'eliminar.
        * Finalment, els resultats de l'operació del procés.

    title_right: "Requisits del sistema"
    content_right: |
        GroupDocs.Signature for Java són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.

        * Sistemes operatius: Microsoft Windows, Linux, MacOS
        * Entorns de desenvolupament: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Baixeu la darrera versió de GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsb file
        String filePath = "input.xlsb";
        // Set up output file
        String outputFilePath = "output.xlsb";

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
    title: "Signant amb Qrcode signatures Demostració en directe"
    content: |
       Afegiu diverses signatures electròniques al fitxer Xlsb ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Suprimeix les teves signatures de Qrcode amb Java"
    content: |
        "Supressió de signatures electròniques que s'han afegit a diversos formats de documents. Elimina les signatures ràpidament sense codi addicional."
    format: 
       
       
back_to_top:
    enable: true
---