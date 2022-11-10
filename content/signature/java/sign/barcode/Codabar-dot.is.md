---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Dot
productName: Java
lang: is
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Dot for Java

############################# Head ############################
head_title: "eSign Dot skjal með Codabar Strikamerki í Java"
head_description: "Búðu til Codabar Strikamerki undirskrift og settu hana á Dot skjal með Java með því að nota nokkrar línur af kóða. Notaðu GroupDocs Document Signature API til að undirrita ýmis skráarsnið."

############################# Header ############################
title: "Búðu til Codabar Strikamerki undirskrift fyrir Dot skjal í Java"
description: "eSignaðu Dot viðskiptaskjölin þín með Codabar Strikamerki. Búðu til Strikamerki undirskrift fljótt og auðveldlega með nokkrum línum af kóða til að setja upp undirskriftarmöguleika."
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
    title_left: "Skref til að undirrita Dot með Barcode í Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) veitir möguleika á að undirrita Dot skjöl með Barcode undirskrift fljótt og auðveldlega.
        
        * Búðu til tilvik af Signature class sem gefur upp Dot skrá sem á að undirrita sem slóð eða minnisstraum
        * Upphafðu SignOptions flokkinn og stilltu öll umbeðin gögn.
        * Kallaðu á Signature.Sign() aðferðina sem sendir úttak Dot skrá eða minnisstraum

    title_right: " kerfis kröfur"
    content_right: |
        GroupDocs.Signature for Java eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.

        * Stýrikerfi: Microsoft Windows, Linux, MacOS
        * Þróunarumhverfi: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Fáðu nýjasta GroupDocs.Signature for Java frá [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dot file
        String filePath = "input.dot";
        // Set up output file
        String outputFilePath = "output.dot";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Codabar);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Dot document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Undirritar Dot skjöl með Barcode lifandi kynningu"
    content: |
       Skrifaðu undir Dot skrána með ýmsum undirskriftum núna með því að fara á [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) vefsíðuna. Ókeypis kynning á netinu bíður þín.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar er línuleg strikamerki táknfræði sem var hönnuð til að vera nákvæmlega lesin, jafnvel þegar þau eru prentuð á punktafylkisprentara fyrir fjölþætt eyðublöð eins og FedEx flugseðla og blóðbankaform.
          characterset: |
             Tölustafir (0-9) og sérstafir $/-:+.
          textcapacity: |
             Engar sérstakar takmarkanir.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aðrar studdar Barcode undirskriftir fyrir Java"
    content: |
        "Þú getur líka skrifað undir Dot með öðrum undirskriftartegundum. Vinsamlegast skoðaðu listann hér að neðan."
    format: 
        
       
back_to_top:
    enable: true
---