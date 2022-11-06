---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Ots
productName: Java
lang: et
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ots for Java

############################# Head ############################
head_title: "Digitaalsete elektrooniliste allkirjade lisamine failile Ots rakendusega Java"
head_description: "Sisestage digitaalallkiri toote Java failile Ots, kasutades mõnda koodirida. Kasutage GroupDocs Document Signature API-t kümnete failivormingute allkirjastamiseks."

############################# Header ############################
title: "eSign Ots failid Digital allkirjaga rakenduses Java"
description: "Kuidas lisada allkirja Digital mõne reaga Java koodiga"
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
    title: "Teave GroupDocs.Signature for Java digitaalallkirjade API kohta"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) on populaarne API dokumentide allkirjastamiseks digitaalsete elektrooniliste allkirjadega ja digitaalsete sertifikaatidega. Digitaalallkirjade jaoks kasutab API parooliga kaitstud privaatsete ja avalike võtmetega dokumendi allkirjastamiseks PFX-sertifikaadi faile. Digitaalallkirju võib kasutada äridokumentide sertifitseerimiseks eSign PDF-i konkreetse lehe abil, tervete Microsoft Office'i dokumentide, näiteks Wordsi, Exceli, Powerpointi failide ja Open Office'i dokumentide sertifitseerimiseks. Kliendid saavad allkirjadega hõlpsalt manipuleerida, näiteks neid redigeerida, eemaldada või kohandada. API pakub võimalust allkirjade otsimiseks ja kinnitamiseks. Lisaks pakutakse palju allkirjade kohandamise võimalusi.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Toimingud Ots allkirjastamiseks rakendusega Digital rakenduses Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) võimaldab kiiresti ja lihtsalt allkirjastada Ots dokumente Digital allkirjaga.
        
        * Looge allkirjaklassi eksemplar, mis sisaldab faili Ots, mis peaks allkirjastama tee või mäluvoona
        * Käivitage klass SignOptions ja määrake kõik nõutavad andmed.
        * Käivitage meetod Signature.Sign(), mis edastab väljundfaili Ots või mäluvoo

    title_right: " Nõuded süsteemile"
    content_right: |
        Toodet GroupDocs.Signature for Java toetavad kõik suuremad platvormid ja operatsioonisüsteemid. Enne alloleva koodi käivitamist veenduge, et teie süsteemi on installitud järgmised eeltingimused.

        * Operatsioonisüsteemid: Microsoft Windows, Linux, MacOS
        * Arenduskeskkonnad: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Hankige uusim GroupDocs.Signature for Java kasutajalt [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ots file
        String filePath = "input.ots";
        // Set up output file
        String outputFilePath = "output.ots";
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

        // sign Ots document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dokumentide Ots allkirjastamine Digital reaalajas demoga"
    content: |
       Allkirjastage fail Ots erinevate allkirjadega kohe, külastades veebisaiti [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Tasuta online demo ootab teid.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muud toetatud Digital allkirjad Java jaoks"
    content: |
        "Saate allkirjastada faili Ots ka muude allkirjatüüpidega. Vaadake allolevat loendit."
    format: 
       
       
back_to_top:
    enable: true
---