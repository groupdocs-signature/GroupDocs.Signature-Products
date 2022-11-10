---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Ots
productName: Java
lang: lv
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ots for Java

############################# Head ############################
head_title: "Dzēst Digital parakstus no Ots failiem, izmantojot Java"
head_description: "Konkrētu Digital parakstu dzēšanu no parakstītiem Ots dokumentiem var viegli veikt, izmantojot īsu Java kodu."

############################# Header ############################
title: "Noņemiet Digital parakstus, kas ir ievietoti Ots failos"
description: "Izdzēsiet dažādus Digital parakstus no Ots dokumentiem. Lai noņemtu Digital parakstus, ir nepieciešams vienkāršs Java kods."
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
    title: "Iegūstiet informāciju par GroupDocs.Signature for Java API funkcijām"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API nodrošina daudzus veidus, kā apstrādāt dokumentus, izmantojot elektroniskos parakstus. Ir pieejami digitālie paraksti, piemēram, teksti, attēli, digitālie sertifikāti, svītrkodi, QR kodi, zīmogi vai metadati. Klientiem ir iespēja pievienot, dzēst, atjaunināt, pārbaudīt vai meklēt ciparparakstus PDF, MS Word dokumentos, MS Excel darbgrāmatās, MS PowerPoint prezentācijās, Adobe Photoshop failos un dažādos attēlu formātos. Tiek nodrošināts liels skaits noderīgu funkciju un iestatījumu.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kā noņemt Digital parakstus no sava Ots dokumenta"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) nodrošina noderīgu līdzekli, lai no Ots dokumentiem notīrītu Digital parakstus, izmantojot dažas koda rindiņas.
        
        * Pirmkārt, kā konstruktora parametru izveidojiet Signature objektu, kas nodod ceļu uz jūsu dokumentu.
        * Pēc tam izveidojiet atbilstošu paraksta objektu un iestatiet tā unikālo identifikatoru.
        * Pēc tam izsauciet Delete metodi, kas nodod paraksta objektu, kas ir jāizdzēš.
        * Visbeidzot, procesa darbības rezultāti.

    title_right: "Sistēmas prasības"
    content_right: |
        GroupDocs.Signature for Java tiek atbalstīti visās lielākajās platformās un operētājsistēmās. Pirms tālāk norādītā koda izpildes, lūdzu, pārliecinieties, vai jūsu sistēmā ir instalēti šādi priekšnosacījumi.

        * Operētājsistēmas: Microsoft Windows, Linux, MacOS
        * Izstrādes vides: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Lejupielādējiet jaunāko GroupDocs.Signature for Java versiju no [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ots file
        String filePath = "input.ots";
        // Set up output file
        String outputFilePath = "output.ots";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "a01e1940-997a-444b-89af-9309a2d559a5";

        // provide signature item to delete
        DigitalSignature signatureToDelete = new DigitalSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Parakstīšana ar Digital parakstiem tiešraidē"
    content: |
       Pievienojiet dažādus elektroniskos parakstus failam Ots tūlīt, apmeklējot vietni [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Izdzēsiet savus Digital parakstus, izmantojot Java"
    content: |
        "Dažādiem dokumentu formātiem pievienoto e-parakstu dzēšana. Ātri noņemiet parakstus bez papildu koda."
    format: 
       
       
back_to_top:
    enable: true
---