---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Zip
productName: Java
lang: pl
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Zip for Java

############################# Head ############################
head_title: "Weryfikacja podpisów Digital dla plików Zip przez Java"
head_description: "Użyj tylko kilku wierszy kodu Java, aby zweryfikować dokumenty Zip i ich podpisy Digital."

############################# Header ############################
title: "Weryfikacja podpisów Digital dla plików Zip"
description: "Interfejs API dla Java umożliwia weryfikację podpisów Digital w dokumentach Zip. Weryfikacja podpisów elektronicznych w dokumentach Zip może być przeprowadzona szybko i łatwo."
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
    title: "Odkryj nowe funkcje interfejsu API GroupDocs.Signature for Java"
    content: |
        Interfejs API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) zapewnia szeroki zakres sposobów przetwarzania wielu formatów dokumentów za pomocą podpisów elektronicznych. Obsługiwanych jest wiele rodzajów podpisów cyfrowych, takich jak teksty, obrazy, certyfikaty cyfrowe, kody kreskowe, kody QR, pieczątki lub metadane. Klienci mogą dodawać, usuwać, edytować, sprawdzać lub wyszukiwać podpisy cyfrowe w plikach PDF, dokumentach MS Word, skoroszytach MS Excel, prezentacjach MS PowerPoint, plikach Adobe Photoshop i różnych formatach graficznych. Dostępna jest zadziwiająca liczba dodatkowych funkcji i ustawień.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Jak zweryfikować podpisy Digital w dokumencie Zip?"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) zawiera przydatne funkcje, takie jak weryfikacja podpisów Digital umieszczonych w dokumentach Zip. Skorzystaj z tej możliwości bez implementowania dodatkowego kodu.
        
        * Po pierwsze, stwórz instancję klasy Signature, podając jako parametr konstruktora ścieżkę do dokumentu, który ma zostać zweryfikowany.
        * Po drugie, utwórz nowy obiekt VerifyOptions i skonfiguruj wszystkie wymagane właściwości.
        * Na koniec wywołaj metodę Verify obiektu Signature przekazując instancję VerifyOptions.
        * Następnie przetwórz wyniki weryfikacji.

    title_right: "wymagania systemowe"
    content_right: |
        GroupDocs.Signature for Java są obsługiwane na wszystkich głównych platformach i systemach operacyjnych. Przed wykonaniem poniższego kodu upewnij się, że masz zainstalowane w systemie następujące wymagania wstępne.

        * Systemy operacyjne: Microsoft Windows, Linux, MacOS
        * Środowiska programistyczne: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Pobierz najnowszą wersję GroupDocs.Signature for Java z [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Zip file
        String filePath = "input.zip";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2020, 12, 12));
        options.setSignDateTimeTo(new Date(2022, 12, 12));
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisywanie za pomocą podpisów Digital Demo na żywo"
    content: |
       Dodaj różne podpisy elektroniczne do pliku Zip już teraz, odwiedzając witrynę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Zweryfikuj inne podpisy Digital za pomocą Java"
    content: |
        "Weryfikacja podpisów elektronicznych złożonych w różnych dokumentach. Sprawdź jakość podpisów w popularnych formatach plików, jak pokazano poniżej."
    format: 
       
       
back_to_top:
    enable: true
---