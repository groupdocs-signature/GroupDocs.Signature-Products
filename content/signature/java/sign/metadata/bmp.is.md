---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Bmp
productName: Java
lang: is
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Bmp for Java

############################# Head ############################
head_title: "Bættu rafrænum undirskriftum lýsigagna við Bmp skjöl í gegnum Java"
head_description: "Notaðu Lýsigögn sem falin rafræn undirskrift í Bmp skjölunum þínum með því að nota nokkrar línur af Java kóða. Notaðu GroupDocs Document Signature API til að rafrænt undirrita viðskiptaskjölin þín og skrár með upplýsingum um lýsigögn."

############################# Header ############################
title: "Rafrænar undirskriftir með lýsigögnum fyrir Bmp skjal í gegnum Java eru einfaldar og auðveldar í notkun!"
description: "eSignaðu Bmp skjölin þín og samninga með földum lýsigagnafærslum. Búðu til lýsigögn fyrir PDF skjöl, MS Word skjöl, MS Excel vinnubækur, MS PowerPoint kynningar og ýmis myndsnið án vandræða og aukakóðun."
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
    title: "Um GroupDocs.Signature for Java Lýsigögn undirskriftarforritaskil"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) er vinsælt forritaskil fyrir rafræn undirskrift stafrænna skjala. Undirskriftir eins og textar, myndir, stafræn skilríki, strikamerki, QR-kóðar, stimplar eða lýsigögn eru tiltækar. Undirskriftir gætu verið settar á PDF skjöl, MS Word skjöl, MS Excel vinnubækur, MS PowerPoint kynningar, Adobe Photoshop skrár og ýmis myndsnið. Viðskiptavinir geta skrifað undir skjalið sitt og uppfært, leitað, staðfest, eytt eða forskoðað rafrænar undirskriftir sem settar voru á þau skjöl. Þar að auki er mikið af hæfileikum til að sérsníða undirskriftir.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Skref til að undirrita Bmp með Metadata í Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) veitir möguleika á að undirrita Bmp skjöl með Metadata undirskrift fljótt og auðveldlega.
        
        * Búðu til tilvik af Signature class sem gefur upp Bmp skrá sem á að undirrita sem slóð eða minnisstraum
        * Upphafðu SignOptions flokkinn og stilltu öll umbeðin gögn.
        * Kallaðu á Signature.Sign() aðferðina sem sendir úttak Bmp skrá eða minnisstraum

    title_right: " kerfis kröfur"
    content_right: |
        GroupDocs.Signature for Java eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Fáðu nýjasta GroupDocs.Signature for Java frá [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Bmp file
        String filePath = "input.bmp";
        // Set up output file
        String outputFilePath = "output.bmp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Bmp document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Undirritar Bmp skjöl með Metadata lifandi kynningu"
    content: |
       Skrifaðu undir Bmp skrána með ýmsum undirskriftum núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna. Ókeypis kynning á netinu bíður þín.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aðrar studdar Metadata undirskriftir fyrir Java"
    content: |
        "Þú getur líka skrifað undir Bmp með öðrum undirskriftartegundum. Vinsamlegast skoðaðu listann hér að neðan."
    format: 
       
       
back_to_top:
    enable: true
---