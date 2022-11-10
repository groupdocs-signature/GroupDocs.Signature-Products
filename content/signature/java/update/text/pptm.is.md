---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Pptm
productName: Java
lang: is
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Pptm for Java

############################# Head ############################
head_title: "Uppfærðu Text undirskriftir settar á Pptm skrár með Java"
head_description: "Notaðu einfaldan og auðskilinn Java kóða fyrir uppfærslu á Text undirskriftum í undirrituðum Pptm skjölum."

############################# Header ############################
title: "Breyttu og uppfærðu Text undirskriftir sem settar eru á Pptm skrár"
description: "API fyrir Java veitir virkni fyrir Text undirskriftir sem uppfæra á Pptm skjölum. Uppfærðu rafrænar undirskriftir í Pptm skjölunum þínum með nokkrum línum af Java kóða fljótt og auðveldlega."
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
    title: "Lærðu um GroupDocs.Signature for Java API eiginleika"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API virkni inniheldur mikið úrval af aðferðum til að vinna eftirspurn eftir skjölum með því að nota rafrænar undirskriftir. Fjölbreytt úrval rafrænna undirskrifta eins og texta, myndir, stafræn skilríki, strikamerki, QR-kóða, stimpla eða lýsigögn eru studd. Viðskiptavinir geta bætt við, fjarlægt, breytt, staðfest eða leitað í stafrænum undirskriftum á PDF skjölum, MS Word skjölum, MS Excel vinnubókum, MS PowerPoint kynningum, Adobe Photoshop skrám og ýmsum myndsniðum. Fjölmargir gagnlegir eiginleikar og stillingar eru í boði.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hvernig á að breyta Text undirskriftum í Pptm skjalinu þínu"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) inniheldur gagnlega eiginleika eins og uppfærslu á Text undirskriftum sem settar eru á Pptm skjöl. Það gerir mögulegt að breyta eiginleikum undirskrifta án aukakóða.
        
        * Til að byrja með, búðu til Signature hlut sem fer sem slóð byggingarbreytu í skjal sem á að uppfæra.
        * Settu síðan upp viðeigandi tiltekinn undirskriftarhlut og settu upp auðkenni hans og eiginleika sem þarf að breyta.
        * Að lokum skaltu kalla uppfærsluaðferð Signature sem sendir tiltekinn undirskriftarhlut.
        * Vinndu við að uppfæra niðurstöður til þín.

    title_right: "kerfis kröfur"
    content_right: |
        GroupDocs.Signature for Java eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Sæktu nýjustu útgáfuna af GroupDocs.Signature for Java frá [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pptm file
        String filePath = "input.pptm";
        // Set up output file
        String outputFilePath = "output.pptm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to update
        // set up particular signature id
        TextSignature signatureToUpdate = new TextSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(130);
        // specify signature height
        signatureToUpdate.setHeight(20);
        // set left position
        signatureToUpdate.setLeft(40);
        // set top position
        signatureToUpdate.setTop(50);
        // set up new text
        signatureToUpdate.setText("Mr. John Smith");

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
    title: "Að uppfæra Text undirskriftirnar á skjalasíðunum - Sýning í beinni"
    content: |
       Breyttu ýmsum rafrænum undirskriftum Pptm skjalsins núna með því að fara á vefsíðuna [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Uppfærðu ýmsar Text undirskriftir í gegnum Java"
    content: |
        "Breyta stafrænum undirskriftum sem eru settar á mismunandi skjalasnið. Uppfærðu undirskriftargögn án aukakóða."
    format: 
       
       
back_to_top:
    enable: true
---