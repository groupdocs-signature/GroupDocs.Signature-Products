---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Code39
fileformat: Pptm
productName: Java
lang: is
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Pptm for Java

############################# Head ############################
head_title: "eSign Pptm skjal með Code39 Strikamerki í Java"
head_description: "Búðu til Code39 Strikamerki undirskrift og settu hana á Pptm skjal með Java með því að nota nokkrar línur af kóða. Notaðu GroupDocs Document Signature API til að undirrita ýmis skráarsnið."

############################# Header ############################
title: "Búðu til Code39 Strikamerki undirskrift fyrir Pptm skjal í Java"
description: "eSignaðu Pptm viðskiptaskjölin þín með Code39 Strikamerki. Búðu til Strikamerki undirskrift fljótt og auðveldlega með nokkrum línum af kóða til að setja upp undirskriftarmöguleika."
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
    title: "Um GroupDocs.Signature for Java Strikamerki undirskriftarforritaskil."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) er fljótlegt og auðvelt forritaskil til að stjórna rafrænni undirskrift skjala með því að nota Strikamerki eins og UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 og margir aðrir. Viðskiptavinir geta auðveldlega búið til Strikamerki með nauðsynlegum texta og sett þá á PDF, Microsoft Office Words Documents, Microsoft Office Excel vinnubækur, MS PowerPoint kynningar, Adobe Photoshop skrár og ýmis myndsnið. Strikamerki sem sett eru í skjöl er hægt að uppfæra, leita, staðfesta, eyða eða forskoða annað hvort. Þar að auki er aðlögun strikamerkja studd.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Skref til að undirrita Pptm með Barcode í Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) veitir möguleika á að undirrita Pptm skjöl með Barcode undirskrift fljótt og auðveldlega.
        
        * Búðu til tilvik af Signature class sem gefur upp Pptm skrá sem á að undirrita sem slóð eða minnisstraum
        * Upphafðu SignOptions flokkinn og stilltu öll umbeðin gögn.
        * Kallaðu á Signature.Sign() aðferðina sem sendir úttak Pptm skrá eða minnisstraum

    title_right: " kerfis kröfur"
    content_right: |
        GroupDocs.Signature for Java eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Fáðu nýjasta GroupDocs.Signature for Java frá [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pptm file
        String filePath = "input.pptm";
        // Set up output file
        String outputFilePath = "output.pptm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Code39);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Pptm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Undirritar Pptm skjöl með Barcode lifandi kynningu"
    content: |
       Skrifaðu undir Pptm skrána með ýmsum undirskriftum núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna. Ókeypis kynning á netinu bíður þín.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Code39 Barcode"
          content: |
            Kóði 39 (einnig þekktur sem Alpha39, Kóði 3 af 9, Kóði 3/9, Tegund 39, USS Kóði 39, eða USD-3) er breytileg lengd, staka strikamerkjamerki.
          characterset: |
             Tölustafir (0-9) og hástafir (A-Z) og fjöldi sérstafa (-, ., $, /, +, % og bil).
          textcapacity: |
             Engar sérstakar takmarkanir.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aðrar studdar Barcode undirskriftir fyrir Java"
    content: |
        "Þú getur líka skrifað undir Pptm með öðrum undirskriftartegundum. Vinsamlegast skoðaðu listann hér að neðan."
    format: 
        
       
back_to_top:
    enable: true
---