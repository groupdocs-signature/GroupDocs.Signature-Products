---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Odt
productName: Java
lang: ro
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Odt for Java

############################# Head ############################
head_title: "Ștergeți semnăturile Qrcode din fișierele Odt prin Java"
head_description: "Ștergerea anumitor semnături Qrcode din documentele Odt semnate poate fi efectuată cu ușurință cu ajutorul unui cod scurt Java."

############################# Header ############################
title: "Eliminați semnăturile Qrcode care sunt plasate în fișiere Odt"
description: "Ștergeți diferite semnături Qrcode din documentele Odt. Eliminarea semnăturilor Qrcode necesită un cod simplu Java."
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
    title: "Obțineți informații despre funcțiile API-ului GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API oferă multe modalități de a vă procesa documentele folosind semnături electronice. Sunt disponibile semnături digitale precum texte, imagini, certificate digitale, coduri de bare, coduri QR, ștampile sau metadate. Clienții au posibilitatea de a adăuga, șterge, actualiza, verifica sau căuta semnături digitale în PDF-uri, documente MS Word, registre de lucru MS Excel, prezentări MS PowerPoint, fișiere Adobe Photoshop și diferite formate de imagine. Sunt oferite un număr mare de funcții și setări utile.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cum să eliminați semnăturile Qrcode din documentul dvs. Odt"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) oferă o funcție utilă pentru ștergerea documentelor Odt de semnăturile Qrcode cu câteva linii de cod.
        
        * În primul rând, instanțiază obiectul Signature care trece calea către documentul tău ca parametru de constructor.
        * Apoi, creați un obiect de semnătură adecvat și configurați identificatorul unic al acestuia.
        * {steps.content_left.step_3}
        * {steps.content_left.step_4}

    title_right: "Cerințe de sistem"
    content_right: |
        GroupDocs.Signature for Java sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.

        * Sisteme de operare: Microsoft Windows, Linux, MacOS
        * Medii de dezvoltare: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Descărcați cea mai recentă versiune a GroupDocs.Signature for Java de la [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Odt file
        String filePath = "input.odt";
        // Set up output file
        String outputFilePath = "output.odt";

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
    title: "Semnează cu Qrcode semnături Demo live"
    content: |
       Adăugați diverse semnături electronice în fișierul Odt chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ștergeți-vă semnăturile Qrcode cu Java"
    content: |
        "Ștergerea semnăturilor electronice care au fost adăugate la diferite formate de documente. Eliminați rapid semnăturile fără cod suplimentar."
    format: 
       
       
back_to_top:
    enable: true
---