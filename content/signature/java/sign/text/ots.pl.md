---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Ots
productName: Java
lang: pl
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Ots for Java

############################# Head ############################
head_title: "Utwórz tekstowe podpisy elektroniczne do pliku Ots za pomocą Java"
head_description: "Umieść Text eSignature w pliku Ots dla Java, używając kilku linijek kodu. Użyj interfejsu GroupDocs Document Signature API, aby podpisać dziesiątki formatów plików."

############################# Header ############################
title: "Podpisz pliki Ots z podpisami Text w Java"
description: "Jak dodać podpis Text z kilkoma linijkami kodu Java?"
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
    title: "Informacje o interfejsie API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) to popularny interfejs API do elektronicznego podpisywania dokumentów. Dostępne są podpisy, takie jak teksty, obrazy, certyfikaty cyfrowe, kody kreskowe, kody QR, pieczątki lub metadane. Podpisy mogą być umieszczane na plikach PDF, dokumentach MS Word, skoroszytach MS Excel, prezentacjach MS PowerPoint, plikach Adobe Photoshop i różnych formatach graficznych. Klienci mogą podpisywać swoje dokumenty i aktualizować, wyszukiwać, weryfikować, usuwać lub przeglądać podpisy elektroniczne, które zostały umieszczone na tych dokumentach. Ponadto zapewniono wiele możliwości dostosowywania podpisów.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroki do podpisania Ots za pomocą Text w Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) umożliwia szybkie i łatwe podpisywanie dokumentów w formacie Ots za pomocą podpisów Text.
        
        * Utwórz instancję klasy Signature podając plik Ots do podpisania jako ścieżkę lub strumień pamięci
        * Utwórz wystąpienie klasy SignOptions i ustaw wszystkie wymagane dane.
        * Wywołaj metodę Signature.Sign() przekazującą wyjściowy plik Ots lub strumień pamięci

    title_right: " wymagania systemowe"
    content_right: |
        GroupDocs.Signature for Java są obsługiwane na wszystkich głównych platformach i systemach operacyjnych. Przed wykonaniem poniższego kodu upewnij się, że masz zainstalowane w systemie następujące wymagania wstępne.

        * Systemy operacyjne: Microsoft Windows, Linux, MacOS
        * Środowiska programistyczne: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Pobierz najnowszą wersję GroupDocs.Signature for Java z [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ots file
        String filePath = "input.ots";
        // Set up output file
        String outputFilePath = "output.ots";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Ots document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisywanie dokumentów Ots za pomocą Text Demo na żywo"
    content: |
       Podpisz teraz plik Ots różnymi podpisami, odwiedzając witrynę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Darmowe demo online czeka na Ciebie.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Inne obsługiwane podpisy Text dla Java"
    content: |
        "Możesz także podpisać Ots innymi typami podpisów. Zobacz poniższą listę."
    format: 
       
       
back_to_top:
    enable: true
---