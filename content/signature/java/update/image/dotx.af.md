---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Dotx
productName: Java
lang: af
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Dotx for Java

############################# Head ############################
head_title: "Dateer Image-handtekeninge wat by Dotx-lêers geplaas is op met Java"
head_description: "Gebruik eenvoudig en maklik om Java-kode te verstaan ​​vir opdatering van Image-handtekeninge in ondertekende Dotx-dokumente."

############################# Header ############################
title: "Wysig en werk Image-handtekeninge op wat by Dotx-lêers geplaas is"
description: "API vir Java verskaf funksionaliteit vir Image handtekeninge wat by Dotx dokumente opdateer. Dateer e-handtekeninge binne jou Dotx dokumente op met 'n paar reëls van Java kode vinnig en maklik."
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
    title: "Kom meer te wete oor GroupDocs.Signature for Java API-kenmerke"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API-funksionaliteit bevat 'n groot verskeidenheid maniere om in aanvraag-dokumentformate te verwerk deur elektroniese handtekeninge te gebruik. Wye spektrum van e-handtekeninge soos tekste, beelde, digitale sertifikate, strepieskodes, QR-kodes, seëls of metadata word ondersteun. Kliënte kan digitale handtekeninge by PDF's, MS Word-dokumente, MS Excel-werkboeke, MS PowerPoint-aanbiedings, Adobe Photoshop-lêers en verskeie beeldformate byvoeg, verwyder, redigeer, valideer of deursoek. Talle nuttige kenmerke en instellings is beskikbaar.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hoe om Image-handtekeninge in jou Dotx-dokument te verander"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) sluit nuttige kenmerke in soos opdatering van Image-handtekeninge wat by Dotx-dokumente geplaas is. Dit maak dit moontlik om handtekeningkenmerke te verander sonder ekstra kode.
        
        * Om mee te begin, skep Signature-objek wat as 'n konstruktor-parameterpad na 'n dokument wat veronderstel is om opgedateer te word, deurgaan.
        * Instansieer dan 'n toepaslike spesifieke handtekeningvoorwerp en stel sy identifiseerder en eienskappe op wat verander moet word.
        * Laastens, roep Signature se Update-metode deur spesifieke handtekeningvoorwerp deur te gee.
        * Verwerk die opdatering van resultate na u kennisgewing.

    title_right: "Stelselvereistes"
    content_right: |
        GroupDocs.Signature for Java word op alle groot platforms en bedryfstelsels ondersteun. Voordat u die kode hieronder uitvoer, maak asseblief seker dat u die volgende voorvereistes op u stelsel geïnstalleer het.

        * Bedryfstelsels: Microsoft Windows, Linux, MacOS
        * Ontwikkelingsomgewings: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Laai die nuutste weergawe van GroupDocs.Signature for Java af vanaf [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dotx file
        String filePath = "input.dotx";
        // Set up output file
        String outputFilePath = "output.dotx";

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
    title: "Opdatering van die Image-handtekeninge op die dokumentbladsye - Live Demo"
    content: |
       Wysig verskeie elektroniese handtekeninge van die Dotx-dokument op die oomblik deur die [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) webwerf te besoek.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Dateer verskeie Image handtekeninge op via Java"
    content: |
        "Redigering van digitale handtekeninge wat in verskeie dokumentformate geplaas word. Dateer handtekeningdata op sonder ekstra kode."
    format: 
       
       
back_to_top:
    enable: true
---