---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Pps
productName: Java
lang: ro
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Pps for Java

############################# Head ############################
head_title: "eSign Pps document cu Pharmacode cod de bare în Java"
head_description: "Creați semnătura codului de bare Pharmacode și puneți-o pe documentul Pps cu Java folosind câteva rânduri de cod. Utilizați API-ul GroupDocs Document Signature pentru a semna diferite formate de fișiere."

############################# Header ############################
title: "Generați semnătura de cod de bare Pharmacode pentru documentul Pps în Java"
description: "eSemnați documentele dvs. comerciale Pps cu codul de bare Pharmacode. Generați semnătura cod de bare rapid și ușor cu câteva linii de cod pentru a configura opțiunile de semnare."
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
    title: "Despre GroupDocs.Signature for Java API-ul pentru semnături coduri de bare."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) este un API rapid și ușor pentru a gestiona semnarea electronică a documentelor digitale folosind tipuri de coduri de bare precum UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 și multe altele. Clienții pot crea cu ușurință coduri de bare care oferă textul necesar și le pot pune pe PDF, documente Microsoft Office Words, cărți de lucru Microsoft Office Excel, prezentări MS PowerPoint, fișiere Adobe Photoshop și diferite formate de imagine. Codurile de bare plasate în documente pot fi actualizate, căutate, verificate, șterse sau previzualizate. În plus, personalizarea codurilor de bare este acceptată.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Pași pentru a semna Pps cu Barcode în Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) oferă posibilitatea de a semna documente Pps cu semnături Barcode rapid și ușor.
        
        * Creați o instanță a clasei Signature care furnizează fișierul Pps care ar trebui să se semneze ca cale sau flux de memorie
        * Instanțiați clasa SignOptions și setați toate datele solicitate.
        * Invocați metoda Signature.Sign() pasând fișierul de ieșire Pps sau fluxul de memorie

    title_right: " Cerințe de sistem"
    content_right: |
        GroupDocs.Signature for Java sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.

        * Sisteme de operare: Microsoft Windows, Linux, MacOS
        * Medii de dezvoltare: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obțineți cel mai recent GroupDocs.Signature for Java de la [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pps file
        String filePath = "input.pps";
        // Set up output file
        String outputFilePath = "output.pps";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Pharmacode);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Pps document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Semnează documente Pps cu Barcode Live Demo"
    content: |
       Semnați fișierul Pps cu diferite semnături chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuită vă așteaptă.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            Pharmacode, cunoscut și sub numele de Pharmaceutical Binary Code, este un standard de coduri de bare, utilizat în industria farmaceutică ca sistem de control al ambalajului.
          characterset: |
             Cifre numerice (0-9).
          textcapacity: |
             Reprezintă un singur număr întreg de la 3 la 131070.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Alte semnături acceptate de Barcode pentru Java"
    content: |
        "De asemenea, puteți semna Pps cu alte tipuri de semnături. Vă rugăm să vedeți lista de mai jos."
    format: 
        
       
back_to_top:
    enable: true
---