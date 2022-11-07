---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Dotx
productName: Java
lang: sv
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Dotx for Java

############################# Head ############################
head_title: "Skapa elektroniska textsignaturer till filen Dotx med Java"
head_description: "Sätt Text eSignature på filen Dotx för Java med några rader kod. Använd GroupDocs Document Signature API för att signera dussintals filformat."

############################# Header ############################
title: "Signera {{Filformat}}-filer med Text-signaturer i Java"
description: "Hur man lägger till Text-signatur med några rader med Java-kod"
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
    title: "Om GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) är ett populärt API för e-signering av digitala dokument. Signaturer som texter, bilder, digitala certifikat, streckkoder, QR-koder, stämplar eller metadata finns tillgängliga. Signaturer kan placeras på PDF-filer, MS Word-dokument, MS Excel-arbetsböcker, MS PowerPoint-presentationer, Adobe Photoshop-filer och olika bildformat. Kunder kan signera sina dokument och uppdatera, söka, verifiera, ta bort eller förhandsgranska e-signaturer som satts på dessa dokument. Dessutom tillhandahålls många funktioner för anpassning av signaturer.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Steg för att signera {{Filformat}} med Text i Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ger möjlighet att signera Dotx-dokument med Text-signaturer snabbt och enkelt.
        
        * Skapa en instans av Signature class som tillhandahåller Dotx fil som ska signera som sökväg eller minnesström
        * Instantera SignOptions-klassen och ställ in all efterfrågad data.
        * Anropa metoden Signature.Sign() och skicka utdatafilen Dotx eller minnesström

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for Java stöds på alla större plattformar och operativsystem. Innan du kör koden nedan, se till att du har följande förutsättningar installerade på ditt system.

        * Operativsystem: Microsoft Windows, Linux, MacOS
        * Utvecklingsmiljöer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Få den senaste GroupDocs.Signature for Java från [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dotx file
        String filePath = "input.dotx";
        // Set up output file
        String outputFilePath = "output.dotx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Dotx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signerar {{Filformat}} dokument med Text Live Demo"
    content: |
       Signera filen Dotx med olika signaturer just nu genom att besöka webbplatsen [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Gratis onlinedemo väntar på dig.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andra stödda Text-signaturer för Java"
    content: |
        "Du kan också signera {{Filformat}} med andra signaturtyper. Se listan nedan."
    format: 
       
       
back_to_top:
    enable: true
---