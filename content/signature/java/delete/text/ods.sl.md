---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Ods
productName: Java
lang: sl
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Ods for Java

############################# Head ############################
head_title: "Izbrišite podpise Text iz datotek Ods prek Java"
head_description: "Brisanje določenih podpisov Text iz podpisanih dokumentov Ods je mogoče preprosto izvesti s kratko kodo Java."

############################# Header ############################
title: "Odstranite podpise Text, ki so v datotekah Ods"
description: "Izbrišite različne podpise Text iz dokumentov Ods. Odstranjevanje podpisov Text zahteva preprosto kodo Java."
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
    title: "Pridobite informacije o funkcijah API-ja GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API ponuja številne načine za obdelavo vaših dokumentov z uporabo elektronskih podpisov. Na voljo so digitalni podpisi, kot so besedila, slike, digitalna potrdila, črtne kode, QR-kode, žigi ali metapodatki. Stranke imajo možnost dodajanja, brisanja, posodabljanja, preverjanja ali iskanja digitalnih podpisov v PDF-jih, dokumentih MS Word, delovnih zvezkih MS Excel, predstavitvah MS PowerPoint, datotekah Adobe Photoshop in različnih slikovnih formatih. Na voljo je ogromno uporabnih funkcij in nastavitev.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kako odstraniti podpise Text iz vašega dokumenta Ods"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) nudi uporabno funkcijo za čiščenje dokumentov Ods podpisov Text z nekaj vrsticami kode.
        
        * Najprej ustvarite pot podajanja predmeta podpisa do vašega dokumenta kot parameter konstruktorja.
        * Nato ustvarite ustrezen predmet podpisa in nastavite njegov enolični identifikator.
        * Po tem pokličite metodo Delete, ki posreduje predmet podpisa, ki ga je treba izbrisati.
        * Končno, procesni rezultati operacije.

    title_right: "Sistemske zahteve"
    content_right: |
        GroupDocs.Signature for Java so podprti na vseh glavnih platformah in operacijskih sistemih. Preden izvedete spodnjo kodo, se prepričajte, da imate v sistemu nameščene naslednje predpogoje.

        * Operacijski sistemi: Microsoft Windows, Linux, MacOS
        * Razvojna okolja: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Prenesite najnovejšo različico GroupDocs.Signature for Java iz [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ods file
        String filePath = "input.ods";
        // Set up output file
        String outputFilePath = "output.ods";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to delete
        TextSignature signatureToDelete = new TextSignature(id);

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
    title: "Podpisovanje s podpisi Text Demo v živo"
    content: |
       Takoj dodajte različne elektronske podpise v datoteko Ods tako, da obiščete spletno mesto [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Izbrišite svoje podpise Text z Java"
    content: |
        "Brisanje e-podpisov, ki so bili dodani v različne formate dokumentov. Hitro odstranite podpise brez dodatne kode."
    format: 
       
       
back_to_top:
    enable: true
---