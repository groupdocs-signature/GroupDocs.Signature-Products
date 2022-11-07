---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Png
productName: Java
lang: pl
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Png for Java

############################# Head ############################
head_title: "Dołącz podpisy elektroniczne metadanych do dokumentów Png za pośrednictwem Java"
head_description: "Użyj metadanych jako ukrytych podpisów elektronicznych w swoich dokumentach Png, używając kilku wierszy kodu Java. Użyj interfejsu GroupDocs Document Signature API do elektronicznego podpisywania dokumentów biznesowych i plików za pomocą informacji metadanych."

############################# Header ############################
title: "Elektroniczne podpisy metadanych dla dokumentu Png za pośrednictwem Java są proste i łatwe w użyciu!"
description: "Podpisz elektronicznie dokumenty i umowy Png z ukrytymi wpisami metadanych. Generuj metadane dla plików PDF, dokumentów MS Word, skoroszytów MS Excel, prezentacji MS PowerPoint i różnych formatów obrazów bez problemów i dodatkowego kodowania."
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
    title: "Informacje o interfejsie API sygnatur metadanych GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) to popularny interfejs API do elektronicznego podpisywania dokumentów. Dostępne są podpisy, takie jak teksty, obrazy, certyfikaty cyfrowe, kody kreskowe, kody QR, pieczątki lub metadane. Podpisy mogą być umieszczane na plikach PDF, dokumentach MS Word, skoroszytach MS Excel, prezentacjach MS PowerPoint, plikach Adobe Photoshop i różnych formatach graficznych. Klienci mogą podpisywać swoje dokumenty i aktualizować, wyszukiwać, weryfikować, usuwać lub przeglądać podpisy elektroniczne, które zostały umieszczone na tych dokumentach. Ponadto zapewniono wiele możliwości dostosowywania podpisów.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroki do podpisania Png za pomocą Metadata w Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) umożliwia szybkie i łatwe podpisywanie dokumentów w formacie Png za pomocą podpisów Metadata.
        
        * Utwórz instancję klasy Signature podając plik Png do podpisania jako ścieżkę lub strumień pamięci
        * Utwórz wystąpienie klasy SignOptions i ustaw wszystkie wymagane dane.
        * Wywołaj metodę Signature.Sign() przekazującą wyjściowy plik Png lub strumień pamięci

    title_right: " wymagania systemowe"
    content_right: |
        GroupDocs.Signature for Java są obsługiwane na wszystkich głównych platformach i systemach operacyjnych. Przed wykonaniem poniższego kodu upewnij się, że masz zainstalowane w systemie następujące wymagania wstępne.

        * Systemy operacyjne: Microsoft Windows, Linux, MacOS
        * Środowiska programistyczne: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Pobierz najnowszą wersję GroupDocs.Signature for Java z [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Png file
        String filePath = "input.png";
        // Set up output file
        String outputFilePath = "output.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Png document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisywanie dokumentów Png za pomocą Metadata Demo na żywo"
    content: |
       Podpisz teraz plik Png różnymi podpisami, odwiedzając witrynę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Darmowe demo online czeka na Ciebie.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Inne obsługiwane podpisy Metadata dla Java"
    content: |
        "Możesz także podpisać Png innymi typami podpisów. Zobacz poniższą listę."
    format: 
       
       
back_to_top:
    enable: true
---