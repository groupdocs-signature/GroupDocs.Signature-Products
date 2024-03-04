---
############################# Static ############################
layout: "landing"
date: 2024-03-04T17:52:03
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: pl
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET, Java, interfejsy API w chmurze i aplikacje do podpisywania dokumentów online"
head_description: "Uzyskaj kompleksowe rozwiązanie do podpisu elektronicznego dokumentów dla aplikacji .NET, Java i opartych na chmurze. Podpisuj online popularne formaty dokumentów za pomocą prostej funkcji przeciągania i upuszczania"

############################# Header ############################
title: "Podpisz dokumenty<br>z API Node.js"
description: "Podpisuj cyfrowe dokumenty i obrazy na dowolnej platformie, korzystając z naszych elastycznych interfejsów API i rozwiązań opartych na aplikacjach dla programistów i użytkowników końcowych."
words:
  for: "Do"

actions:
  main: "Pobierz z NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Koncesjonowanie"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Gotowy żeby zacząć?"
  description: "Wypróbuj bezpłatnie funkcje GroupDocs.Signature lub poproś o licencję"

release:
  title: "Wydano wersję {0}"
  notes: "Zobacz co nowego"
  downloads: "Pliki do pobrania"

code:
  title: "Podpisywanie plików PDF przez Node.js"
  more: "Więcej przykładów"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```javascript {style=abap}   
    // Wybierz dokument PDF
    let signature = new Signature("sample.pdf");
    
    // Podaj tekst
    let options = new TextSignOptions("John Smith");
    
    // Ustaw kolor
    options.ForeColor = Color.Red;
    
    // Podpisz dokument i zapisz do pliku
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Przegląd GroupDocs.Signature"
  description: "Biblioteka podpisywania dokumentów gotowa do użycia w aplikacjach Node.js"
  features:
    # feature loop
    - title: "Rozwiązanie do podpisów cyfrowych dla dokumentów biznesowych w środowisku Node.js"
      content: "GroupDocs.Signature for Node.js via Java oferuje kompleksowy zestaw opcji podpisu cyfrowego dla dokumentów PDF, dokumentów Office i obrazów. Dostępne są teksty, kody kreskowe, obrazy, certyfikaty cyfrowe i metadane. Usprawnione przetwarzanie dokumentów zapewnia wydajność."

    # feature loop
    - title: "Zaawansowana manipulacja podpisanymi dokumentami"
      content: "GroupDocs.Signature umożliwia przetwarzanie podpisanych dokumentów. Wyszukuj i sprawdzaj podpisy przy użyciu różnych kryteriów. Dodatkowo wyodrębnij szczegółowe informacje o dokumencie lub wygeneruj obrazy podglądu stron."

    # feature loop
    - title: "Różnorodne formaty wyjściowe"
      content: "Nasze rozwiązanie zapewnia szeroką kontrolę nad formatem wyjściowym podpisanych dokumentów. Precyzyjnie umieść podpisy na dowolnej stronie i dostosuj ich wygląd. Zapisuj podpisane dokumenty w wielu obsługiwanych formatach i opcjonalnie zabezpiecz je hasłami."

############################# Platforms ############################
platforms:
  enable: true
  title: "Niezależność platformy"
  description: "GroupDocs.Signature for Node.js via Java przetwarza dokumenty w różnych systemach operacyjnych"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Obsługiwane formaty plików"
  description: |
    GroupDocs.Signature for Node.js via Java ułatwia operacje na [popularnych formatach plików](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formaty pakietu Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Obrazy i inne formaty
        * **Przenośny:** PDF
        * **Obrazy:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Inne formaty biurowe:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Inne formaty
        * **Sieć:** HTML, MHTML
        * **Archiwa:** ZIP, TAR, 7Z
        * **Certyfikaty:** PFX

############################# Features ############################
features:
  enable: true
  title: "Funkcje GroupDocs.Signature"
  description: "Podpisuj pliki PDF, dokumenty pakietu Office i obrazy za pomocą podpisów cyfrowych"

  items:
    # feature loop
    - icon: "sign"
      title: "Podpisy biznesowe"
      content: "Do podpisywania dokumentów stosuj różne typy podpisów. Umieść podpisy cyfrowe dokładnie w dowolnym miejscu strony."

    # feature loop
    - icon: "custom"
      title: "Dostosowywanie wyglądu podpisu"
      content: "Dostosuj wizualne aspekty podpisów, dostosowując kolor, czcionkę, obramowania, obrót i inne elementy, aby osiągnąć pożądany efekt."

    # feature loop
    - icon: "password"
      title: "Dokumenty chronione hasłem"
      content: "W przypadku wielu obsługiwanych formatów dokumentów zabezpiecz podpisane dokumenty hasłem, aby zwiększyć bezpieczeństwo."

    # feature loop
    - icon: "protect"
      title: "Zapobieganie nieautoryzowanym modyfikacjom"
      content: "Chroń najważniejsze dokumenty biznesowe podpisane certyfikatami cyfrowymi przed nieautoryzowanymi zmianami."

    # feature loop
    - icon: "convert"
      title: "Żądane formaty wyjściowe"
      content: "Bez problemu otrzymuj podpisane dokumenty w dowolnym obsługiwanym formacie. Z łatwością konwertuj dokumenty MS Word do formatu PDF."

    # feature loop
    - icon: "preview"
      title: "Podgląd dokumentów"
      content: "Zapisz poszczególne strony dokumentu jako obrazy na przyszłe potrzeby."

    # feature loop
    - icon: "search"
      title: "Wyszukiwanie podpisów"
      content: "Odzyskaj informacje o wcześniej dodanych podpisach w dokumentach."

    # feature loop
    - icon: "validate"
      title: "Walidacja dokumentu"
      content: "Zweryfikuj autentyczność podpisów złożonych na dowolnym dokumencie."

    # feature loop
    - icon: "update"
      title: "Zarządzanie podpisami"
      content: "Usuń, przenieś lub zmodyfikuj podpisy umieszczone na dowolnej stronie dokumentu."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Próbki kodu"
  description: "Przykłady ilustrujące typowe operacje GroupDocs.Signature for Node.js via Java"
  items:
    # code sample loop
    - title: "Oznacz plik PDF kodami QR"
      content: |
        Włączenie [kodów kreskowych](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) do określonych stron dokumentów PDF może usprawnić procesy biznesowe. W tej sekcji przedstawiono przykład dodania kodu QR za pomocą GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Jak umieścić kod QR w formacie PDF.">}}
        ```javascript {style=abap}
        // Załaduj dokument do podpisu
        let signature = new Signature("file_to_sign.pdf");
        
        // Twórz opcje kodów QR z predefiniowanym tekstem
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Skonfiguruj typ i położenie kodowania kodu QR na stronie
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Podpisz dokument i zapisz go jako plik wynikowy
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Ochrona DOCX za pomocą podpisu cyfrowego"
      content: |
        [Chroń swoje dokumenty](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) za pomocą podpisów opartych na certyfikatach cyfrowych. Podpis cyfrowy chroni dokumenty biznesowe przed zmianą treści.
        {{< landing/code title="Oto, jak zapewnić integralność dokumentów.">}}
        ```javascript {style=abap}   
        // Załaduj dokument, który ma zostać podpisany cyfrowo
        let signature = new Signature("file_to_sign.pdf");
        
        // Określ opcje podpisu cyfrowego i podaj ścieżkę do pliku certyfikatu
        let options = new DigitalSignOptions("certificate.pfx");

        // Ustaw hasło certyfikatu
        options.Password = "1234567890";

        // Podpisz dokument i zapisz go w wybranej ścieżce
        signature.Sign("digitally_signed.pdf", options);

        ```
        {{< /landing/code >}}

---
