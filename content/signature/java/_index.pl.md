---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Digital Signature API, dodaj podpis elektroniczny do obrazu PDF Word Excel"
head_description: "Interfejs API podpisu cyfrowego Java. Biblioteka podpisów elektronicznych do cyfrowego podpisywania plików PDF, Microsoft Word, arkuszy kalkulacyjnych Excel, prezentacji PowerPoint i formatów dokumentów graficznych."

############################# Header ############################
title: "Java API do zarządzania podpisami cyfrowymi"
description: "Zarządzaj podpisami elektronicznymi obrazów, kodów QR, kodów kreskowych, metadanych, tekstu i stempli w aplikacjach Java do podpisywania obrazów i formatów plików dokumentów cyfrowych."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

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
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "cennik"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API pomaga tworzyć aplikacje Java z funkcją podpisów elektronicznych do podpisywania dokumentów cyfrowych w obsługiwanych formatach bez instalowania zewnętrznego oprogramowania. Obsługuje manipulację i zarządzanie różnymi typami podpisów elektronicznych, takimi jak obraz, kod kreskowy, kod QR, stempel, tekst, optyczny i metadane. Wszystkie elektroniczne dokumenty biznesowe, takie jak Microsoft Office Word, prezentacje PowerPoint, arkusze kalkulacyjne Excel, obrazy i pliki PDF, można podpisać cyfrowo, dostosowując właściwości podpisu, np. cień, wymiary, wyrównanie i więcej zgodnie z Twoimi wymaganiami. Biblioteka podpisów cyfrowych jest prosta i lekka, składa się z pojedynczego pliku DLL, który można łatwo zintegrować z nową lub istniejącą aplikacją Java.  

      Dzięki GroupDocs.Signature for Java API możesz załadować wszystkie zarejestrowane certyfikaty z systemu lub zlokalizować istniejące podpisy za pomocą wyszukiwania prostego i zaawansowanego. Opcje pracy z dokumentami chronionymi hasłem, określające wspólne właściwości podpisu (rozmiar tekstu, przezroczystość, obrót, weryfikacja, właściwości czcionki, opcje kolorów, numer strony, szerokość, góra, lewo itp.) Rozwiązanie do zarządzania podpisami elektronicznymi dla dokumentów cyfrowych.  

      GroupDocs.Signature for Java jest kompatybilny ze wszystkimi wersjami Java i obsługuje popularne systemy operacyjne (Windows, Linux, MacOS), które mogą uruchamiać środowisko wykonawcze Java
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          To jest przegląd funkcji GroupDocs.Signature dla Javy:
      
        right:
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
            * Podpis pola formularza
      
      ## TAB TWO ##
      tab_two:
        description: |
          Interfejs API podpisu elektronicznego Java obsługuje różne formaty plików dokumentów, które wymieniono poniżej. [Obsługiwane formaty dokumentów.](https://docs.groupdocs.com/signature/java/supported-document-formats/)

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
          GroupDocs.Signature for Java obsługuje następujące systemy operacyjne, frameworki i menedżery pakietów:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "System operacyjny"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Obsługiwane frameworki"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Środowiska programistyczne"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Narzędzie do automatyzacji budowania"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature dla funkcji Java"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Twórz, czytaj, modyfikuj, ukrywaj i usuwaj podpisy elektroniczne z obsługiwanych formatów dokumentów"

      # feature loop
      - icon: "fas fa-eye"
        content: "Dostęp do podpisanego dokumentu ze strumienia, ścieżki względnej lub ścieżki bezwzględnej"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Zastosuj podpis tekstowy do dokumentów, arkuszy kalkulacyjnych, prezentacji, obrazów i plików PDF"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Dodaj podpis tekstowy jako adnotację, naklejkę, obraz do plików PDF, a także skonfiguruj styl i kolor"

      # feature loop
      - icon: "fas fa-code"
        content: "Podpisz dokument PDF, plik obrazu i uzyskaj dane wyjściowe w innym formacie pliku"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Podpisuj cyfrowo obrazy podpisem tekstowym jako znakiem wodnym i dodaj przezroczystość, obrót do podpisu elektronicznego"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Wyszukuj certyfikaty i podpisuj dokumenty Microsoft Word, Excel i PDF za pomocą certyfikatów cyfrowych"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Podpisuj formaty dokumentów edytora tekstu za pomocą rodzimych znaków wodnych"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Użyj kodu QR, kodu kreskowego do podpisywania plików Word, slajdów, komórek, plików PDF i obrazów"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Konfiguruj i stosuj podpisy stempli do bezpiecznych obsługiwanych formatów plików"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Konfiguruj i przypisuj podpisy obrazów do dokumentów, arkuszy kalkulacyjnych, prezentacji, obrazów i plików PDF"

      # feature loop
      - icon: "fas fa-columns"
        content: "Skonfiguruj właściwości podpisu, np. Wygląd i styl, marginesy, wyrównanie itp."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Zastosuj podpis cyfrowy do dokumentu chronionego hasłem"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Przeprowadź weryfikację tekstu dokumentów PDF za pomocą modułu obsługi podpisów"

      # feature loop
      - icon: "fas fa-print"
        content: "Cyfrowa weryfikacja dokumentów Word, Cell, PDF z kontenerami certyfikatów .CER i .PFX"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Określ różne typy jednostek miary (np. milimetry, piksele itp.) dla podpisów tekstowych PDF"

      # feature loop
      - icon: "fas fa-lock"
        content: "Uzyskaj informacje o dokumencie za pośrednictwem pliku lub adresu URL — dodaj podpisy pól formularza do dokumentów PDF"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Dodaj niestandardowy obiekt danych, wbudowaną kartę VCard, e-mail, EPC, MeCard lub obiekt zdarzenia do kodu QR"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Stosowanie różnych stylów pędzla do podpisów, np. pędzla gradientowego, promieniowego, jednolitego i tekstury"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Podpisz dokument znajdujący się na FTP lub Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Ustaw wyrównanie tekstu wewnątrz kształtów dla dokumentów, slajdów, obrazów i plików PDF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Wyszukuj, weryfikuj i podpisuj cyfrowo dokumenty prezentacji programu PowerPoint"

      # feature loop
      - icon: "fas fa-cube"
        content: "Umieść podpis za pomocą pikseli w dokumentach komórek i pozycjonowaniu tekstu dla podpisów stempli"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Zaimplementuj prostokątny podpis stempla z zaokrąglonymi narożnikami"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Rozszerz podpisy kodów kreskowych i kodów QR o zawartość danych obrazu"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Dodaj zaszyfrowane podpisy metadanych podczas pracy z opcjami podpisywania i wyszukiwania"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Osadzaj niestandardowe obiekty w podpisach metadanych w programach Word, Excel i prezentacjach"

    more_feature:
      # more_feature_loop
      - title: "Łatwo konfiguruj i stosuj podpisy elektroniczne"
        content: |
          GroupDocs.Signature for Java API umożliwia konfigurowanie i dodawanie podpisów elektronicznych do obsługiwanych formatów dokumentów. Poniżej znajduje się przykład kodu, który pokazuje, jak łatwo zastosować podpis tekstowy do pliku PDF:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // ustaw pozycję podpisu
          options.setLeft(100);
          options.setTop(100);
          
          // ustaw prostokąt podpisu
          options.setWidth(100);
          options.setHeight(30);

          // ustaw kolor tekstu i czcionkę
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // podpisz dokument do pliku
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Obsługiwane typy kodowania kodów kreskowych dla podpisu elektronicznego"
        content: |
          Korzystając z GroupDocs.Signature for Java API, możesz zastosować podpisy kodów kreskowych i kodów QR do obsługiwanych formatów plików. GroupDocs.Signature for Java obsługuje szeroki zakres typów kodowania kodów kreskowych, aby zaspokoić większość wymagań. Obsługiwane typy kodowania kodów kreskowych obejmują: Code 11, Code 128, Code 16K/32, Databar codes, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard i Kod39 rozszerzony.

          Podobnie GroupDocs.Signature for Java API umożliwia korzystanie z typów kodów QR, takich jak QR, Aztec i Data Matrix. Obsługiwane typy kodowania QR-Code obejmują Aztec, DataMatrix, GS1 DataMatrix i GS1 QR.

      # more_feature_loop
      - title: "Wyszukaj podpisy i certyfikaty"
        content: |
          Dzięki GroupDocs.Signature for Java API możesz przeszukiwać podpisy kodów QR i kodów kreskowych w dowolnym dokumencie, prezentacji, arkuszu kalkulacyjnym, obrazie, a także w pliku PDF i pobrać wynik wyszukiwania. Możesz także wyszukiwać niestandardowe obiekty danych z dokumentów podpisanych za pomocą kodu QR, a także przeszukiwać standardową kartę VCard i obiekt e-mail z dokumentów podpisanych za pomocą kodu QR. Obsługiwana jest również weryfikacja zaszyfrowanego tekstu podpisów QR-Code oraz wyszukiwanie podpisu metadanych w dokumentach PDF. Zastosuj dodatkowe kryteria wyszukiwania dla podpisów cyfrowych dokumentów Words & Cells.  

          Opcja wyszukiwania jest również dostępna dla sygnatur metadanych dla dokumentów Word, slajdów i arkuszy kalkulacyjnych, podczas gdy wyszukiwanie pól formularza jest dostępne dla dokumentów PDF.

      # more_feature_loop
      - title: "Skonfiguruj właściwości podpisu elektronicznego"
        content: |
          Aby poprawić UX użytkowników końcowych, GroupDocs.Signature for Java API zapewnia wiele właściwości, które można dość łatwo skonfigurować. Można ustawić opcje czcionek i kolorów (kolor tła, kolor pierwszego planu, pogrubienie, kursywa, podkreślenie, rodzina czcionek, rozmiar czcionki itp.), opcje tła i obramowania (kolor tła, przezroczystość tła, kolor obramowania, styl kreski obramowania, grubość obramowania, Przezroczystość obramowania itp.), Marginesy podpisu (lewy, górny, szerokość, wysokość, dopełnienie itp.) oraz Ustaw obszar podpisu obrazu i wyrównanie podpisu (wyrównanie w poziomie, wyrównanie w pionie itp.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature oferuje interfejsy API do podpisywania dokumentów dla innych popularnych środowisk programistycznych"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---