---
############################# Static ############################
layout: "product"
date: 2022-03-01T15:12:22
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: pl
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Interfejs API podpisu cyfrowego platformy .NET — podpis elektroniczny w formacie PDF Word Excel, obrazy"
head_description: "Interfejs API podpisu cyfrowego C# .NET, biblioteka eSignature do elektronicznego podpisywania plików PDF, Word, arkuszy kalkulacyjnych Excel, PowerPoint, obrazów i formatów dokumentów graficznych."

############################# Header ############################
title: "Natywny interfejs API .NET dla podpisów elektronicznych"
description: "Dodawaj podpisy cyfrowe do formatów dokumentów i wdrażaj popularne typy podpisów elektronicznych (tekst, obraz, kod QR, kod kreskowy, stempel i metadane) w aplikacjach .NET."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Przegląd"

            # button loop
            - link: "#features"
              text: "Cechy"

            # button loop
            - link: "#support"
              text: "Wsparcie"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Demo na żywo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/net"
              text: "cennik"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      Używaj GroupDocs.Signature for .NET API do tworzenia aplikacji w C#, ASP.NET i innych technologiach opartych na .NET, które umożliwiają podpisywanie cyfrowych dokumentów biznesowych, takich jak PDF, Microsoft Word, arkusze kalkulacyjne Excel, prezentacje PowerPoint, obrazy, OpenDocument i innych standardowych formatów plików bez konieczności instalowania dodatkowego oprogramowania. Ta biblioteka podpisów elektronicznych jest łatwa w obsłudze, a programiści .NET mogą łatwo dodawać zaawansowane funkcje podpisów cyfrowych do swoich aplikacji, umożliwiając użytkownikom bezpieczne podpisywanie, wyszukiwanie i weryfikację podpisów elektronicznych z popularnych formatów dokumentów. Obsługuje wdrażanie różnych typów podpisów, takich jak tekst, obraz, kod kreskowy, kod QR, pole formularza, pieczęć i metadane.  

      Interfejs API podpisów dokumentów zapewnia proste i zaawansowane opcje wyszukiwania umożliwiające błyskawiczne zlokalizowanie wymaganych podpisów na dokumencie. Opcje stosowania stylu podpisu, zarządzania wyglądem i dostosowywania właściwości podpisu, takich jak wymiary, cień, wyrównanie i inne, są również wykonalne dzięki temu bogatemu w funkcje interfejsowi API do podpisywania dokumentów.  

      GroupDocs.Signature for .NET może być używany w dowolnym środowisku programistycznym obsługującym platformę .NET. Jest kompatybilny ze wszystkimi językami opartymi na .NET i obsługuje popularne systemy operacyjne (Windows, Linux, MacOS), w których można zainstalować frameworki Mono lub .NET (w tym .NET Core).
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Poniżej znajduje się omówienie GroupDocs.Signature dla platformy .NET:
      
        left:
          enable: true
          icon: "fab fa-html5"
          title: "Typy podpisów"
          content: |
            * Podpis tekstowy
            * Podpis obrazu
            * Podpisy cyfrowe
            * Podpis kodu QR
            * Podpis kodu kreskowego
            * Pieczęć podpisu
            * Podpis metadanych
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Signature for .NET obsługuje podpisywanie wszystkich popularnych formatów dokumentów. Wystarczy kilka wierszy kodu, aby dodać podpis PDF, Microsoft Office Word, arkusz kalkulacyjny Excel, obraz, HTML, pocztę e-mail programu Outlook, program OneNote, podpisywanie projektów i grafiki w aplikacjach .NET. [Obsługiwane formaty dokumentów.](https://docs.groupdocs.com/signature/net/supported-document-formats/)

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Other Formats"
              content: |
                * **Obrazy**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Metapliki**: EMF, WMF, CMX
                * **Przenośny**: PDF
                * **Skalowalna Grafika wektorowa**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Inni**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for .NET obsługuje następujące systemy operacyjne, frameworki i menedżery pakietów:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "System operacyjny"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Obsługiwane frameworki"
              content: |
                * .NET Framework 2.0 or higher
                * Mono Framework 1.2 or higher
                * .NET Standard 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Menedżer pakietów"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Środowiska programistyczne"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature dla funkcji platformy .NET"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Twórz, wyszukuj, aktualizuj, ukrywaj, weryfikuj i usuwaj podpisy elektroniczne z obsługiwanych formatów dokumentów"

      # feature loop
      - icon: "fas fa-eye"
        content: "Określ zaawansowane podpisy elektroniczne XML (XAdES) dla arkuszy kalkulacyjnych Excel"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Odzyskaj zawartość obrazu z dokumentów podpisanych za pomocą kodu QR, kodu kreskowego i podpisów graficznych"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Ustaw wysokość, szerokość, marginesy i wyrównanie dla podpisu tekstu lub obrazu i umieść na określonej stronie"

      # feature loop
      - icon: "fas fa-code"
        content: "Wyszukuj, weryfikuj i podpisuj cyfrowo dokumenty prezentacji programu PowerPoint"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Podpisuj formaty dokumentów edytora tekstu za pomocą rodzimych znaków wodnych"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Obsługuje zaokrąglone rogi dla prostokątnych typów podpisów stempli"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Zastosuj podpis tekstowy lub graficzny na określonym arkuszu Excel lub ustaw podpis elektroniczny we wszystkich arkuszach"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Określ konkretny numer wiersza i kolumny, aby umieścić podpis tekstowy lub graficzny w arkuszu Excel"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Zastosuj cień do podpisu tekstowego w programie Microsoft PowerPoint i ustaw jego kolor, kąt i przezroczystość"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Skonfiguruj style obramowania podpisu tekstowego i opcje czcionek dla arkuszy programu Excel"

      # feature loop
      - icon: "fas fa-columns"
        content: "Ustaw typ podpisu obrazu, np. Okrągły lub kwadratowy i skonfiguruj marginesy, kolor czcionki, obrót"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Zastosuj certyfikaty cyfrowe do dokumentów, arkuszy kalkulacyjnych i plików PDF z linią podpisu"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Wykonaj ustawienia kolorów, zastosuj przezroczystość i obrót do podpisu tekstowego"

      # feature loop
      - icon: "fas fa-print"
        content: "Ustaw opcje jasności i skali szarości oraz określ wcięcie podpisu obrazu w obrazie"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Osadzaj niestandardowe obiekty, serializuj, a także szyfruj i odszyfruj wartości sygnatur metadanych dokumentu PDF"

      # feature loop
      - icon: "fas fa-lock"
        content: "Ukryj, usuń lub dostosuj wygląd podpisów cyfrowych z dokumentów PDF"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Podpisuj dokumenty PDF za pomocą cyfrowego pola formularza i podpisu tekstowego jako obrazu, adnotacji, naklejki lub znaku wodnego"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Umieść podpis tekstowy w polach formularzy dokumentów MS Word i PDF"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Określ dowolne strony dokumentów do przetwarzania podpisu lub rozszerzonej weryfikacji podpisu elektronicznego dla plików Word"

      # feature loop
      - icon: "fas fa-heading"
        content: "Zapisz podpisany plik obrazu w innym formacie i wyeksportuj podpisany arkusz kalkulacyjny jako obraz lub wielostronicowy TIFF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Przypisz, zmodyfikuj i usuń hasło do podpisanych plików oraz zastosuj podpis elektroniczny do plików chronionych hasłem"

      # feature loop
      - icon: "fas fa-cube"
        content: "Arkusze eSign, slajdy PowerPoint, dokumenty Word i obrazy z niestandardowymi obiektami w metadanych"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Skonfiguruj style pędzla podpisu jako bryłę, teksturę, gradient liniowy i gradient promieniowy"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Podpisuj dokumenty za pomocą niestandardowego zaszyfrowanego tekstu lub danych z kodu QR"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Wyszukuj i podpisuj pliki w formacie DjVu jako dokument obrazu"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Wyodrębnij informacje o dokumencie, np. liczbę stron, poprzez adres URL pliku"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Wyszukuj, podpisuj i weryfikuj pliki programu CorelDraw jako dokumenty graficzne"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Przechowuj informacje o historii przetworzonych lub usuniętych podpisów w metadanych"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Dodaj niestandardowy obiekt danych, kartę VCard lub obiekt e-mail do kodu QR i zweryfikuj zaszyfrowany kod QR w plikach PDF"

    more_feature:
      # more_feature_loop
      - title: "Łatwe dodawanie podpisów cyfrowych"
        content: |
          GroupDocs.Signature for .NET API umożliwia dodawanie różnych typów podpisów do obsługiwanych formatów plików. Typy podpisów, takie jak Tekst, Obraz, Cyfrowy, Pieczęć, Kod QR, Kod kreskowy i Metadane, można zastosować za pomocą GroupDocs.Signature for .NET. Poniższy przykład kodu pokazuje, jak zastosować podpis tekstowy do dokumentu PDF:

          ```cs
          using (Signature signature = new Signature("D:\\sample.pdf"))
          {
          TextSignOptions options = new TextSignOptions("John Smith")
          {
          // ustaw Kolor tekstu
          ForeColor = Color.Red
          };
          // podpisz dokument do pliku
          signature.Sign("D:\\signed.pdf", options);
          }
          ```

      # more_feature_loop
      - title: "Obsługiwane typy podpisów kodów kreskowych"
        content: |
          Nasz interfejs API do manipulacji podpisami oferuje funkcję stosowania podpisów kodów kreskowych do obsługiwanych formatów dokumentów. GroupDocs.Signature for .NET obsługuje różne typy kodów kreskowych, takie jak Code128, Code39Extended, Code39Standard, EAN14, EAN8, ITF14, UPCA i UPCE. Dostępny jest również statyczny obiekt o nazwie „AllTypes”, który obsługuje wszystkie zarejestrowane typy kodów kreskowych.

      # more_feature_loop
      - title: "Wyszukaj podpisy i certyfikaty"
        content: |
          GroupDocs.Signature for .NET API umożliwia wyszukiwanie certyfikatów cyfrowych w dokumentach Word, arkuszach kalkulacyjnych Excel i plikach PDF. Możesz także pobrać wszystkie certyfikaty cyfrowe zarejestrowane w systemie. Podpisy metadanych można również wyszukiwać w dokumentach Word, arkuszach kalkulacyjnych Excel, obrazach i plikach PDF za pomocą GroupDocs.Signature for .NET API.  

          Dzięki GroupDocs.Signature for .NET API możesz wyszukiwać podpisy QR-Code i Barcode w dowolnym dokumencie, prezentacji, arkuszu kalkulacyjnym, obrazie, a także w pliku PDF i pobierać postęp wyszukiwania. Możesz także wyszukiwać niestandardowe obiekty danych z dokumentów podpisanych podpisem QR-Code.

      # more_feature_loop
      - title: "Zaawansowane opcje wyszukiwania kodu kreskowego"
        content: |
          Możesz bardzo łatwo wyszukać i zlokalizować wymagany kod kreskowy za pomocą interfejsu API GroupDocs.Signature for.NET, ponieważ nasz interfejs API podpisu oferuje zaawansowane opcje wyszukiwania. Umożliwiają one wyszukiwanie kodu kreskowego na określonej stronie, wyszukiwanie w całym dokumencie, określanie różnych stron do przeszukania (pierwsza, ostatnia, parzysta, nieparzysta), wyszukiwanie kodu kreskowego o określonym typie kodowania, wyszukiwanie kodu kreskowego na podstawie określonego ciągu tekstowego lub wyszukiwanie kodu kreskowego na podstawie ciągu znaków z opcją „zawiera”.

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature oferuje interfejsy API do podpisywania dokumentów dla innych popularnych środowisk programistycznych"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
          product: "GroupDocs.Signature"
          platform: "Java"
          link: "/signature/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---