---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Doc
productName: Java
lang: is
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Doc for Java

############################# Head ############################
head_title: "Búðu til rafrænar undirskriftir í Doc skrá með Java"
head_description: "Settu Text eSignature á Doc skrá fyrir Java með því að nota nokkrar línur af kóða. Notaðu GroupDocs Document Signature API til að undirrita heilmikið af skráarsniðum."

############################# Header ############################
title: "Undirritaðu Doc skrár með Text undirskriftum í Java"
description: "Hvernig á að bæta við Text undirskrift með nokkrum línum af Java kóða"
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
    title: "Um GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) er vinsælt forritaskil fyrir rafræn undirskrift stafrænna skjala. Undirskriftir eins og textar, myndir, stafræn skilríki, strikamerki, QR-kóðar, stimplar eða lýsigögn eru tiltækar. Undirskriftir gætu verið settar á PDF skjöl, MS Word skjöl, MS Excel vinnubækur, MS PowerPoint kynningar, Adobe Photoshop skrár og ýmis myndsnið. Viðskiptavinir geta skrifað undir skjalið sitt og uppfært, leitað, staðfest, eytt eða forskoðað rafrænar undirskriftir sem settar voru á þau skjöl. Þar að auki er mikið af hæfileikum til að sérsníða undirskriftir.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Skref til að undirrita Doc með Text í Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) veitir möguleika á að undirrita Doc skjöl með Text undirskrift fljótt og auðveldlega.
        
        * Búðu til tilvik af Signature class sem gefur upp Doc skrá sem á að undirrita sem slóð eða minnisstraum
        * Upphafðu SignOptions flokkinn og stilltu öll umbeðin gögn.
        * Kallaðu á Signature.Sign() aðferðina sem sendir úttak Doc skrá eða minnisstraum

    title_right: " kerfis kröfur"
    content_right: |
        GroupDocs.Signature for Java eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Fáðu nýjasta GroupDocs.Signature for Java frá [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Doc file
        String filePath = "input.doc";
        // Set up output file
        String outputFilePath = "output.doc";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Doc document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Undirritar Doc skjöl með Text lifandi kynningu"
    content: |
       Skrifaðu undir Doc skrána með ýmsum undirskriftum núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna. Ókeypis kynning á netinu bíður þín.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aðrar studdar Text undirskriftir fyrir Java"
    content: |
        "Þú getur líka skrifað undir Doc með öðrum undirskriftartegundum. Vinsamlegast skoðaðu listann hér að neðan."
    format: 
       
       
back_to_top:
    enable: true
---