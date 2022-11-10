---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Text
fileformat: Xlsx
productName: Java
lang: et
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Text signatures at Xlsx with Java

############################# Head ############################
head_title: "Otsige allkirju Text failist Xlsx rakenduses Java"
head_description: "Kasutage Java allkirjade Text otsimiseks failides Xlsx, kasutades paari koodirida."

############################# Header ############################
title: "Otsige failist Text allkirju Xlsx"
description: "Native API Java võimaldab otsida allkirju Text juba allkirjastatud Xlsx failides. Tehke oma Xlsx dokumentides täpsem e-allkirjaotsing, kasutades paari koodirida."
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
    title: "Teave toote GroupDocs.Signature for Java API kohta"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) pakub Java API-d dokumentide töötlemiseks, kasutades erinevaid allkirjatüüpe (nt tekste, pilte, digitaalseid sertifikaate, vöötkoode, QR-koode, templeid või metaandmeid). Kasutajad saavad lisada, kustutada, värskendada, kontrollida või otsida elektroonilisi allkirju PDF-failides, MS Wordi dokumentides, MS Exceli töövihikutes, MS PowerPointi esitlustes, Adobe Photoshopi failides ja erinevates pildivormingutes koos täiendava toega allkirjade atribuutide kohandamiseks vastavalt vajadusele.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Allkirjade Text otsimine failivormingus Xlsx"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) hõlbustab toote Java arendajatel allkirjade Text otsimist oma rakendustest failides Xlsx, rakendades mõnda lihtsat sammu.
        
        * Looge Signature klassi uus eksemplar ja edastage lähtedokumendi tee konstruktori parameetrina.
        * Looge otsingusuvandite objekt vastavalt oma vajadustele ja määrake otsingusuvandid.
        * Helistage Signature klassi eksemplari otsingumeetodile ja edastage sellele SearchOptions.
        * Töötle otsingutulemusi vastavalt oma nõudmistele.

    title_right: "Nõuded süsteemile"
    content_right: |
        Toodet GroupDocs.Signature for Java toetavad kõik suuremad platvormid ja operatsioonisüsteemid. Enne alloleva koodi käivitamist veenduge, et teie süsteemi on installitud järgmised eeltingimused.

        * Operatsioonisüsteemid: Microsoft Windows, Linux, MacOS
        * Arenduskeskkonnad: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Laadige alla toote GroupDocs.Signature for Java uusim versioon saidilt [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsx file
        String filePath = "input.xlsx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        TextSearchOptions options = new TextSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
                            
        // search for Text signatures in Xlsx document
        List<TextSignature> signatures = signature.search(TextSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Otsige Text elektroonilisi allkirju reaalajas demo"
    content: |
       Otsige kohe dokumendist erinevaid elektroonilisi allkirju Xlsx-failidele, külastades veebisaiti [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Otsige teisi Text allkirju, kasutades Java"
    content: |
        "Elektroonilised allkirjad otsivad erinevatest dokumentidest. Leidke allkirjad ühest populaarsest failivormingust, nagu allpool näidatud."
    format: 
           
       
back_to_top:
    enable: true
---