---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Xls
productName: Java
lang: ca
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xls for Java

############################# Head ############################
head_title: "Suprimeix les signatures de Digital dels fitxers Xls mitjançant Java"
head_description: "L'eliminació de signatures específiques de Digital dels documents signats Xls es pot dur a terme fàcilment amb un codi Java curt."

############################# Header ############################
title: "Elimineu les signatures de Digital que es col·loquen als fitxers Xls"
description: "Suprimeix diverses signatures de Digital dels documents Xls. L'eliminació de signatures Digital requereix un codi Java senzill."
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
    title_left: "Com eliminar les signatures de Digital del vostre document Xls"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ofereix una funció útil per esborrar documents de Xls de signatures de Digital amb unes poques línies de codi.
        
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
                
        // Set up input Xls file
        String filePath = "input.xls";
        // Set up output file
        String outputFilePath = "output.xls";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "a01e1940-997a-444b-89af-9309a2d559a5";

        // provide signature item to delete
        DigitalSignature signatureToDelete = new DigitalSignature(id);

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
    title: "Signant amb Digital signatures Demostració en directe"
    content: |
       Afegiu diverses signatures electròniques al fitxer Xls ara mateix visitant el lloc web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Suprimeix les teves signatures de Digital amb Java"
    content: |
        "Supressió de signatures electròniques que s'han afegit a diversos formats de documents. Elimina les signatures ràpidament sense codi addicional."
    format: 
       
       
back_to_top:
    enable: true
---