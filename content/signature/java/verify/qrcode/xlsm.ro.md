---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Xlsm
productName: Java
lang: ro
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Xlsm for Java

############################# Head ############################
head_title: "Verificarea semnăturilor Qrcode pentru fișierele Xlsm prin Java"
head_description: "Utilizați doar câteva rânduri de cod Java pentru a verifica documentele Xlsm și semnăturile acestora Qrcode."

############################# Header ############################
title: "Qrcode verificarea semnăturilor pentru fișiere Xlsm"
description: "API-ul pentru Java oferă posibilitatea de a verifica semnăturile Qrcode în documentele Xlsm. Verificarea semnăturilor electronice din documentele dvs. Xlsm poate fi efectuată rapid și ușor."
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
    title: "Descoperiți noi funcții API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API oferă o gamă largă de moduri de a procesa numeroase formate de documente prin utilizarea semnăturilor electronice. Sunt acceptate multe tipuri de semnături digitale precum texte, imagini, certificate digitale, coduri de bare, coduri QR, ștampile sau metadate. Clienții pot adăuga, elimina, edita, valida sau căuta semnături digitale în PDF-uri, documente MS Word, registre de lucru MS Excel, prezentări MS PowerPoint, fișiere Adobe Photoshop și diferite formate de imagine. Sunt disponibile un număr uimitor de funcții și setări suplimentare.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cum să validați semnăturile Qrcode în documentul dvs. Xlsm"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) include funcții utile, cum ar fi verificarea semnăturilor Qrcode plasate în documentele Xlsm. Folosiți această oportunitate fără a implementa cod suplimentar.
        
        * În primul rând, instanțiați clasa Signature furnizând ca parametru constructor calea către un document care ar trebui să fie verificat.
        * În al doilea rând, creați un nou obiect VerifyOptions și configurați toate proprietățile necesare.
        * În cele din urmă, invocați metoda Verify a obiectului Signature, trecând instanța VerifyOptions.
        * Apoi procesați rezultatele verificării.

    title_right: "Cerințe de sistem"
    content_right: |
        GroupDocs.Signature for Java sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.

        * Sisteme de operare: Microsoft Windows, Linux, MacOS
        * Medii de dezvoltare: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Descărcați cea mai recentă versiune a GroupDocs.Signature for Java de la [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsm file
        String filePath = "input.xlsm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        QrCodeVerifyOptions options = new QrCodeVerifyOptions();

        // process only first page
        options.setPagesSetup(new PagesSetup());
        options.setPageNumber(1);
        options.setAllPages(false);
        // specify text match type
        options.setMatchType(TextMatchType.StartsWith);
        // specify text pattern to search
        options.setText("QrCode text");
                            
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
    title: "Semnează cu Qrcode semnături Demo live"
    content: |
       Adăugați diverse semnături electronice în fișierul Xlsm chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verificați alte semnături Qrcode folosind Java"
    content: |
        "Verificarea semnăturilor electronice plasate în diverse documente. Verificați calitatea semnăturilor în formatele de fișiere populare, așa cum este dezvăluit mai jos."
    format: 
       
       
back_to_top:
    enable: true
---