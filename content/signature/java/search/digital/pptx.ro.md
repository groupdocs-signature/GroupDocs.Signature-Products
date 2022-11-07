---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Pptx
productName: Java
lang: ro
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Pptx with Java

############################# Head ############################
head_title: "Căutați semnături Digital în fișierul Pptx în Java"
head_description: "Utilizați Java pentru a căuta semnături Digital în fișiere Pptx folosind câteva rânduri de cod."

############################# Header ############################
title: "Căutați semnături Digital în fișierul Pptx"
description: "API-ul nativ Java permite căutarea semnăturilor Digital în fișierele Pptx deja semnate. Efectuați o căutare avansată de semnătură electronică în documentele dvs. Pptx folosind câteva rânduri de cod."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Despre GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) oferă Java API pentru procesarea documentelor folosind diferite tipuri de semnături, cum ar fi texte, imagini, certificate digitale, coduri de bare, coduri QR, ștampile sau metadate. Utilizatorii pot adăuga, șterge, actualiza, verifica sau căuta semnături electronice în PDF-uri, documente MS Word, registre de lucru MS Excel, prezentări MS PowerPoint, fișiere Adobe Photoshop și diferite formate de imagine, cu suport suplimentar pentru personalizarea proprietăților semnăturilor după cum este necesar.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cum să căutați semnături Digital în Pptx"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) facilitează pentru dezvoltatorii Java să caute semnături Digital în fișierele Pptx din aplicațiile lor prin implementarea câțiva pași simpli.
        
        * Creați o nouă instanță a clasei Signature și treceți calea documentului sursă ca parametru de constructor.
        * Instanciați obiectul SearchOptions în funcție de cerințele dvs. și specificați opțiunile de căutare.
        * Apelați metoda Search a instanței clasei Signature și transmiteți-i SearchOptions.
        * Procesați rezultatele căutării în funcție de cerințele dvs.

    title_right: "Cerințe de sistem"
    content_right: |
        GroupDocs.Signature for Java sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.

        * Sisteme de operare: Microsoft Windows, Linux, MacOS
        * Medii de dezvoltare: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Descărcați cea mai recentă versiune a GroupDocs.Signature for Java de la [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pptx file
        String filePath = "input.pptx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        DigitalSearchOptions options = new DigitalSearchOptions();

        // specify special search criteria
        options.setComments("Approved");
        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2021, 3, 5));
        options.setSignDateTimeTo(new Date(2022, 7, 16));
        
        // search for Digital signatures in Pptx document
        List<DigitalSignature> signatures = signature.search(DigitalSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Căutați Digital semnături electronice Live Demo"
    content: |
       Căutați în document diferite semnături electronice în fișiere Pptx chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Căutați alte semnături Digital folosind Java"
    content: |
        "Căutare de semnături electronice în diverse documente. Găsiți semnături din unul dintre formatele de fișiere populare, așa cum se arată mai jos."
    format: 
           
       
back_to_top:
    enable: true
---