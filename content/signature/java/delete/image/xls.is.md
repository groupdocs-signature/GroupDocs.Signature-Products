---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Xls
productName: Java
lang: is
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Xls for Java

############################# Head ############################
head_title: "Eyða Image undirskriftum úr Xls skrám í gegnum Java"
head_description: "Auðvelt er að eyða tilteknum Image undirskriftum úr undirrituðum Xls skjölum með stuttum Java kóða."

############################# Header ############################
title: "Fjarlægðu Image undirskriftir sem eru settar í Xls skrár"
description: "Eyða ýmsum Image undirskriftum úr Xls skjölum. Til að fjarlægja Image undirskrift þarf einfaldan Java kóða."
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
    title_left: "Hvernig á að fjarlægja Image undirskriftir úr Xls skjalinu þínu"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) býður upp á gagnlegan eiginleika til að hreinsa Xls skjöl af Image undirskriftum með nokkrum línum af kóða.
        
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
                
        // Set up input Xls file
        String filePath = "input.xls";
        // Set up output file
        String outputFilePath = "output.xls";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "e3ad0ec7-9abf-426d-b9aa-b3328f3f1470";

        // provide signature features to delete
        ImageSignature signatureToDelete = new ImageSignature(id);

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
    title: "Undirskrift með Image undirskriftum Live Demo"
    content: |
       Bættu ýmsum rafrænum undirskriftum við Xls skrá núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Eyddu Image undirskriftunum þínum með Java"
    content: |
        "Eyðing rafrænna undirskrifta sem bætt var við ýmis skjalasnið. Fjarlægðu undirskriftir fljótt án aukakóða."
    format: 
       
       
back_to_top:
    enable: true
---