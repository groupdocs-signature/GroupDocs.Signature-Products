---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Ots
productName: Java
lang: sv
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Ots with Java

############################# Head ############################
head_title: "Sök efter Image-signaturer i filen Ots i Java"
head_description: "Använd Java för att söka efter Image-signaturer i Ots-filer med några rader kod."

############################# Header ############################
title: "Sök efter Image-signaturer i filen Ots"
description: "Inbyggt API för Java gör det möjligt att söka efter Image-signaturer i redan signerade Ots-filer. Utför avancerad e-signatursökning i dina Ots-dokument med några rader kod."
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
    title: "Om GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) tillhandahåller Java API för att bearbeta dokument med olika signaturtyper som texter, bilder, digitala certifikat, streckkoder, QR-koder, stämplar eller metadata. Användare kan lägga till, ta bort, uppdatera, verifiera eller söka efter elektroniska signaturer i PDF-filer, MS Word-dokument, MS Excel-arbetsböcker, MS PowerPoint-presentationer, Adobe Photoshop-filer och olika bildformat, med ytterligare stöd för att anpassa signaturegenskaper efter behov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hur man söker efter Image-signaturer i Ots"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gör det enklare för Java-utvecklare att söka efter Image-signaturer i Ots-filer från sina applikationer genom att implementera några enkla steg.
        
        * Skapa en ny instans av Signature-klassen och skicka källdokumentsökvägen som en konstruktorparameter.
        * Instantiera SearchOptions-objektet enligt dina krav och ange sökalternativ.
        * Anrop sökmetoden för Signature-klassinstansen och skicka SearchOptions till den.
        * Bearbeta sökresultaten efter dina krav.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for Java stöds på alla större plattformar och operativsystem. Innan du kör koden nedan, se till att du har följande förutsättningar installerade på ditt system.

        * Operativsystem: Microsoft Windows, Linux, MacOS
        * Utvecklingsmiljöer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Ladda ner den senaste versionen av GroupDocs.Signature for Java från [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ots file
        String filePath = "input.ots";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        ImageSearchOptions options = new ImageSearchOptions();

        // set minimum size if needed 
        options.setMinContentSize(100);
        // set maximum image size if needed
        options.setMaxContentSize(2000);
        // return images for processing
        options.setReturnContent(true);
        // set up type of returned images
        options.setReturnContentType(FileType.PNG);

        // search for Image signatures in Ots document
        List<ImageSignature> signatures = signature.search(ImageSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Sök efter Image elektroniska signaturer Live Demo"
    content: |
       Sök i dokumentet efter olika elektroniska signaturer till Ots-filer just nu genom att besöka webbplatsen [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Sök efter andra Image-signaturer med Java"
    content: |
        "Sök efter elektroniska signaturer i olika dokument. Hitta signaturer från ett av de populära filformaten som visas nedan."
    format: 
           
       
back_to_top:
    enable: true
---