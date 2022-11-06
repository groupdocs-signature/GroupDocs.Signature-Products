---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Xltx
productName: Java
lang: et
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Xltx for Java

############################# Head ############################
head_title: "Lisage metaandmete elektroonilised allkirjad Xltx dokumentidele Java kaudu"
head_description: "Kasutage metaandmeid peidetud elektrooniliste allkirjadena oma Xltx dokumentides, kasutades paari rida Java koodi. Kasutage GroupDocs Document Signature API-t, et oma äridokumente ja -faile metaandmetega e-allkirjastada."

############################# Header ############################
title: "Dokumendi Xltx metaandmete elektroonilised allkirjad toote Java kaudu on lihtsad ja hõlpsasti kasutatavad!"
description: "eAllkirjasta oma Xltx dokumendid ja lepingud peidetud metaandmete kirjetega. Genereerige metaandmeid PDF-ide, MS Wordi dokumentide, MS Exceli töövihikute, MS PowerPointi esitluste ja erinevate pildivormingute jaoks ilma probleemide ja täiendava kodeerimiseta."
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
    title_left: "Toimingud Xltx allkirjastamiseks rakendusega Metadata rakenduses Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) võimaldab kiiresti ja lihtsalt allkirjastada Xltx dokumente Metadata allkirjaga.
        
        * Looge allkirjaklassi eksemplar, mis sisaldab faili Xltx, mis peaks allkirjastama tee või mäluvoona
        * Käivitage klass SignOptions ja määrake kõik nõutavad andmed.
        * Käivitage meetod Signature.Sign(), mis edastab väljundfaili Xltx või mäluvoo

    title_right: " Nõuded süsteemile"
    content_right: |
        Toodet GroupDocs.Signature for Java toetavad kõik suuremad platvormid ja operatsioonisüsteemid. Enne alloleva koodi käivitamist veenduge, et teie süsteemi on installitud järgmised eeltingimused.

        * Operatsioonisüsteemid: Microsoft Windows, Linux, MacOS
        * Arenduskeskkonnad: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Hankige uusim GroupDocs.Signature for Java kasutajalt [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xltx file
        String filePath = "input.xltx";
        // Set up output file
        String outputFilePath = "output.xltx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Xltx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentide Xltx allkirjastamine Metadata reaalajas demoga"
    content: |
       Allkirjastage fail Xltx erinevate allkirjadega kohe, külastades veebisaiti [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Tasuta online demo ootab teid.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muud toetatud Metadata allkirjad Java jaoks"
    content: |
        "Saate allkirjastada faili Xltx ka muude allkirjatüüpidega. Vaadake allolevat loendit."
    format: 
       
       
back_to_top:
    enable: true
---