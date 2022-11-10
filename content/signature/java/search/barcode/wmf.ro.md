---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Barcode
fileformat: Wmf
productName: Java
lang: ro
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Barcode signatures at Wmf with Java

############################# Head ############################
head_title: "Căutați semnături Barcode în fișierul Wmf în Java"
head_description: "Utilizați Java pentru a căuta semnături Barcode în fișiere Wmf folosind câteva rânduri de cod."

############################# Header ############################
title: "Căutați semnături Barcode în fișierul Wmf"
description: "API-ul nativ Java permite căutarea semnăturilor Barcode în fișierele Wmf deja semnate. Efectuați o căutare avansată de semnătură electronică în documentele dvs. Wmf folosind câteva rânduri de cod."
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
    title_left: "Cum să căutați semnături Barcode în Wmf"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) facilitează pentru dezvoltatorii Java să caute semnături Barcode în fișierele Wmf din aplicațiile lor prin implementarea câțiva pași simpli.
        
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
        
        // Set up input Wmf file
        String filePath = "input.wmf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        BarcodeSearchOptions options = new BarcodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Barcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Barcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Barcode signatures in Wmf document
        List<BarcodeSignature> signatures = signature.search(BarcodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Căutați Barcode semnături electronice Live Demo"
    content: |
       Căutați în document diferite semnături electronice în fișiere Wmf chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Căutați alte semnături Barcode folosind Java"
    content: |
        "Căutare de semnături electronice în diverse documente. Găsiți semnături din unul dintre formatele de fișiere populare, așa cum se arată mai jos."
    format: 
           
       
back_to_top:
    enable: true
---