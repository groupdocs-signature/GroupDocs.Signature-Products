---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Xltm
productName: Java
lang: is
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Xltm for Java

############################# Head ############################
head_title: "Eyða Text undirskriftum úr Xltm skrám í gegnum Java"
head_description: "Auðvelt er að eyða tilteknum Text undirskriftum úr undirrituðum Xltm skjölum með stuttum Java kóða."

############################# Header ############################
title: "Fjarlægðu Text undirskriftir sem eru settar í Xltm skrár"
description: "Eyða ýmsum Text undirskriftum úr Xltm skjölum. Til að fjarlægja Text undirskrift þarf einfaldan Java kóða."
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
    title: "Fáðu upplýsingar um eiginleika GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API veitir margar leiðir til að vinna úr skjölum þínum með rafrænum undirskriftum. Stafrænar undirskriftir eins og textar, myndir, stafræn skilríki, strikamerki, QR-kóðar, stimplar eða lýsigögn eru tiltækar. Viðskiptavinir hafa möguleika á að bæta við, eyða, uppfæra, sannreyna eða leita í stafrænum undirskriftum á PDF skjölum, MS Word skjölum, MS Excel vinnubókum, MS PowerPoint kynningum, Adobe Photoshop skrám og ýmsum myndsniðum. Mikill fjöldi gagnlegra eiginleika og stillinga er til staðar.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hvernig á að fjarlægja Text undirskriftir úr Xltm skjalinu þínu"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) býður upp á gagnlegan eiginleika til að hreinsa Xltm skjöl af Text undirskriftum með nokkrum línum af kóða.
        
        * Í fyrsta lagi, staðfestu Signature hlut sem fer í gegnum slóðina í skjalið þitt sem byggingarbreytu.
        * Búðu síðan til viðeigandi undirskriftarhlut og settu upp einstakt auðkenni hans.
        * Eftir það skaltu kalla á Delete method sem sendir undirskriftarhlut sem verður að eyða.
        * Að lokum, niðurstöður vinnsluaðgerða.

    title_right: "kerfis kröfur"
    content_right: |
        GroupDocs.Signature for Java eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Sæktu nýjustu útgáfuna af GroupDocs.Signature for Java frá [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xltm file
        String filePath = "input.xltm";
        // Set up output file
        String outputFilePath = "output.xltm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to delete
        TextSignature signatureToDelete = new TextSignature(id);

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
    title: "Undirskrift með Text undirskriftum Live Demo"
    content: |
       Bættu ýmsum rafrænum undirskriftum við Xltm skrá núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Eyddu Text undirskriftunum þínum með Java"
    content: |
        "Eyðing rafrænna undirskrifta sem bætt var við ýmis skjalasnið. Fjarlægðu undirskriftir fljótt án aukakóða."
    format: 
       
       
back_to_top:
    enable: true
---