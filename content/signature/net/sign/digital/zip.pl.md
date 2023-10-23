---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Zip
productName: .NET
lang: pl
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Zip for C#

############################# Head ############################
head_title: "Dodawanie podpisów elektronicznych do pliku Zip za pomocą C#"
head_description: "Umieść podpis cyfrowy w pliku Zip dla .NET, używając kilku linijek kodu. Użyj interfejsu GroupDocs Document Signature API, aby podpisać dziesiątki formatów plików."

############################# Header ############################
title: "eSign Zip pliki z podpisami Digital w C#"
description: "Jak dodać podpis Digital za pomocą kilku linijek kodu .NET?"
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
    title: "O GroupDocs.Signature for .NET API podpisów cyfrowych"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) to popularny interfejs API do podpisywania dokumentów z cyfrowymi podpisami elektronicznymi i certyfikatami cyfrowymi. W przypadku podpisów cyfrowych API wykorzystuje pliki certyfikatów PFX do opisywania dokumentów za pomocą chronionych hasłem kluczy prywatnych i publicznych. Podpisy cyfrowe mogą być używane do poświadczania dokumentów biznesowych za pomocą określonej strony eSign PDF, poświadczania całych dokumentów Microsoft Office, takich jak Words, Excel, pliki Powerpoint i dokumenty Open Office. Klienci mogą łatwo manipulować podpisami, np. edytować je, usuwać lub dostosowywać. API umożliwia wyszukiwanie i weryfikację podpisów. Ponadto zapewniono wiele możliwości dostosowywania podpisów.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kroki do podpisania Zip za pomocą Digital w C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) umożliwia szybkie i łatwe podpisywanie dokumentów w formacie Zip za pomocą podpisów Digital.
        
        * Utwórz instancję klasy Signature podając plik Zip do podpisania jako ścieżkę lub strumień pamięci
        * Utwórz wystąpienie klasy SignOptions i ustaw wszystkie wymagane dane.
        * Wywołaj metodę Signature.Sign() przekazującą wyjściowy plik Zip lub strumień pamięci

    title_right: " wymagania systemowe"
    content_right: |
        GroupDocs.Signature for .NET są obsługiwane na wszystkich głównych platformach i systemach operacyjnych. Przed wykonaniem poniższego kodu upewnij się, że masz zainstalowane w systemie następujące wymagania wstępne.

        * Systemy operacyjne: Microsoft Windows, Linux, MacOS
        * Środowiska programistyczne: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Pobierz najnowszą wersję GroupDocs.Signature for .NET z [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Zip file
        string filePath = "input.zip";
        // Set up output file
        string outputFilePath = "output.zip";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Zip document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisywanie dokumentów Zip za pomocą Digital Demo na żywo"
    content: |
       Podpisz teraz plik Zip różnymi podpisami, odwiedzając witrynę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Darmowe demo online czeka na Ciebie.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Inne obsługiwane podpisy Digital dla C#"
    content: |
        "Możesz także podpisać Zip innymi typami podpisów. Zobacz poniższą listę."
    format: 
       
       
back_to_top:
    enable: true
---