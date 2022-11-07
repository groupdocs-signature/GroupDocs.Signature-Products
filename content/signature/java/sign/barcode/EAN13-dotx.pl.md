---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: E A N13
fileformat: Dotx
productName: Java
lang: pl
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Dotx for Java

############################# Head ############################
head_title: "Podpisz dokument Dotx z kodem kreskowym E A N13 w Java"
head_description: "Utwórz podpis z kodem kreskowym E A N13 i umieść go w dokumencie Dotx za pomocą Java, używając kilku linijek kodu. Użyj interfejsu GroupDocs Document Signature API do podpisywania różnych formatów plików."

############################# Header ############################
title: "Wygeneruj E A N13 podpis z kodem kreskowym dla dokumentu Dotx w Java"
description: "ePodpisz swoje dokumenty biznesowe w Dotx za pomocą kodu kreskowego E A N13. Szybko i łatwo generuj podpis z kodem kreskowym za pomocą kilku linijek kodu, aby skonfigurować opcje podpisywania."
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
    title: "Informacje o interfejsie API podpisów kodów kreskowych GroupDocs.Signature for Java."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) to szybki i łatwy interfejs API do zarządzania elektronicznym podpisywaniem dokumentów cyfrowych przy użyciu typów kodów kreskowych, takich jak UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 i wiele innych. Klienci mogą łatwo tworzyć kody kreskowe zawierające wymagany tekst i umieszczać je w plikach PDF, dokumentach Microsoft Office Words, skoroszytach programu Microsoft Office Excel, prezentacjach MS PowerPoint, plikach Adobe Photoshop i różnych formatach graficznych. Kody kreskowe umieszczone w dokumentach mogą być aktualizowane, przeszukiwane, weryfikowane, usuwane lub przeglądane. Ponadto obsługiwane jest dostosowywanie kodów kreskowych.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroki do podpisania Dotx za pomocą Barcode w Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) umożliwia szybkie i łatwe podpisywanie dokumentów w formacie Dotx za pomocą podpisów Barcode.
        
        * Utwórz instancję klasy Signature podając plik Dotx do podpisania jako ścieżkę lub strumień pamięci
        * Utwórz wystąpienie klasy SignOptions i ustaw wszystkie wymagane dane.
        * Wywołaj metodę Signature.Sign() przekazującą wyjściowy plik Dotx lub strumień pamięci

    title_right: " wymagania systemowe"
    content_right: |
        GroupDocs.Signature for Java są obsługiwane na wszystkich głównych platformach i systemach operacyjnych. Przed wykonaniem poniższego kodu upewnij się, że masz zainstalowane w systemie następujące wymagania wstępne.

        * Systemy operacyjne: Microsoft Windows, Linux, MacOS
        * Środowiska programistyczne: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Pobierz najnowszą wersję GroupDocs.Signature for Java z [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dotx file
        String filePath = "input.dotx";
        // Set up output file
        String outputFilePath = "output.dotx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.E A N13);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Dotx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisywanie dokumentów Dotx za pomocą Barcode Demo na żywo"
    content: |
       Podpisz teraz plik Dotx różnymi podpisami, odwiedzając witrynę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Darmowe demo online czeka na Ciebie.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About E A N13 Barcode"
          content: |
            Najczęściej używanym standardem EAN jest trzynastocyfrowy kod EAN-13, nadzbiór oryginalnego 12-cyfrowego standardu Universal Product Code.
          characterset: |
             Tylko cyfry (0-9).
          textcapacity: |
             Pojemność kodu: dokładnie 12 cyfr + 1 cyfra kontrolna.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAGwAAABjCAYAAAB+MOUYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAARpSURBVHhe7ZFBimBRCMT6/pfuUYaAi6pe58MLSJCAG39+H5/iPexjvId9jPewj/Ee9jHewz7Ge9jH+PNhPz//M4bdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXh5K3sM+xnvYx3gP+xjvYR/jPexT/P7+A4FOQDtpBhIBAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Inne obsługiwane podpisy Barcode dla Java"
    content: |
        "Możesz także podpisać Dotx innymi typami podpisów. Zobacz poniższą listę."
    format: 
        
       
back_to_top:
    enable: true
---