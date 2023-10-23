---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Tar
productName: Java
lang: sv
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Tar for Java

############################# Head ############################
head_title: "Lägger till digitala elektroniska signaturer i filen Tar med Java"
head_description: "Lägg digital signatur på filen Tar för Java med några rader kod. Använd GroupDocs Document Signature API för att signera dussintals filformat."

############################# Header ############################
title: "eSign Tar-filer med Digital-signaturer i Java"
description: "Hur man lägger till Digital-signatur med några rader med Java-kod"
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
    title: "Om GroupDocs.Signature for Java API för digitala signaturer"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) är ett populärt API för att esignera dokument med digitala elektroniska signaturer, med digitala certifikat. För digitala signaturer använder API PFX-certifikatfiler för att esignera dokument med lösenordsskyddade privata och publika nycklar. De digitala signaturerna kan användas för att certifiera affärsdokument med eSign PDF-specifik sida, certifiera hela Microsoft Office-dokument som Words, Excel, Powerpoint-filer och Open Office-dokument. Kunder kan enkelt manipulera signaturerna som att redigera dem, ta bort eller justera. API ger ett sätt att söka och verifiera signaturer. Dessutom tillhandahålls många funktioner för anpassning av signaturer.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Steg för att signera Tar med Digital i Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ger möjlighet att signera Tar-dokument med Digital-signaturer snabbt och enkelt.
        
        * Skapa en instans av Signature class som tillhandahåller Tar fil som ska signera som sökväg eller minnesström
        * Instantera SignOptions-klassen och ställ in all efterfrågad data.
        * Anropa metoden Signature.Sign() och skicka utdatafilen Tar eller minnesström

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for Java stöds på alla större plattformar och operativsystem. Innan du kör koden nedan, se till att du har följande förutsättningar installerade på ditt system.

        * Operativsystem: Microsoft Windows, Linux, MacOS
        * Utvecklingsmiljöer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Få den senaste GroupDocs.Signature for Java från [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Tar file
        String filePath = "input.tar";
        // Set up output file
        String outputFilePath = "output.tar";
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

        // sign Tar document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signerar Tar dokument med Digital Live Demo"
    content: |
       Signera filen Tar med olika signaturer just nu genom att besöka webbplatsen [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Gratis onlinedemo väntar på dig.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andra stödda Digital-signaturer för Java"
    content: |
        "Du kan också signera Tar med andra signaturtyper. Se listan nedan."
    format: 
       
       
back_to_top:
    enable: true
---