---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Otp
productName: Java
lang: is
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Otp with Java

############################# Head ############################
head_title: "Leitaðu að Qrcode undirskriftum í Otp skrá í Java"
head_description: "Notaðu Java til að leita að Qrcode undirskriftum í Otp skrám með því að nota nokkrar línur af kóða."

############################# Header ############################
title: "Leitaðu að Qrcode undirskriftum í Otp skrá"
description: "Innbyggt forritaskil Java gerir kleift að leita að Qrcode undirskriftum í þegar undirrituðum Otp skrám. Framkvæmdu háþróaða leit með rafrænum undirskriftum í Otp skjölunum þínum með því að nota nokkrar línur af kóða."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Um GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) býður upp á Java API til að vinna úr skjölum með því að nota ýmsar undirskriftargerðir eins og texta, myndir, stafræn skilríki, strikamerki, QR-kóða, stimpla eða lýsigögn. Notendur geta bætt við, eytt, uppfært, staðfest eða leitað í rafrænum undirskriftum í PDF-skjölum, MS Word skjölum, MS Excel vinnubókum, MS PowerPoint kynningum, Adobe Photoshop skrám og ýmsum myndsniðum, með viðbótarstuðningi við að sérsníða eiginleika undirskrifta eftir þörfum.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hvernig á að leita að Qrcode undirskriftum í Otp"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) auðveldar forriturum Java að leita að Qrcode undirskriftum í Otp skrám úr forritum sínum með því að útfæra nokkur einföld skref.
        
        * Búðu til nýtt tilvik af Signature class og sendu frumskjalsslóð sem byggingarbreytu.
        * Stofnaðu SearchOptions hlutinn í samræmi við kröfur þínar og tilgreindu leitarmöguleika.
        * Hringdu í leitaraðferð fyrir undirskriftarflokkstilvik og sendu SearchOptions til þess.
        * Vinndu leitarniðurstöður í samræmi við kröfur þínar.

    title_right: "kerfis kröfur"
    content_right: |
        GroupDocs.Signature for Java eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Sæktu nýjustu útgáfuna af GroupDocs.Signature for Java frá [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Otp file
        String filePath = "input.otp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        QrCodeSearchOptions options = new QrCodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Qrcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Qrcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Qrcode signatures in Otp document
        List<QrCodeSignature> signatures = signature.search(QrCodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Leitaðu að Qrcode rafrænum undirskriftum Live Demo"
    content: |
       Leitaðu í skjalinu að ýmsum rafrænum undirskriftum í Otp skrár núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Leitaðu að öðrum Qrcode undirskriftum með því að nota Java"
    content: |
        "Rafrænar undirskriftir leita í ýmsum skjölum. Finndu undirskriftir frá einu af vinsælustu skráarsniðunum eins og sýnt er hér að neðan."
    format: 
           
       
back_to_top:
    enable: true
---