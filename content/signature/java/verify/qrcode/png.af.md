---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Png
productName: Java
lang: af
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Png for Java

############################# Head ############################
head_title: "Verifikasie van Qrcode handtekeninge vir Png lêers via Java"
head_description: "Gebruik slegs 'n paar reëls van Java-kode om Png-dokumente en hul Qrcode-handtekeninge te verifieer."

############################# Header ############################
title: "Qrcode handtekeningverifikasie vir {{Lêerformaat}} lêers"
description: "API vir Java bied geleentheid om Qrcode handtekeninge by Png dokumente te verifieer. Verifikasie van e-handtekeninge binne jou {{Lêerformaat}} dokumente kan vinnig en maklik uitgevoer word."
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
    title: "Ontdek nuwe GroupDocs.Signature for Java API-kenmerke"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API bied wye verskeidenheid maniere om talle dokumentformate te verwerk deur elektroniese handtekeninge te gebruik. Baie soorte digitale handtekeninge soos tekste, beelde, digitale sertifikate, strepieskodes, QR-kodes, seëls of metadata word ondersteun. Kliënte kan digitale handtekeninge by PDF's, MS Word-dokumente, MS Excel-werkboeke, MS PowerPoint-aanbiedings, Adobe Photoshop-lêers en verskeie beeldformate byvoeg, verwyder, redigeer, valideer of deursoek. Verstommende aantal bykomende kenmerke en instellings is beskikbaar.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hoe om Qrcode handtekeninge in jou Png dokument te bekragtig"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) sluit nuttige kenmerke in soos verifikasie van Qrcode-handtekeninge wat by {{Lêerformaat}}-dokumente geplaas word. Gebruik hierdie geleentheid sonder om ekstra kode te implementeer.
        
        * Eerstens, instansieer Handtekeningklas wat as 'n konstruktor parameter pad verskaf na 'n dokument wat veronderstel is om geverifieer te word.
        * Tweedens, skep 'n nuwe VerifyOptions-objek en stel alle vereiste eienskappe op.
        * Laastens, roep Signature se objek Verifieer-metode deur VerifyOptions-instansie deur te gee.
        * Verwerk dan verifikasieresultate.

    title_right: "Stelselvereistes"
    content_right: |
        GroupDocs.Signature for Java word op alle groot platforms en bedryfstelsels ondersteun. Voordat u die kode hieronder uitvoer, maak asseblief seker dat u die volgende voorvereistes op u stelsel geïnstalleer het.

        * Bedryfstelsels: Microsoft Windows, Linux, MacOS
        * Ontwikkelingsomgewings: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Laai die nuutste weergawe van GroupDocs.Signature for Java af vanaf [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Png file
        String filePath = "input.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        QrCodeVerifyOptions options = new QrCodeVerifyOptions();

        // process only first page
        options.setPagesSetup(new PagesSetup());
        options.setPageNumber(1);
        options.setAllPages(false);
        // specify text match type
        options.setMatchType(TextMatchType.StartsWith);
        // specify text pattern to search
        options.setText("QrCode text");
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ondertekening met Qrcode handtekeninge Live Demo"
    content: |
       Voeg nou verskeie elektroniese handtekeninge by die Png-lêer deur die [GroupDocs.Signature-toepassing](https://products.groupdocs.app/signature/family) webwerf te besoek.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verifieer ander Qrcode handtekeninge met behulp van Java"
    content: |
        "Verifikasie van elektroniese handtekeninge wat in verskeie dokumente geplaas is. Kontroleer die kwaliteit van handtekeninge in die gewilde lêerformate soos hieronder geopenbaar."
    format: 
       
       
back_to_top:
    enable: true
---