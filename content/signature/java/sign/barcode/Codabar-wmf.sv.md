---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Wmf
productName: Java
lang: sv
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Wmf for Java

############################# Head ############################
head_title: "eSign Wmf dokument med Codabar streckkod i Java"
head_description: "Skapa Codabar streckkodsignatur och lägg den på Wmf dokument med Java med ett par rader kod. Använd GroupDocs Document Signature API för att signera olika filformat."

############################# Header ############################
title: "Generera Codabar streckkodsignatur för Wmf dokument i Java"
description: "esignera dina Wmf affärsdokument med Codabar streckkod. Skapa streckkodsignatur snabbt och enkelt med några rader kod för att ställa in signeringsalternativ."
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
    title: "Om GroupDocs.Signature for Java API för streckkodsignaturer."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) är ett snabbt och enkelt API för att hantera digitala dokument e-signering med streckkodstyper som UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 och många andra. Kunder kan enkelt skapa streckkoder som ger önskad text och lägga dem på PDF, Microsoft Office Words-dokument, Microsoft Office Excel-arbetsböcker, MS PowerPoint-presentationer, Adobe Photoshop-filer och olika bildformat. Streckkoder som placeras i dokument kan uppdateras, genomsökas, verifieras, raderas eller förhandsgranskas antingen. Dessutom stöds anpassning av streckkoder.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Steg för att signera Wmf med Barcode i Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ger möjlighet att signera Wmf-dokument med Barcode-signaturer snabbt och enkelt.
        
        * Skapa en instans av Signature class som tillhandahåller Wmf fil som ska signera som sökväg eller minnesström
        * Instantera SignOptions-klassen och ställ in all efterfrågad data.
        * Anropa metoden Signature.Sign() och skicka utdatafilen Wmf eller minnesström

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for Java stöds på alla större plattformar och operativsystem. Innan du kör koden nedan, se till att du har följande förutsättningar installerade på ditt system.

        * Operativsystem: Microsoft Windows, Linux, MacOS
        * Utvecklingsmiljöer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Få den senaste GroupDocs.Signature for Java från [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Wmf file
        String filePath = "input.wmf";
        // Set up output file
        String outputFilePath = "output.wmf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Codabar);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Wmf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signerar Wmf dokument med Barcode Live Demo"
    content: |
       Signera filen Wmf med olika signaturer just nu genom att besöka webbplatsen [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Gratis onlinedemo väntar på dig.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar är en linjär streckkodssymbologi som designades för att kunna läsas exakt även när den skrivs ut på matrisskrivare för flerdelade formulär som FedEx flygsedlar och blodbanksformulär.
          characterset: |
             Numeriska siffror (0-9) och specialtecken $/-:+.
          textcapacity: |
             Inga specifika begränsningar.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andra stödda Barcode-signaturer för Java"
    content: |
        "Du kan också signera Wmf med andra signaturtyper. Se listan nedan."
    format: 
        
       
back_to_top:
    enable: true
---