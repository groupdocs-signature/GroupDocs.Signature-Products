---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Ott
productName: Java
lang: af
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ott for Java

############################# Head ############################
head_title: "Vee Digital handtekeninge van Ott lêers uit via Java"
head_description: "Die uitvee van spesifieke Digital handtekeninge van getekende {{Lêerformaat}} dokumente kan maklik uitgevoer word met kort Java kode."

############################# Header ############################
title: "Verwyder Digital handtekeninge wat in {{Lêerformaat}} lêers geplaas is"
description: "Vee verskeie Digital handtekeninge uit {{Lêerformaat}} dokumente uit. Die verwydering van Digital handtekeninge vereis eenvoudige Java kode."
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
    title: "Kry inligting oor GroupDocs.Signature for Java API-kenmerke"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API bied baie maniere om jou dokumente te verwerk deur elektroniese handtekeninge te gebruik. Digitale handtekeninge soos tekste, beelde, digitale sertifikate, strepieskodes, QR-kodes, seëls of metadata is beskikbaar. Kliënte het die moontlikheid om digitale handtekeninge by PDF's, MS Word-dokumente, MS Excel-werkboeke, MS PowerPoint-aanbiedings, Adobe Photoshop-lêers en verskeie beeldformate by te voeg, uit te vee, op te dateer, te verifieer of te soek. 'n Groot aantal nuttige kenmerke en instellings word verskaf.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hoe om Digital-handtekeninge uit jou {{Lêerformaat}}-dokument te verwyder"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) bied nuttige kenmerk vir die skoonmaak van {{Lêerformaat}} dokumente van Digital handtekeninge met 'n paar reëls kode.
        
        * Eerstens, instansieer Handtekening-objek wat deurgaanpad na jou dokument as 'n konstruktor parameter.
        * Skep dan 'n toepaslike handtekeningvoorwerp en stel sy unieke identifiseerder op.
        * Daarna, roep Verwyder metode deur handtekeningvoorwerp wat uitgevee moet word.
        * Laastens, die resultate van die proses.

    title_right: "Stelselvereistes"
    content_right: |
        GroupDocs.Signature for Java word op alle groot platforms en bedryfstelsels ondersteun. Voordat u die kode hieronder uitvoer, maak asseblief seker dat u die volgende voorvereistes op u stelsel geïnstalleer het.

        * Bedryfstelsels: Microsoft Windows, Linux, MacOS
        * Ontwikkelingsomgewings: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Laai die nuutste weergawe van GroupDocs.Signature for Java af vanaf [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ott file
        String filePath = "input.ott";
        // Set up output file
        String outputFilePath = "output.ott";

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
    title: "Ondertekening met Digital handtekeninge Live Demo"
    content: |
       Voeg nou verskeie elektroniese handtekeninge by die Ott-lêer deur die [GroupDocs.Signature-toepassing](https://products.groupdocs.app/signature/family) webwerf te besoek.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Vee jou Digital handtekeninge uit met Java"
    content: |
        "Skraping van e-handtekeninge wat by verskeie dokumentformate gevoeg is. Verwyder handtekeninge vinnig sonder ekstra kode."
    format: 
       
       
back_to_top:
    enable: true
---