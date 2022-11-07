---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Pdf
productName: Java
lang: pl
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Pdf with Java

############################# Head ############################
head_title: "Wyszukaj podpisy Digital w pliku Pdf w Java"
head_description: "Użyj Java do wyszukiwania podpisów Digital w plikach Pdf przy użyciu kilku linijek kodu."

############################# Header ############################
title: "Wyszukaj podpisy Digital w pliku Pdf"
description: "Natywny interfejs API Java umożliwia wyszukiwanie podpisów Digital w już podpisanych plikach Pdf. Przeprowadź zaawansowane wyszukiwanie podpisu elektronicznego w swoich dokumentach Pdf, używając kilku linijek kodu."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Informacje o interfejsie API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) udostępnia interfejs API Java do przetwarzania dokumentów przy użyciu różnych typów podpisów, takich jak teksty, obrazy, certyfikaty cyfrowe, kody kreskowe, kody QR, pieczątki lub metadane. Użytkownicy mogą dodawać, usuwać, aktualizować, weryfikować lub wyszukiwać podpisy elektroniczne w plikach PDF, dokumentach MS Word, skoroszytach MS Excel, prezentacjach MS PowerPoint, plikach Adobe Photoshop i różnych formatach obrazów, z dodatkową obsługą dostosowywania właściwości podpisów zgodnie z potrzebami.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Jak wyszukiwać podpisy Digital w Pdf"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ułatwia programistom Java wyszukiwanie podpisów Digital w plikach Pdf z ich aplikacji, wykonując kilka prostych kroków.
        
        * Utwórz nową instancję klasy Signature i przekaż ścieżkę dokumentu źródłowego jako parametr konstruktora.
        * Utwórz wystąpienie obiektu SearchOptions zgodnie z własnymi wymaganiami i określ opcje wyszukiwania.
        * Wywołaj metodę Search instancji klasy Signature i przekaż do niej SearchOptions.
        * Przetwarzaj wyniki wyszukiwania zgodnie z Twoimi wymaganiami.

    title_right: "wymagania systemowe"
    content_right: |
        GroupDocs.Signature for Java są obsługiwane na wszystkich głównych platformach i systemach operacyjnych. Przed wykonaniem poniższego kodu upewnij się, że masz zainstalowane w systemie następujące wymagania wstępne.

        * Systemy operacyjne: Microsoft Windows, Linux, MacOS
        * Środowiska programistyczne: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Pobierz najnowszą wersję GroupDocs.Signature for Java z [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pdf file
        String filePath = "input.pdf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        DigitalSearchOptions options = new DigitalSearchOptions();

        // specify special search criteria
        options.setComments("Approved");
        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2021, 3, 5));
        options.setSignDateTimeTo(new Date(2022, 7, 16));
        
        // search for Digital signatures in Pdf document
        List<DigitalSignature> signatures = signature.search(DigitalSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Wyszukaj Digital podpisy elektroniczne Demo na żywo"
    content: |
       Wyszukaj w dokumencie różne podpisy elektroniczne w plikach Pdf, odwiedzając witrynę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Wyszukaj inne podpisy Digital za pomocą Java"
    content: |
        "Wyszukiwanie podpisów elektronicznych w różnych dokumentach. Znajdź podpisy z jednego z popularnych formatów plików, jak pokazano poniżej."
    format: 
           
       
back_to_top:
    enable: true
---