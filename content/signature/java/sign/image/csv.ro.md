---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Csv
productName: Java
lang: ro
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Csv for Java

############################# Head ############################
head_title: "Adăugarea de semnături Image la fișierul Csv cu Java"
head_description: "Puneți Image Semnătura pe fișierul Csv pentru Java folosind câteva rânduri de cod. Utilizați API-ul GroupDocs Document Signature pentru a semna zeci de formate de fișiere."

############################# Header ############################
title: "Semnează fișiere Csv cu semnături Image în Java"
description: "Cum să adăugați semnătura Image cu câteva rânduri de cod Java"
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
    title: "Despre GroupDocs.Signature for Java API-ul pentru semnături imagine"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) este un API popular pentru semnarea electronică a documentelor digitale. Sunt disponibile semnături precum texte, imagini, certificate digitale, coduri de bare, coduri QR, ștampile sau metadate. Semnăturile pot fi plasate pe fișiere PDF, documente MS Word, cărți de lucru MS Excel, prezentări MS PowerPoint, fișiere Adobe Photoshop și diferite formate de imagine. Clienții își pot semna documentul și își pot actualiza, căuta, verifica, șterge sau previzualiza semnăturile electronice care au fost puse pe acele documente. În plus, sunt oferite o mulțime de abilități pentru personalizarea semnăturilor.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Pași pentru a semna Csv cu Image în Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) oferă posibilitatea de a semna documente Csv cu semnături Image rapid și ușor.
        
        * Creați o instanță a clasei Signature care furnizează fișierul Csv care ar trebui să se semneze ca cale sau flux de memorie
        * Instanțiați clasa SignOptions și setați toate datele solicitate.
        * Invocați metoda Signature.Sign() pasând fișierul de ieșire Csv sau fluxul de memorie

    title_right: " Cerințe de sistem"
    content_right: |
        GroupDocs.Signature for Java sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.

        * Sisteme de operare: Microsoft Windows, Linux, MacOS
        * Medii de dezvoltare: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obțineți cel mai recent GroupDocs.Signature for Java de la [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Csv file
        String filePath = "input.csv";
        // Set up output file
        String outputFilePath = "output.csv";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Csv document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Semnează documente Csv cu Image Live Demo"
    content: |
       Semnați fișierul Csv cu diferite semnături chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuită vă așteaptă.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Alte semnături acceptate de Image pentru Java"
    content: |
        "De asemenea, puteți semna Csv cu alte tipuri de semnături. Vă rugăm să vedeți lista de mai jos."
    format: 
       
       
back_to_top:
    enable: true
---