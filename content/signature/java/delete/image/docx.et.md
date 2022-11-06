---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Docx
productName: Java
lang: et
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Docx for Java

############################# Head ############################
head_title: "Kustutage Image allkirjad failist Docx läbi Java"
head_description: "Konkreetsete Image allkirjade kustutamine allkirjastatud Docx dokumentidest saab hõlpsasti teostada lühikese Java koodiga."

############################# Header ############################
title: "Eemaldage allkirjad Image, mis on paigutatud failidesse Docx"
description: "Kustutage erinevad allkirjad Image dokumentidest Docx. Allkirjade Image eemaldamine nõuab lihtsat Java koodi."
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
    title: "Hankige teavet toote GroupDocs.Signature for Java API funktsioonide kohta"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API pakub palju võimalusi dokumentide töötlemiseks elektrooniliste allkirjade abil. Saadaval on digitaalallkirjad, nagu tekstid, pildid, digitaalsed sertifikaadid, vöötkoodid, QR-koodid, templid või metaandmed. Klientidel on võimalus lisada, kustutada, uuendada, kontrollida või otsida digiallkirju PDF-idest, MS Wordi dokumentidest, MS Exceli töövihikutest, MS PowerPointi esitlustest, Adobe Photoshopi failidest ja erinevatest pildivormingutest. Saadaval on suur hulk kasulikke funktsioone ja sätteid.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kuidas eemaldada allkirjad Image oma dokumendist Docx"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) pakub kasulikku funktsiooni Docx dokumentide Image allkirjade eemaldamiseks mõne koodireaga.
        
        * Esiteks looge signatuuriobjekt, mis edastab konstruktori parameetrina teie dokumendi tee.
        * Seejärel looge sobiv allkirjaobjekt ja seadistage selle kordumatu identifikaator.
        * Pärast seda käivitage kustutamismeetod, mis edastab allkirjaobjekti, mis tuleb kustutada.
        * Lõpuks protsessi toimimise tulemused.

    title_right: "Nõuded süsteemile"
    content_right: |
        Toodet GroupDocs.Signature for Java toetavad kõik suuremad platvormid ja operatsioonisüsteemid. Enne alloleva koodi käivitamist veenduge, et teie süsteemi on installitud järgmised eeltingimused.

        * Operatsioonisüsteemid: Microsoft Windows, Linux, MacOS
        * Arenduskeskkonnad: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Laadige alla toote GroupDocs.Signature for Java uusim versioon saidilt [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Docx file
        String filePath = "input.docx";
        // Set up output file
        String outputFilePath = "output.docx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "e3ad0ec7-9abf-426d-b9aa-b3328f3f1470";

        // provide signature features to delete
        ImageSignature signatureToDelete = new ImageSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Allkirjastamine Image allkirjaga Live Demo"
    content: |
       Lisage kohe failile Docx erinevad elektroonilised allkirjad, külastades veebisaiti [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Kustutage oma allkirjad Image rakendusega Java"
    content: |
        "Erinevatele dokumendivormingutele lisatud e-allkirjade kustutamine. Eemaldage allkirjad kiiresti ilma lisakoodita."
    format: 
       
       
back_to_top:
    enable: true
---