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
lang: sl
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Dot for Java

############################# Head ############################
head_title: "eSign Dot dokument s črtno kodo Codabar v Java"
head_description: "Ustvarite podpis črtne kode Codabar in ga postavite na dokument Dot z Java z nekaj vrsticami kode. Uporabite API za podpis dokumentov GroupDocs za podpisovanje različnih formatov datotek."

############################# Header ############################
title: "Ustvari Codabar podpis črtne kode za Dot dokument v Java"
description: "e-Podpišite svoje Dot poslovne dokumente s črtno kodo Codabar. Hitro in preprosto ustvarite podpis črtne kode z nekaj vrsticami kode za nastavitev možnosti podpisovanja."
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
    title: "O API-ju za podpise črtne kode GroupDocs.Signature for Java."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) je hiter in preprost API za upravljanje e-podpisovanja digitalnih dokumentov z uporabo vrst črtne kode, kot so UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 in mnogi drugi. Stranke lahko preprosto ustvarijo črtne kode z zahtevanim besedilom in jih dodajo v PDF, dokumente Microsoft Office Words, delovne zvezke Microsoft Office Excel, predstavitve MS PowerPoint, datoteke Adobe Photoshop in različne formate slik. Črtne kode v dokumentih je mogoče posodobiti, iskati, preveriti, izbrisati ali predogledati. Poleg tega je podprto prilagajanje črtnih kod.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Koraki za podpis Dot z Barcode v Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) omogoča hitro in enostavno podpisovanje dokumentov Dot s podpisi Barcode.
        
        * Ustvarite primerek razreda podpisa, ki zagotavlja datoteko Dot, ki naj bi se podpisala kot pot ali pomnilniški tok
        * Instanciirajte razred SignOptions in nastavite vse zahtevane podatke.
        * Prikličite metodo Signature.Sign(), ki posreduje izhodno datoteko Dot ali pomnilniški tok

    title_right: " Sistemske zahteve"
    content_right: |
        GroupDocs.Signature for Java so podprti na vseh glavnih platformah in operacijskih sistemih. Preden izvedete spodnjo kodo, se prepričajte, da imate v sistemu nameščene naslednje predpogoje.

        * Operacijski sistemi: Microsoft Windows, Linux, MacOS
        * Razvojna okolja: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Pridobite najnovejši GroupDocs.Signature for Java iz [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
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
    title: "Podpisovanje dokumentov Dot z Barcode Live Demo"
    content: |
       Takoj zdaj podpišite datoteko Dot z različnimi podpisi, tako da obiščete spletno mesto [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Brezplačna spletna predstavitev čaka na vas.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar je linearna simbologija črtne kode, ki je bila zasnovana za natančno branje, tudi če je natisnjena na matričnih tiskalnikih za večdelne obrazce, kot so letalski računi FedEx in obrazci za krvne banke.
          characterset: |
             Številke (0-9) in posebni znaki $/-:+.
          textcapacity: |
             Brez posebnih omejitev.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Drugi podprti podpisi Barcode za Java"
    content: |
        "Dot lahko podpišete tudi z drugimi vrstami podpisov. Oglejte si spodnji seznam."
    format: 
        
       
back_to_top:
    enable: true
---