---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Docx
productName: Java
lang: sl
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Docx with Java

############################# Head ############################
head_title: "Poiščite podpise Digital v datoteki Docx v Java"
head_description: "Uporabite Java za iskanje podpisov Digital v datotekah Docx z uporabo nekaj vrstic kode."

############################# Header ############################
title: "Poiščite podpise Digital v datoteki Docx"
description: "Izvorni API za Java omogoča iskanje podpisov Digital v že podpisanih datotekah Docx. Izvedite napredno iskanje e-podpisov znotraj svojih dokumentov Docx z uporabo nekaj vrstic kode."
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
    title_left: "Kako poiskati podpise Digital v Docx"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) razvijalcem za Java olajša iskanje podpisov Digital v datotekah Docx iz njihovih aplikacij z implementacijo nekaj preprostih korakov.
        
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
                
        // Set up input Docx file
        String filePath = "input.docx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        DigitalSearchOptions options = new DigitalSearchOptions();

        // specify special search criteria
        options.setComments("Approved");
        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2021, 3, 5));
        options.setSignDateTimeTo(new Date(2022, 7, 16));
        
        // search for Digital signatures in Docx document
        List<DigitalSignature> signatures = signature.search(DigitalSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Iskanje elektronskih podpisov Digital Predstavitev v živo"
    content: |
       Takoj zdaj poiščite v dokumentu različne elektronske podpise za datoteke Docx tako, da obiščete spletno mesto [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Išči druge Digital podpise z Java"
    content: |
        "Iskanje elektronskih podpisov v različnih dokumentih. Poiščite podpise enega od priljubljenih formatov datotek, kot je prikazano spodaj."
    format: 
           
       
back_to_top:
    enable: true
---