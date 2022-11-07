---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Text
fileformat: Odt
productName: .NET
lang: pl
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Text signatures at Odt with C#

############################# Head ############################
head_title: "Wyszukaj podpisy Text w pliku Odt w C#"
head_description: "Użyj .NET do wyszukiwania podpisów Text w plikach Odt przy użyciu kilku linijek kodu."

############################# Header ############################
title: "Wyszukaj podpisy Text w pliku Odt"
description: "Natywny interfejs API .NET umożliwia wyszukiwanie podpisów Text w już podpisanych plikach Odt. Przeprowadź zaawansowane wyszukiwanie podpisu elektronicznego w swoich dokumentach Odt, używając kilku linijek kodu."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Informacje o interfejsie API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) udostępnia interfejs API .NET do przetwarzania dokumentów przy użyciu różnych typów podpisów, takich jak teksty, obrazy, certyfikaty cyfrowe, kody kreskowe, kody QR, pieczątki lub metadane. Użytkownicy mogą dodawać, usuwać, aktualizować, weryfikować lub wyszukiwać podpisy elektroniczne w plikach PDF, dokumentach MS Word, skoroszytach MS Excel, prezentacjach MS PowerPoint, plikach Adobe Photoshop i różnych formatach obrazów, z dodatkową obsługą dostosowywania właściwości podpisów zgodnie z potrzebami.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Jak wyszukiwać podpisy Text w Odt"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ułatwia programistom .NET wyszukiwanie podpisów Text w plikach Odt z ich aplikacji, wykonując kilka prostych kroków.
        
        * Utwórz nową instancję klasy Signature i przekaż ścieżkę dokumentu źródłowego jako parametr konstruktora.
        * Utwórz wystąpienie obiektu SearchOptions zgodnie z własnymi wymaganiami i określ opcje wyszukiwania.
        * Wywołaj metodę Search instancji klasy Signature i przekaż do niej SearchOptions.
        * Przetwarzaj wyniki wyszukiwania zgodnie z Twoimi wymaganiami.

    title_right: "wymagania systemowe"
    content_right: |
        GroupDocs.Signature for .NET są obsługiwane na wszystkich głównych platformach i systemach operacyjnych. Przed wykonaniem poniższego kodu upewnij się, że masz zainstalowane w systemie następujące wymagania wstępne.

        * Systemy operacyjne: Microsoft Windows, Linux, MacOS
        * Środowiska programistyczne: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Pobierz najnowszą wersję GroupDocs.Signature for .NET z [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Odt file
        string filePath = "input.odt";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                TextSearchOptions options = new TextSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // specify text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature"
                };

                // search for Text signatures in Odt document
                List<TextSignature> signatures = signature.Search<TextSignature>(options);

                // process signatures which were found                
                foreach (TextSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Wyszukaj Text podpisy elektroniczne Demo na żywo"
    content: |
       Wyszukaj w dokumencie różne podpisy elektroniczne w plikach Odt, odwiedzając witrynę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Wyszukaj inne podpisy Text za pomocą C#"
    content: |
        "Wyszukiwanie podpisów elektronicznych w różnych dokumentach. Znajdź podpisy z jednego z popularnych formatów plików, jak pokazano poniżej."
    format: 
           
       
back_to_top:
    enable: true
---