---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Xls
productName: Java
lang: ro
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xls for Java

############################# Head ############################
head_title: "Adăugarea semnăturilor electronice digitale la fișierul Xls cu Java"
head_description: "Puneți semnătura digitală pe fișierul Xls pentru Java folosind câteva rânduri de cod. Utilizați API-ul GroupDocs Document Signature pentru a semna zeci de formate de fișiere."

############################# Header ############################
title: "eSign fișiere Xls cu semnături Digital în Java"
description: "Cum să adăugați semnătura Digital cu câteva rânduri de cod Java"
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
    title: "Despre GroupDocs.Signature for Java API-ul pentru semnături digitale"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) este un API popular pentru a semna documente cu semnături electronice digitale, cu certificate digitale. Pentru semnăturile digitale, API-ul utilizează fișiere de certificat PFX pentru a emite documentul cu chei publice și private protejate cu parolă. Semnăturile digitale pot fi folosite pentru a certifica documente de afaceri cu o anumită pagină eSign PDF, pentru a certifica documente întregi Microsoft Office, cum ar fi Words, Excel, fișiere Powerpoint și documente Open Office. Clienții pot manipula cu ușurință semnăturile, cum ar fi editarea, eliminarea sau ajustarea acestora. API-ul oferă o modalitate de a căuta și verifica semnăturile. În plus, sunt oferite o mulțime de abilități pentru personalizarea semnăturilor.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Pași pentru a semna Xls cu Digital în Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) oferă posibilitatea de a semna documente Xls cu semnături Digital rapid și ușor.
        
        * Creați o instanță a clasei Signature care furnizează fișierul Xls care ar trebui să se semneze ca cale sau flux de memorie
        * Instanțiați clasa SignOptions și setați toate datele solicitate.
        * Invocați metoda Signature.Sign() pasând fișierul de ieșire Xls sau fluxul de memorie

    title_right: " Cerințe de sistem"
    content_right: |
        GroupDocs.Signature for Java sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.

        * Sisteme de operare: Microsoft Windows, Linux, MacOS
        * Medii de dezvoltare: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obțineți cel mai recent GroupDocs.Signature for Java de la [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xls file
        String filePath = "input.xls";
        // Set up output file
        String outputFilePath = "output.xls";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Xls document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Semnează documente Xls cu Digital Live Demo"
    content: |
       Semnați fișierul Xls cu diferite semnături chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuită vă așteaptă.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Alte semnături acceptate de Digital pentru Java"
    content: |
        "De asemenea, puteți semna Xls cu alte tipuri de semnături. Vă rugăm să vedeți lista de mai jos."
    format: 
       
       
back_to_top:
    enable: true
---