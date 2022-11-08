---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Dot
productName: Java
lang: da
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Dot for Java

############################# Head ############################
head_title: "Tilføjelse af digitale elektroniske signaturer til filen Dot med Java"
head_description: "Sæt digital signatur på filen Dot for Java ved hjælp af et par linjer kode. Brug GroupDocs Document Signature API til at signere snesevis af filformater."

############################# Header ############################
title: "eSign Dot filer med Digital signaturer i Java"
description: "Sådan tilføjer du Digital-signatur med et par linjer med Java-kode"
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
    title: "Om GroupDocs.Signature for Java Digitale signaturer API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) er en populær API til at esignere dokumenter med de digitale elektroniske signaturer med digitale certifikater. Til Digitale signaturer bruger API PFX-certifikatfiler til at designe dokument med adgangskodebeskyttede private og offentlige nøgler. De digitale signaturer kan bruges til at certificere forretningsdokumenter med en bestemt eSign PDF-side, certificere hele Microsoft Office-dokumenter som Words, Excel, Powerpoint-filer og Open Office-dokumenter. Kunder kan nemt manipulere signaturerne som at redigere dem, fjerne eller justere. API'en giver mulighed for at søge og verificere signaturer. Desuden er der en masse muligheder for signaturtilpasning.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Trin til at signere Dot med Digital i Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) giver mulighed for at signere Dot dokumenter med Digital signaturer hurtigt og nemt.
        
        * Opret en forekomst af signaturklassen, der leverer Dot-fil, der skal signere som sti eller hukommelsesstrøm
        * Instantiér SignOptions-klassen og indstil alle krævede data.
        * Kald Signature.Sign()-metoden ved at sende output Dot-fil eller hukommelsesstrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for Java understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Udviklingsmiljøer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Få den seneste GroupDocs.Signature for Java fra [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dot file
        String filePath = "input.dot";
        // Set up output file
        String outputFilePath = "output.dot";
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

        // sign Dot document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering af Dot dokumenter med Digital Live Demo"
    content: |
       Signer Dot-filen med forskellige signaturer lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Gratis online demo venter på dig.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre understøttede Digital-signaturer for Java"
    content: |
        "Du kan også signere Dot med andre signaturtyper. Se venligst listen nedenfor."
    format: 
       
       
back_to_top:
    enable: true
---