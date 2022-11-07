---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Jpg
productName: Java
lang: sl
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Jpg with Java

############################# Head ############################
head_title: "Poiščite podpise Qrcode v datoteki Jpg v Java"
head_description: "Uporabite Java za iskanje podpisov Qrcode v datotekah Jpg z uporabo nekaj vrstic kode."

############################# Header ############################
title: "Poiščite podpise Qrcode v datoteki Jpg"
description: "Izvorni API za Java omogoča iskanje podpisov Qrcode v že podpisanih datotekah Jpg. Izvedite napredno iskanje e-podpisov znotraj svojih dokumentov Jpg z uporabo nekaj vrstic kode."
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
    title: "O API-ju GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ponuja API za Java za obdelavo dokumentov z uporabo različnih vrst podpisov, kot so besedila, slike, digitalna potrdila, črtne kode, kode QR, žigi ali metapodatki. Uporabniki lahko dodajajo, brišejo, posodabljajo, preverjajo ali iščejo elektronske podpise v datotekah PDF, dokumentih MS Word, delovnih zvezkih MS Excel, predstavitvah MS PowerPoint, datotekah Adobe Photoshop in različnih formatih slik, z dodatno podporo za prilagajanje lastnosti podpisov po potrebi.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kako poiskati podpise Qrcode v Jpg"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) razvijalcem za Java olajša iskanje podpisov Qrcode v datotekah Jpg iz njihovih aplikacij z implementacijo nekaj preprostih korakov.
        
        * Ustvarite nov primerek razreda Signature in podajte pot izvornega dokumenta kot parameter konstruktorja.
        * Instanciirajte objekt SearchOptions v skladu z vašimi zahtevami in določite možnosti iskanja.
        * Pokličite metodo Search instance razreda Signature in ji posredujte SearchOptions.
        * Rezultate iskanja obdelajte v skladu z vašimi zahtevami.

    title_right: "Sistemske zahteve"
    content_right: |
        GroupDocs.Signature for Java so podprti na vseh glavnih platformah in operacijskih sistemih. Preden izvedete spodnjo kodo, se prepričajte, da imate v sistemu nameščene naslednje predpogoje.

        * Operacijski sistemi: Microsoft Windows, Linux, MacOS
        * Razvojna okolja: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Prenesite najnovejšo različico GroupDocs.Signature for Java iz [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Jpg file
        String filePath = "input.jpg";

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
                            
        // search for Qrcode signatures in Jpg document
        List<QrCodeSignature> signatures = signature.search(QrCodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Iskanje elektronskih podpisov Qrcode Predstavitev v živo"
    content: |
       Takoj zdaj poiščite v dokumentu različne elektronske podpise za datoteke Jpg tako, da obiščete spletno mesto [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Išči druge Qrcode podpise z Java"
    content: |
        "Iskanje elektronskih podpisov v različnih dokumentih. Poiščite podpise enega od priljubljenih formatov datotek, kot je prikazano spodaj."
    format: 
           
       
back_to_top:
    enable: true
---