---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Odt
productName: Java
lang: sl
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Odt for Java

############################# Head ############################
head_title: "Dodajanje digitalnih elektronskih podpisov datoteki Odt z Java"
head_description: "Z nekaj vrsticami kode postavite digitalni podpis na datoteko Odt za Java. Uporabite API za podpis dokumentov GroupDocs za podpis na desetine formatov datotek."

############################# Header ############################
title: "Datoteke eSign Odt s podpisi Digital v Java"
description: "Kako dodati podpis Digital z nekaj vrsticami kode Java"
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
    title: "O API-ju za digitalne podpise GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) je priljubljen API za oblikovanje dokumentov z digitalnimi elektronskimi podpisi z digitalnimi potrdili. API za digitalne podpise uporablja datoteke s potrdili PFX za podpis dokumenta z zasebnimi in javnimi ključi, zaščitenimi z geslom. Digitalni podpisi se lahko uporabljajo za potrjevanje poslovnih dokumentov z določeno stranjo eSign PDF, potrjevanje celotnih dokumentov Microsoft Office, kot so Words, Excel, datoteke Powerpoint in dokumenti Open Office. Stranke lahko preprosto manipulirajo s podpisi, kot jih urejajo, odstranjujejo ali prilagajajo. API omogoča iskanje in preverjanje podpisov. Poleg tega je na voljo veliko možnosti za prilagajanje podpisov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Koraki za podpis Odt z Digital v Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) omogoča hitro in enostavno podpisovanje dokumentov Odt s podpisi Digital.
        
        * Ustvarite primerek razreda podpisa, ki zagotavlja datoteko Odt, ki naj bi se podpisala kot pot ali pomnilniški tok
        * Instanciirajte razred SignOptions in nastavite vse zahtevane podatke.
        * Prikličite metodo Signature.Sign(), ki posreduje izhodno datoteko Odt ali pomnilniški tok

    title_right: " Sistemske zahteve"
    content_right: |
        GroupDocs.Signature for Java so podprti na vseh glavnih platformah in operacijskih sistemih. Preden izvedete spodnjo kodo, se prepričajte, da imate v sistemu nameščene naslednje predpogoje.

        * Operacijski sistemi: Microsoft Windows, Linux, MacOS
        * Razvojna okolja: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Pridobite najnovejši GroupDocs.Signature for Java iz [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Odt file
        String filePath = "input.odt";
        // Set up output file
        String outputFilePath = "output.odt";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Odt document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisovanje dokumentov Odt z Digital Live Demo"
    content: |
       Takoj zdaj podpišite datoteko Odt z različnimi podpisi, tako da obiščete spletno mesto [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Brezplačna spletna predstavitev čaka na vas.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Drugi podprti podpisi Digital za Java"
    content: |
        "Odt lahko podpišete tudi z drugimi vrstami podpisov. Oglejte si spodnji seznam."
    format: 
       
       
back_to_top:
    enable: true
---