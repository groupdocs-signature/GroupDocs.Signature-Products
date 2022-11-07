---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Csv
productName: .NET
lang: pl
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Csv for C#

############################# Head ############################
head_title: "Dodawanie podpisów Image do pliku Csv za pomocą C#"
head_description: "Umieść podpis Image w pliku Csv dla .NET, używając kilku linijek kodu. Użyj interfejsu GroupDocs Document Signature API, aby podpisać dziesiątki formatów plików."

############################# Header ############################
title: "Podpisz pliki Csv z podpisami Image w C#"
description: "Jak dodać podpis Image z kilkoma linijkami kodu .NET?"
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
    title: "Informacje o interfejsie API podpisów graficznych GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) to popularny interfejs API do elektronicznego podpisywania dokumentów. Dostępne są podpisy, takie jak teksty, obrazy, certyfikaty cyfrowe, kody kreskowe, kody QR, pieczątki lub metadane. Podpisy mogą być umieszczane na plikach PDF, dokumentach MS Word, skoroszytach MS Excel, prezentacjach MS PowerPoint, plikach Adobe Photoshop i różnych formatach graficznych. Klienci mogą podpisywać swoje dokumenty i aktualizować, wyszukiwać, weryfikować, usuwać lub przeglądać podpisy elektroniczne, które zostały umieszczone na tych dokumentach. Ponadto zapewniono wiele możliwości dostosowywania podpisów.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroki do podpisania Csv za pomocą Image w C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) umożliwia szybkie i łatwe podpisywanie dokumentów w formacie Csv za pomocą podpisów Image.
        
        * Utwórz instancję klasy Signature podając plik Csv do podpisania jako ścieżkę lub strumień pamięci
        * Utwórz wystąpienie klasy SignOptions i ustaw wszystkie wymagane dane.
        * Wywołaj metodę Signature.Sign() przekazującą wyjściowy plik Csv lub strumień pamięci

    title_right: " wymagania systemowe"
    content_right: |
        GroupDocs.Signature for .NET są obsługiwane na wszystkich głównych platformach i systemach operacyjnych. Przed wykonaniem poniższego kodu upewnij się, że masz zainstalowane w systemie następujące wymagania wstępne.

        * Systemy operacyjne: Microsoft Windows, Linux, MacOS
        * Środowiska programistyczne: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Pobierz najnowszą wersję GroupDocs.Signature for .NET z [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Csv file
        string filePath = "input.csv";
        // Set up output file
        string outputFilePath = "output.csv";
        // Provide image file
        string imageFilePath = "image.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
            //Provide sign options
            ImageSignOptions options = new ImageSignOptions(imageFilePath)
            {
                // set signature position
                Left = 50,
                Top = 200
            };

            // sign Csv document
            SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisywanie dokumentów Csv za pomocą Image Demo na żywo"
    content: |
       Podpisz teraz plik Csv różnymi podpisami, odwiedzając witrynę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Darmowe demo online czeka na Ciebie.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Inne obsługiwane podpisy Image dla C#"
    content: |
        "Możesz także podpisać Csv innymi typami podpisów. Zobacz poniższą listę."
    format: 
       
       
back_to_top:
    enable: true
---