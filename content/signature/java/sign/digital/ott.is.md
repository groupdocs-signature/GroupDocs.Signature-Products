---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Ott
productName: Java
lang: is
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ott for Java

############################# Head ############################
head_title: "Bætir stafrænum rafrænum undirskriftum við Ott skrá með Java"
head_description: "Settu stafræna undirskrift á Ott skrá fyrir Java með því að nota nokkrar línur af kóða. Notaðu GroupDocs Document Signature API til að undirrita heilmikið af skráarsniðum."

############################# Header ############################
title: "eSign Ott skrár með Digital undirskriftum í Java"
description: "Hvernig á að bæta við Digital undirskrift með nokkrum línum af Java kóða"
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
    title: "Um GroupDocs.Signature for Java API fyrir stafrænar undirskriftir"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) er vinsælt API til að útskrifa skjöl með stafrænum rafrænum undirskriftum, með stafrænum skilríkjum. Fyrir stafrænar undirskriftir notar API PFX vottorðsskrár til að útskrifa skjal með lykilorðavörðum einka- og opinberum lyklum. Stafrænu undirskriftirnar gætu verið notaðar til að votta viðskiptaskjöl með eSign PDF tiltekinni síðu, votta heil Microsoft Office skjöl eins og Words, Excel, Powerpoint skrár og Open Office skjöl. Viðskiptavinir geta auðveldlega unnið með undirskriftirnar eins og að breyta þeim, fjarlægja eða stilla. API veitir leið til að leita og staðfesta undirskriftir. Þar að auki er mikið af hæfileikum til að sérsníða undirskriftir.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Skref til að undirrita Ott með Digital í Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) veitir möguleika á að undirrita Ott skjöl með Digital undirskrift fljótt og auðveldlega.
        
        * Búðu til tilvik af Signature class sem gefur upp Ott skrá sem á að undirrita sem slóð eða minnisstraum
        * Upphafðu SignOptions flokkinn og stilltu öll umbeðin gögn.
        * Kallaðu á Signature.Sign() aðferðina sem sendir úttak Ott skrá eða minnisstraum

    title_right: " kerfis kröfur"
    content_right: |
        GroupDocs.Signature for Java eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Fáðu nýjasta GroupDocs.Signature for Java frá [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ott file
        String filePath = "input.ott";
        // Set up output file
        String outputFilePath = "output.ott";
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

        // sign Ott document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Undirritar Ott skjöl með Digital lifandi kynningu"
    content: |
       Skrifaðu undir Ott skrána með ýmsum undirskriftum núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna. Ókeypis kynning á netinu bíður þín.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aðrar studdar Digital undirskriftir fyrir Java"
    content: |
        "Þú getur líka skrifað undir Ott með öðrum undirskriftartegundum. Vinsamlegast skoðaðu listann hér að neðan."
    format: 
       
       
back_to_top:
    enable: true
---