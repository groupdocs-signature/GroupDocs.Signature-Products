---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Potm
productName: Java
lang: sv
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Potm for Java

############################# Head ############################
head_title: "Uppdatera Image-signaturer placerade i Potm-filer med Java"
head_description: "Använd enkel och lätt att förstå Java-koden för uppdatering av Image-signaturer i signerade Potm-dokument."

############################# Header ############################
title: "Redigera och uppdatera Image-signaturer placerade i Potm-filer"
description: "API för Java tillhandahåller funktionalitet för Image-signaturer som uppdateras i Potm-dokument. Uppdatera e-signaturer i dina Potm-dokument med ett par rader Java-kod snabbt och enkelt."
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
    title: "Läs mer om GroupDocs.Signature for Java API-funktioner"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API-funktionalitet innehåller ett stort urval av sätt att behandla efterfrågade dokumentformat genom att använda elektroniska signaturer. Ett brett spektrum av e-signaturer som texter, bilder, digitala certifikat, streckkoder, QR-koder, stämplar eller metadata stöds. Kunder kan lägga till, ta bort, redigera, validera eller söka i digitala signaturer i PDF-filer, MS Word-dokument, MS Excel-arbetsböcker, MS PowerPoint-presentationer, Adobe Photoshop-filer och olika bildformat. Många användbara funktioner och inställningar är tillgängliga.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Så här ändrar du Image-signaturer i ditt Potm-dokument"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) innehåller användbara funktioner som uppdatering av Image-signaturer placerade i Potm-dokument. Det gör det möjligt att ändra signaturfunktioner utan extra kod.
        
        * Till att börja med, skapa signaturobjekt som passerar som en konstruktorparametersökväg till ett dokument som ska uppdateras.
        * Instantiera sedan ett lämpligt särskilt signaturobjekt och ställ in dess identifierare och egenskaper som behöver ändras.
        * Till sist, anropa Signatures uppdateringsmetod som skickar ett visst signaturobjekt.
        * Bearbeta uppdatering av resultat till ditt meddelande.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for Java stöds på alla större plattformar och operativsystem. Innan du kör koden nedan, se till att du har följande förutsättningar installerade på ditt system.

        * Operativsystem: Microsoft Windows, Linux, MacOS
        * Utvecklingsmiljöer: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Ladda ner den senaste versionen av GroupDocs.Signature for Java från [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Potm file
        String filePath = "input.potm";
        // Set up output file
        String outputFilePath = "output.potm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to update
        // set up particular signature id
        ImageSignature signatureToUpdate = new ImageSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(170);
        // specify signature height
        signatureToUpdate.setHeight(250);
        // set left position
        signatureToUpdate.setLeft(10);
        // set top position
        signatureToUpdate.setTop(10);

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Uppdatering av Image-signaturerna på dokumentsidorna - Live Demo"
    content: |
       Redigera olika elektroniska signaturer för Potm-dokumentet just nu genom att besöka webbplatsen [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Uppdatera olika Image-signaturer via Java"
    content: |
        "Redigera digitala signaturer som placeras i olika dokumentformat. Uppdatera signaturdata utan extra kod."
    format: 
       
       
back_to_top:
    enable: true
---