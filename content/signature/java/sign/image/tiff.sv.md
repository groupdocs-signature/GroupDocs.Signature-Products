---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Tiff
productName: Java
lang: sv
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Tiff for Java

############################# Head ############################
head_title: "Lägger till Image-signaturer i filen Tiff med Java"
head_description: "Sätt Image Signatur på Tiff-filen för Java med några rader kod. Använd GroupDocs Document Signature API för att signera dussintals filformat."

############################# Header ############################
title: "Signera Tiff-filer med Image-signaturer i Java"
description: "Hur man lägger till Image-signatur med några rader med Java-kod"
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
    title: "Om GroupDocs.Signature for Java API för bildsignaturer"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) är ett populärt API för e-signering av digitala dokument. Signaturer som texter, bilder, digitala certifikat, streckkoder, QR-koder, stämplar eller metadata finns tillgängliga. Signaturer kan placeras på PDF-filer, MS Word-dokument, MS Excel-arbetsböcker, MS PowerPoint-presentationer, Adobe Photoshop-filer och olika bildformat. Kunder kan signera sina dokument och uppdatera, söka, verifiera, ta bort eller förhandsgranska e-signaturer som satts på dessa dokument. Dessutom tillhandahålls många funktioner för anpassning av signaturer.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Steg för att signera Tiff med Image i Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ger möjlighet att signera Tiff-dokument med Image-signaturer snabbt och enkelt.
        
        * Skapa en instans av Signature class som tillhandahåller Tiff fil som ska signera som sökväg eller minnesström
        * Instantera SignOptions-klassen och ställ in all efterfrågad data.
        * Anropa metoden Signature.Sign() och skicka utdatafilen Tiff eller minnesström

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for Java stöds på alla större plattformar och operativsystem. Innan du kör koden nedan, se till att du har följande förutsättningar installerade på ditt system.

        * Operativsystem: Microsoft Windows, Linux, MacOS
        * Utvecklingsmiljöer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Få den senaste GroupDocs.Signature for Java från [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Tiff file
        String filePath = "input.tiff";
        // Set up output file
        String outputFilePath = "output.tiff";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Tiff document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signerar Tiff dokument med Image Live Demo"
    content: |
       Signera filen Tiff med olika signaturer just nu genom att besöka webbplatsen [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Gratis onlinedemo väntar på dig.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andra stödda Image-signaturer för Java"
    content: |
        "Du kan också signera Tiff med andra signaturtyper. Se listan nedan."
    format: 
       
       
back_to_top:
    enable: true
---