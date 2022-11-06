---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Text
fileformat: Ott
productName: Java
lang: is
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Ott for Java

############################# Head ############################
head_title: "Staðfesting á Text undirskriftum fyrir Ott skrár í gegnum Java"
head_description: "Notaðu aðeins nokkrar línur af Java kóða til að staðfesta Ott skjöl og Text undirskrift þeirra."

############################# Header ############################
title: "Text staðfesting á undirskriftum fyrir Ott skrár"
description: "API fyrir Java veitir tækifæri til að staðfesta Text undirskriftir á Ott skjölum. Staðfesting á rafrænum undirskriftum inni í Ott skjölunum þínum gæti verið framkvæmd fljótt og auðveldlega."
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
    title: "Uppgötvaðu nýja eiginleika GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API býður upp á fjölbreytt úrval leiða til að vinna úr fjölmörgum skjalasniðum með því að nota rafrænar undirskriftir. Margar tegundir stafrænna undirskrifta eins og texta, myndir, stafræn skilríki, strikamerki, QR-kóða, stimpla eða lýsigögn eru studdar. Viðskiptavinir geta bætt við, fjarlægt, breytt, staðfest eða leitað í stafrænum undirskriftum á PDF skjölum, MS Word skjölum, MS Excel vinnubókum, MS PowerPoint kynningum, Adobe Photoshop skrám og ýmsum myndsniðum. Ótrúlegur fjöldi viðbótareiginleika og stillinga er í boði.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hvernig á að staðfesta Text undirskriftir í Ott skjalinu þínu"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) inniheldur gagnlega eiginleika eins og staðfestingu á Text undirskriftum sem settar eru á Ott skjöl. Notaðu þetta tækifæri án þess að innleiða aukakóða.
        
        * Í fyrsta lagi, staðfestu undirskriftarflokk sem veitir slóð fyrir breytu byggingaraðila að skjali sem á að vera staðfest.
        * Í öðru lagi, búðu til nýjan VerifyOptions hlut og settu upp alla nauðsynlega eiginleika.
        * Að lokum skaltu kalla á hlut Staðfestingaraðferð Signature sem framhjá VerifyOptions tilviki.
        * Vinndu síðan úr sannprófunarniðurstöðum.

    title_right: "kerfis kröfur"
    content_right: |
        GroupDocs.Signature for Java eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Sæktu nýjustu útgáfuna af GroupDocs.Signature for Java frá [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ott file
        String filePath = "input.ott";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        TextVerifyOptions options = new TextVerifyOptions();

        // Process all pages
        options.setAllPages(true);
        // specify text match type
        options.setMatchType(TextMatchType.Exact);
        // specify text pattern to search
        options.setText("Very important signature");
                            
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
    title: "Undirskrift með Text undirskriftum Live Demo"
    content: |
       Bættu ýmsum rafrænum undirskriftum við Ott skrá núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Staðfestu aðrar Text undirskriftir með Java"
    content: |
        "Staðfesting rafrænna undirskrifta sem settar eru í ýmis skjöl. Athugaðu gæði undirskrifta í vinsælu skráarsniðunum eins og sýnt er hér að neðan."
    format: 
       
       
back_to_top:
    enable: true
---