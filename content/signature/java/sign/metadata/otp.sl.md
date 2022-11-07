---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Otp
productName: Java
lang: sl
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Otp for Java

############################# Head ############################
head_title: "Dodajte elektronske podpise metapodatkov dokumentom Otp prek Java"
head_description: "Uporabite metapodatke kot skrite elektronske podpise znotraj svojih dokumentov Otp z nekaj vrsticami kode Java. Uporabite API za podpis dokumentov GroupDocs za e-podpisovanje poslovnih dokumentov in datotek z informacijami o metapodatkih."

############################# Header ############################
title: "Elektronski podpisi metapodatkov za dokument Otp preko Java so preprosti in enostavni za uporabo!"
description: "e-Podpišite svoje Otp dokumente in pogodbe s skritimi vnosi metapodatkov. Ustvarite metapodatke za PDF-je, dokumente MS Word, delovne zvezke MS Excel, predstavitve MS PowerPoint in različne formate slik brez težav in dodatnega kodiranja."
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
    title: "O API-ju za podpise metapodatkov GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) je priljubljen API za e-podpisovanje digitalnih dokumentov. Na voljo so podpisi, kot so besedila, slike, digitalna potrdila, črtne kode, QR-kode, žigi ali metapodatki. Podpise lahko postavite na datoteke PDF, dokumente MS Word, delovne zvezke MS Excel, predstavitve MS PowerPoint, datoteke Adobe Photoshop in različne formate slik. Stranke lahko podpišejo svoj dokument in posodabljajo, iščejo, preverjajo, brišejo ali si predogledajo e-podpise, ki so bili na teh dokumentih. Poleg tega je na voljo veliko možnosti za prilagajanje podpisov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Koraki za podpis Otp z Metadata v Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) omogoča hitro in enostavno podpisovanje dokumentov Otp s podpisi Metadata.
        
        * Ustvarite primerek razreda podpisa, ki zagotavlja datoteko Otp, ki naj bi se podpisala kot pot ali pomnilniški tok
        * Instanciirajte razred SignOptions in nastavite vse zahtevane podatke.
        * Prikličite metodo Signature.Sign(), ki posreduje izhodno datoteko Otp ali pomnilniški tok

    title_right: " Sistemske zahteve"
    content_right: |
        GroupDocs.Signature for Java so podprti na vseh glavnih platformah in operacijskih sistemih. Preden izvedete spodnjo kodo, se prepričajte, da imate v sistemu nameščene naslednje predpogoje.

        * Operacijski sistemi: Microsoft Windows, Linux, MacOS
        * Razvojna okolja: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Pridobite najnovejši GroupDocs.Signature for Java iz [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Otp file
        String filePath = "input.otp";
        // Set up output file
        String outputFilePath = "output.otp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Otp document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisovanje dokumentov Otp z Metadata Live Demo"
    content: |
       Takoj zdaj podpišite datoteko Otp z različnimi podpisi, tako da obiščete spletno mesto [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Brezplačna spletna predstavitev čaka na vas.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Drugi podprti podpisi Metadata za Java"
    content: |
        "Otp lahko podpišete tudi z drugimi vrstami podpisov. Oglejte si spodnji seznam."
    format: 
       
       
back_to_top:
    enable: true
---