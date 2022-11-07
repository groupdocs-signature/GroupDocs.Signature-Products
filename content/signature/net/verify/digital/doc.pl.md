---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Doc
productName: .NET
lang: pl
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Doc for C#

############################# Head ############################
head_title: "Weryfikacja podpisów Digital dla plików Doc przez C#"
head_description: "Użyj tylko kilku wierszy kodu .NET, aby zweryfikować dokumenty Doc i ich podpisy Digital."

############################# Header ############################
title: "Weryfikacja podpisów Digital dla plików Doc"
description: "Interfejs API dla .NET umożliwia weryfikację podpisów Digital w dokumentach Doc. Weryfikacja podpisów elektronicznych w dokumentach Doc może być przeprowadzona szybko i łatwo."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Odkryj nowe funkcje interfejsu API GroupDocs.Signature for .NET"
    content: |
        Interfejs API [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) zapewnia szeroki zakres sposobów przetwarzania wielu formatów dokumentów za pomocą podpisów elektronicznych. Obsługiwanych jest wiele rodzajów podpisów cyfrowych, takich jak teksty, obrazy, certyfikaty cyfrowe, kody kreskowe, kody QR, pieczątki lub metadane. Klienci mogą dodawać, usuwać, edytować, sprawdzać lub wyszukiwać podpisy cyfrowe w plikach PDF, dokumentach MS Word, skoroszytach MS Excel, prezentacjach MS PowerPoint, plikach Adobe Photoshop i różnych formatach graficznych. Dostępna jest zadziwiająca liczba dodatkowych funkcji i ustawień.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Jak zweryfikować podpisy Digital w dokumencie Doc?"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) zawiera przydatne funkcje, takie jak weryfikacja podpisów Digital umieszczonych w dokumentach Doc. Skorzystaj z tej możliwości bez implementowania dodatkowego kodu.
        
        * Po pierwsze, stwórz instancję klasy Signature, podając jako parametr konstruktora ścieżkę do dokumentu, który ma zostać zweryfikowany.
        * Po drugie, utwórz nowy obiekt VerifyOptions i skonfiguruj wszystkie wymagane właściwości.
        * Na koniec wywołaj metodę Verify obiektu Signature przekazując instancję VerifyOptions.
        * Następnie przetwórz wyniki weryfikacji.

    title_right: "wymagania systemowe"
    content_right: |
        GroupDocs.Signature for .NET są obsługiwane na wszystkich głównych platformach i systemach operacyjnych. Przed wykonaniem poniższego kodu upewnij się, że masz zainstalowane w systemie następujące wymagania wstępne.

        * Systemy operacyjne: Microsoft Windows, Linux, MacOS
        * Środowiska programistyczne: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Pobierz najnowszą wersję GroupDocs.Signature for .NET z [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                DigitalVerifyOptions options = new DigitalVerifyOptions()
                {
                    // Digital signature comment
                    Comments = "Approved by co-owner",
                    // specify period of signatures
                    SignDateTimeFrom = new DateTime(year: 2021, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2022, month: 12, day: 31)
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisywanie za pomocą podpisów Digital Demo na żywo"
    content: |
       Dodaj różne podpisy elektroniczne do pliku Doc już teraz, odwiedzając witrynę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Zweryfikuj inne podpisy Digital za pomocą C#"
    content: |
        "Weryfikacja podpisów elektronicznych złożonych w różnych dokumentach. Sprawdź jakość podpisów w popularnych formatach plików, jak pokazano poniżej."
    format: 
       
       
back_to_top:
    enable: true
---