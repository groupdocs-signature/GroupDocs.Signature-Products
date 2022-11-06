---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Xls
productName: Java
lang: et
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Xls for Java

############################# Head ############################
head_title: "Värskendage Text allkirja, mis on pandud failidesse Xls rakendusega Java"
head_description: "Kasutage allkirjastatud Xls dokumentides allkirjade Text värskendamiseks lihtsat ja hõlpsasti mõistetavat Java koodi."

############################# Header ############################
title: "Muutke ja värskendage failidesse Xls pandud allkirju Text"
description: "API for Java pakub funktsiooni Text allkirjade värskendamiseks dokumentides Xls. Värskendage oma Xls dokumentides olevaid e-allkirju paari rea koodiga Java kiiresti ja lihtsalt."
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
    title: "Lisateave toote GroupDocs.Signature for Java API funktsioonide kohta"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API-funktsioonid sisaldavad laia valikut vahendeid nõutavate dokumentide vormingute töötlemiseks elektrooniliste allkirjade abil. Toetatud on lai valik e-allkirju, nagu tekstid, pildid, digitaalsed sertifikaadid, vöötkoodid, QR-koodid, templid või metaandmed. Kliendid saavad lisada, eemaldada, redigeerida, kinnitada või otsida digitaalallkirju PDF-ides, MS Wordi dokumentides, MS Exceli töövihikutes, MS PowerPointi esitlustes, Adobe Photoshopi failides ja erinevates pildivormingutes. Saadaval on palju kasulikke funktsioone ja seadeid.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kuidas muuta allkirja Text oma dokumendis Xls"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) sisaldab kasulikke funktsioone, nagu Text allkirjade värskendamine, mis on paigutatud dokumentidele Xls. See võimaldab muuta allkirjafunktsioone ilma lisakoodita.
        
        * Alustuseks looge allkirjaobjekt, mis edastab konstruktori parameetri teena dokumendile, mida peaks värskendama.
        * Seejärel looge sobiv konkreetne allkirjaobjekt ja seadistage selle identifikaator ja atribuudid, mida tuleb muuta.
        * Lõpuks helistage Signature's Update meetodile, edastades konkreetse allkirjaobjekti.
        * Töötlege tulemuste värskendamist teie teate järgi.

    title_right: "Nõuded süsteemile"
    content_right: |
        Toodet GroupDocs.Signature for Java toetavad kõik suuremad platvormid ja operatsioonisüsteemid. Enne alloleva koodi käivitamist veenduge, et teie süsteemi on installitud järgmised eeltingimused.

        * Operatsioonisüsteemid: Microsoft Windows, Linux, MacOS
        * Arenduskeskkonnad: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Laadige alla toote GroupDocs.Signature for Java uusim versioon saidilt [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xls file
        String filePath = "input.xls";
        // Set up output file
        String outputFilePath = "output.xls";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to update
        // set up particular signature id
        TextSignature signatureToUpdate = new TextSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(130);
        // specify signature height
        signatureToUpdate.setHeight(20);
        // set left position
        signatureToUpdate.setLeft(40);
        // set top position
        signatureToUpdate.setTop(50);
        // set up new text
        signatureToUpdate.setText("Mr. John Smith");

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Allkirjade Text värskendamine dokumendilehtedel – reaalajas demo"
    content: |
       Saate kohe redigeerida dokumendi Xls erinevaid elektroonilisi allkirju, külastades veebisaiti [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Värskendage Text allkirju Java kaudu"
    content: |
        "Erinevatesse dokumendivormingutesse paigutatud digitaalallkirjade redigeerimine. Uuendage allkirjaandmeid ilma lisakoodita."
    format: 
       
       
back_to_top:
    enable: true
---