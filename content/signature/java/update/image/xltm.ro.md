---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Xltm
productName: Java
lang: ro
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Xltm for Java

############################# Head ############################
head_title: "Actualizați Image semnături plasate în fișiere Xltm cu Java"
head_description: "Utilizați codul Java simplu și ușor de înțeles pentru actualizarea semnăturilor Image în documentele Xltm semnate."

############################# Header ############################
title: "Editați și actualizați semnăturile Image plasate în fișierele Xltm"
description: "API-ul pentru Java oferă funcționalități pentru actualizarea semnăturilor Image la documentele Xltm. Actualizați rapid și ușor semnăturile electronice din documentele dvs. Xltm cu câteva rânduri de cod Java."
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
    title: "Aflați despre funcțiile API-ului GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) Funcționalitatea API conține o selecție vastă de mijloace de procesare în formate de documente la cerere prin utilizarea semnăturilor electronice. Este acceptat un spectru larg de semnături electronice, cum ar fi texte, imagini, certificate digitale, coduri de bare, coduri QR, ștampile sau metadate. Clienții pot adăuga, elimina, edita, valida sau căuta semnături digitale în PDF-uri, documente MS Word, registre de lucru MS Excel, prezentări MS PowerPoint, fișiere Adobe Photoshop și diferite formate de imagine. Sunt disponibile numeroase funcții și setări utile.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cum să schimbați semnăturile Image în documentul dvs. Xltm"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) include funcții utile, cum ar fi actualizarea semnăturilor Image plasate în documentele Xltm. Face posibilă schimbarea caracteristicilor semnăturilor fără cod suplimentar.
        
        * Pentru început, creați obiectul Signature care trece ca o cale de parametru constructor către un document care ar trebui să fie actualizat.
        * Apoi, instanțiați un anumit obiect de semnătură adecvat și configurați-i identificatorul și proprietățile care trebuie modificate.
        * În cele din urmă, apelați metoda de actualizare a semnăturii trecând un anumit obiect de semnătură.
        * Procesați rezultatele actualizării după notificarea dvs.

    title_right: "Cerințe de sistem"
    content_right: |
        GroupDocs.Signature for Java sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.

        * Sisteme de operare: Microsoft Windows, Linux, MacOS
        * Medii de dezvoltare: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Descărcați cea mai recentă versiune a GroupDocs.Signature for Java de la [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xltm file
        String filePath = "input.xltm";
        // Set up output file
        String outputFilePath = "output.xltm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to update
        // set up particular signature id
        ImageSignature signatureToUpdate = new ImageSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(170);
        // specify signature height
        signatureToUpdate.setHeight(250);
        // set left position
        signatureToUpdate.setLeft(10);
        // set top position
        signatureToUpdate.setTop(10);

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
    title: "Actualizarea semnăturilor Image de pe paginile documentului - Demo live"
    content: |
       Editați diverse semnături electronice ale documentului Xltm chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Actualizați diferite semnături Image prin Java"
    content: |
        "Editarea semnăturilor digitale care sunt plasate în diferite formate de documente. Actualizați datele despre semnături fără cod suplimentar."
    format: 
       
       
back_to_top:
    enable: true
---