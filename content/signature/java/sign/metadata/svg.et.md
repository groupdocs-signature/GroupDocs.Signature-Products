---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Svg
productName: Java
lang: et
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Svg for Java

############################# Head ############################
head_title: "Lisage metaandmete elektroonilised allkirjad Svg dokumentidele Java kaudu"
head_description: "Kasutage metaandmeid peidetud elektrooniliste allkirjadena oma Svg dokumentides, kasutades paari rida Java koodi. Kasutage GroupDocs Document Signature API-t, et oma äridokumente ja -faile metaandmetega e-allkirjastada."

############################# Header ############################
title: "Dokumendi Svg metaandmete elektroonilised allkirjad toote Java kaudu on lihtsad ja hõlpsasti kasutatavad!"
description: "eAllkirjasta oma Svg dokumendid ja lepingud peidetud metaandmete kirjetega. Genereerige metaandmeid PDF-ide, MS Wordi dokumentide, MS Exceli töövihikute, MS PowerPointi esitluste ja erinevate pildivormingute jaoks ilma probleemide ja täiendava kodeerimiseta."
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
    title: "Teave GroupDocs.Signature for Java metaandmete allkirjade API kohta"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) on populaarne API digitaalsete dokumentide e-allkirjastamiseks. Saadaval on allkirjad, nagu tekstid, pildid, digitaalsed sertifikaadid, vöötkoodid, QR-koodid, templid või metaandmed. Allkirju võib panna PDF-idele, MS Wordi dokumentidele, MS Exceli töövihikutele, MS PowerPointi esitlustele, Adobe Photoshopi failidele ja erinevatele pildivormingutele. Kliendid saavad oma dokumenti allkirjastada ning uuendada, otsida, kontrollida, kustutada või vaadata nendele dokumentidele pandud e-allkirju. Lisaks pakutakse palju allkirjade kohandamise võimalusi.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Toimingud Svg allkirjastamiseks rakendusega Metadata rakenduses Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) võimaldab kiiresti ja lihtsalt allkirjastada Svg dokumente Metadata allkirjaga.
        
        * Looge allkirjaklassi eksemplar, mis sisaldab faili Svg, mis peaks allkirjastama tee või mäluvoona
        * Käivitage klass SignOptions ja määrake kõik nõutavad andmed.
        * Käivitage meetod Signature.Sign(), mis edastab väljundfaili Svg või mäluvoo

    title_right: " Nõuded süsteemile"
    content_right: |
        Toodet GroupDocs.Signature for Java toetavad kõik suuremad platvormid ja operatsioonisüsteemid. Enne alloleva koodi käivitamist veenduge, et teie süsteemi on installitud järgmised eeltingimused.

        * Operatsioonisüsteemid: Microsoft Windows, Linux, MacOS
        * Arenduskeskkonnad: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Hankige uusim GroupDocs.Signature for Java kasutajalt [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Svg file
        String filePath = "input.svg";
        // Set up output file
        String outputFilePath = "output.svg";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Svg document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentide Svg allkirjastamine Metadata reaalajas demoga"
    content: |
       Allkirjastage fail Svg erinevate allkirjadega kohe, külastades veebisaiti [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Tasuta online demo ootab teid.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muud toetatud Metadata allkirjad Java jaoks"
    content: |
        "Saate allkirjastada faili Svg ka muude allkirjatüüpidega. Vaadake allolevat loendit."
    format: 
       
       
back_to_top:
    enable: true
---