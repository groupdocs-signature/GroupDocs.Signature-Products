---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Webp
productName: Java
lang: ro
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Webp for Java

############################# Head ############################
head_title: "Adăugați semnături electronice metadate la documente Webp prin Java"
head_description: "Utilizați metadatele ca semnături electronice ascunse în documentele dvs. Webp folosind câteva rânduri de cod Java. Utilizați API-ul GroupDocs Document Signature pentru a vă semna electronic documentele și fișierele de afaceri cu informații despre metadate."

############################# Header ############################
title: "Semnăturile electronice cu metadate pentru documentul Webp prin Java sunt simple și ușor de utilizat!"
description: "eSemnați documentele și contractele Webp cu intrări de metadate ascunse. Generați metadate pentru PDF-uri, documente MS Word, registre de lucru MS Excel, prezentări MS PowerPoint și diferite formate de imagine fără probleme și codare suplimentară."
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
    title: "Despre GroupDocs.Signature for Java API-ul pentru semnături metadate"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) este un API popular pentru semnarea electronică a documentelor digitale. Sunt disponibile semnături precum texte, imagini, certificate digitale, coduri de bare, coduri QR, ștampile sau metadate. Semnăturile pot fi plasate pe fișiere PDF, documente MS Word, cărți de lucru MS Excel, prezentări MS PowerPoint, fișiere Adobe Photoshop și diferite formate de imagine. Clienții își pot semna documentul și își pot actualiza, căuta, verifica, șterge sau previzualiza semnăturile electronice care au fost puse pe acele documente. În plus, sunt oferite o mulțime de abilități pentru personalizarea semnăturilor.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Pași pentru a semna Webp cu Metadata în Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) oferă posibilitatea de a semna documente Webp cu semnături Metadata rapid și ușor.
        
        * Creați o instanță a clasei Signature care furnizează fișierul Webp care ar trebui să se semneze ca cale sau flux de memorie
        * Instanțiați clasa SignOptions și setați toate datele solicitate.
        * Invocați metoda Signature.Sign() pasând fișierul de ieșire Webp sau fluxul de memorie

    title_right: " Cerințe de sistem"
    content_right: |
        GroupDocs.Signature for Java sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.

        * Sisteme de operare: Microsoft Windows, Linux, MacOS
        * Medii de dezvoltare: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obțineți cel mai recent GroupDocs.Signature for Java de la [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Webp file
        String filePath = "input.webp";
        // Set up output file
        String outputFilePath = "output.webp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Webp document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Semnează documente Webp cu Metadata Live Demo"
    content: |
       Semnați fișierul Webp cu diferite semnături chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuită vă așteaptă.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Alte semnături acceptate de Metadata pentru Java"
    content: |
        "De asemenea, puteți semna Webp cu alte tipuri de semnături. Vă rugăm să vedeți lista de mai jos."
    format: 
       
       
back_to_top:
    enable: true
---