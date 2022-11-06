---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: ISBN
fileformat: Ods
productName: Java
lang: is
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Ods for Java

############################# Head ############################
head_title: "eSign Ods skjal með ISBN Strikamerki í Java"
head_description: "Búðu til ISBN Strikamerki undirskrift og settu hana á Ods skjal með Java með því að nota nokkrar línur af kóða. Notaðu GroupDocs Document Signature API til að undirrita ýmis skráarsnið."

############################# Header ############################
title: "Búðu til ISBN Strikamerki undirskrift fyrir Ods skjal í Java"
description: "eSignaðu Ods viðskiptaskjölin þín með ISBN Strikamerki. Búðu til Strikamerki undirskrift fljótt og auðveldlega með nokkrum línum af kóða til að setja upp undirskriftarmöguleika."
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
    title_left: "Skref til að undirrita Ods með Barcode í Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) veitir möguleika á að undirrita Ods skjöl með Barcode undirskrift fljótt og auðveldlega.
        
        * Búðu til tilvik af Signature class sem gefur upp Ods skrá sem á að undirrita sem slóð eða minnisstraum
        * Upphafðu SignOptions flokkinn og stilltu öll umbeðin gögn.
        * Kallaðu á Signature.Sign() aðferðina sem sendir úttak Ods skrá eða minnisstraum

    title_right: " kerfis kröfur"
    content_right: |
        GroupDocs.Signature for Java eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Fáðu nýjasta GroupDocs.Signature for Java frá [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ods file
        String filePath = "input.ods";
        // Set up output file
        String outputFilePath = "output.ods";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.ISBN);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Ods document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Undirritar Ods skjöl með Barcode lifandi kynningu"
    content: |
       Skrifaðu undir Ods skrána með ýmsum undirskriftum núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna. Ókeypis kynning á netinu bíður þín.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About ISBN Barcode"
          content: |
            Alþjóðlega staðlaða bókanúmerið (ISBN) er tölulegt auðkenni auglýsingabóka sem ætlað er að vera einstakt.[a][b] Útgefendur kaupa ISBN-númer frá hlutdeildarfélagi Alþjóða ISBN-stofnunarinnar.
          characterset: |
             Tölustafir (0-9).
          textcapacity: |
             Nákvæmlega 9 tölustafir + 1 gátstafur.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aðrar studdar Barcode undirskriftir fyrir Java"
    content: |
        "Þú getur líka skrifað undir Ods með öðrum undirskriftartegundum. Vinsamlegast skoðaðu listann hér að neðan."
    format: 
        
       
back_to_top:
    enable: true
---