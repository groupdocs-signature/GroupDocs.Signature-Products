---
############################# Static ############################
layout: "landing"
date: 2023-09-13T10:36:50
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
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, interfejsy API w chmurze i aplikacje do podpisywania dokumentów online"
head_description: "Uzyskaj kompleksowe rozwiązanie do podpisu elektronicznego dokumentów dla aplikacji .NET, Java i opartych na chmurze. Podpisuj online popularne formaty dokumentów za pomocą prostej funkcji przeciągania i upuszczania"

############################# Header ############################
title: "Podpisz dokumenty<br>poprzez API Javy"
description: "Podpisuj cyfrowe dokumenty i obrazy na dowolnej platformie, korzystając z naszych elastycznych interfejsów API i rozwiązań opartych na aplikacjach dla programistów i użytkowników końcowych."
words:
  for: "Do"

actions:
  main: "Bezpłatne pobieranie Mavena"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Koncesjonowanie"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Gotowy żeby zacząć?"
  description: "Wypróbuj bezpłatnie funkcje GroupDocs.Signature lub poproś o licencję"

release:
  title: "Wydano wersję {0}"
  notes: "Zobacz co nowego"
  downloads: "Pliki do pobrania"

code:
  title: "Podpisuj pliki PDF w Javie"
  more: "Więcej przykładów"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Wybierz dokument PDF
    Signature signature = new Signature("sample.pdf");
    
    // Podaj tekst
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Podpisz dokument i zapisz do pliku
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Przegląd GroupDocs.Signature"
  description: "API do wykonywania podpisywania dokumentów i operacji z tym związanych w aplikacjach Java"
  features:
    # feature loop
    - title: "Ulepszone dokumenty biznesowe z podpisami cyfrowymi w Javie"
      content: "Szybkie i konfigurowalne podpisywanie: GroupDocs.Signature for Java oferuje szeroką gamę opcji podpisu cyfrowego dla plików PDF, obrazów i dokumentów pakietu Office. Możesz używać tekstu, kodów kreskowych, kodów QR, certyfikatów cyfrowych, zdjęć lub ukrytych metadanych. Przetwarzanie dokumentów jest szybkie i wydajne."

    # feature loop
    - title: "Manipulowanie podpisanymi dokumentami"
      content: "Zaawansowane przetwarzanie dokumentów obejmuje zaawansowane operacje na podpisanych dokumentach za pomocą GroupDocs.Signature for Java. Możesz wyszukiwać i weryfikować podpisy dodane do dokumentów biznesowych, korzystając z różnych przydatnych kryteriów. Dodatkowo możesz uzyskać dostęp do szczegółowych informacji o dokumencie lub uzyskać podgląd jego stron."

    # feature loop
    - title: "Różnorodność opcji wyjściowych"
      content: "Solidne opcje podpisywania umożliwiają dostosowanie wyników dokumentów podpisanych za pomocą GroupDocs.Signature for Java. Możesz precyzyjnie umieścić dowolny podpis na dowolnej stronie dokumentu i skonfigurować jego wygląd na różne sposoby. Interfejs Java API obsługuje zapisywanie podpisanych dokumentów biznesowych w wielu obsługiwanych formatach i udostępnia opcje zabezpieczania ich hasłami."

############################# Platforms ############################
platforms:
  enable: true
  title: "Niezależność platformy"
  description: "GroupDocs.Signature for Java obsługuje następujące systemy operacyjne, struktury i menedżery pakietów"
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Obsługiwane formaty plików"
  description: |
    GroupDocs.Signature for Java obsługuje operacje na następujących [formatach plików](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  description: "Podpisywanie plików PDF, dokumentów pakietu Office i obrazów za pomocą podpisów cyfrowych"

  items:
    # feature loop
    - icon: "merge"
      title: "Dodawanie podpisów"
      content: "Podpisz dokument, korzystając z różnych obsługiwanych typów podpisów, umieszczając podpis cyfrowy dokładnie w dowolnym miejscu na dowolnej stronie."

    # feature loop
    - icon: "split"
      title: "Dostosowywanie wyników"
      content: "Dostosuj wygląd podpisu, dostosowując kolor, czcionkę, obramowanie, obrót i inne funkcje, aby osiągnąć pożądany rezultat."

    # feature loop
    - icon: "move"
      title: "Zabezpieczanie dokumentów hasłem"
      content: "W przypadku wielu obsługiwanych typów dokumentów można chronić podpisany dokument hasłem."

    # feature loop
    - icon: "remove"
      title: "Zapobieganie nieautoryzowanym zmianom"
      content: "Chroń ważne dokumenty biznesowe podpisane certyfikatem cyfrowym przed nieautoryzowanymi modyfikacjami."

    # feature loop
    - icon: "rotate"
      title: "Uzyskiwanie wyników w pożądanych formatach"
      content: "Z łatwością uzyskaj podpisane pliki wynikowe w dowolnym obsługiwanym formacie. Możesz także bez wysiłku konwertować dokumenty MS Word do formatu PDF."

    # feature loop
    - icon: "swap"
      title: "Podgląd dokumentu"
      content: "Zapisz dowolną stronę dokumentu jako obraz do przyszłego przetwarzania."

    # feature loop
    - icon: "extract"
      title: "Szukanie podpisów"
      content: "Istnieje możliwość uzyskania informacji o wcześniej dodanych podpisach w konkretnych dokumentach."

    # feature loop
    - icon: "orientation"
      title: "Walidacja dokumentów"
      content: "Sprawdź poprawność podpisów na każdym podpisanym dokumencie."

    # feature loop
    - icon: "preview"
      title: "Zarządzanie podpisami"
      content: "Po umieszczeniu podpisu na stronie dokumentu można go usunąć, przenieść lub zaktualizować w razie potrzeby."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Próbki kodu"
  description: "Niektóre przypadki użycia typowych operacji GroupDocs.Signature for Java"
  items:
    # code sample loop
    - title: "Wzbogać dokument PDF kodem QR"
      content: |
        Ulepszanie procesów biznesowych poprzez dodanie [kodów QR](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) do określonych stron dokumentów PDF może być cenne. Poniżej znajduje się przykład dodania kodu QR za pomocą GroupDocs.Signature for Java.
        {{< landing/code title="Wzbogać dokument PDF kodem QR">}}
        ```java {style=abap}
        // Załaduj dokument do podpisu
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Twórz opcje kodów QR z predefiniowanym tekstem
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Skonfiguruj typ i położenie kodowania kodu QR na stronie
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Podpisz dokument i zapisz go jako plik wynikowy
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Użyj podpisu cyfrowego, aby chronić dokument DOCX"
      content: |
        Możesz [zabezpieczyć dokument](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/), używając podpisów osobistych lub firmowych przechowywanych jako certyfikaty cyfrowe. Dokumentów zabezpieczonych certyfikatem nie można zmieniać bez unieważnienia podpisu.
        {{< landing/code title="Użyj podpisu cyfrowego, aby chronić dokument DOCX">}}
        ```java {style=abap}   
        // Załaduj dokument, który ma zostać podpisany cyfrowo
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Określ opcje podpisu cyfrowego i podaj ścieżkę do pliku certyfikatu
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Ustaw hasło certyfikatu
        options.setPassword("1234567890");

        // Podpisz dokument i zapisz go w wybranej ścieżce
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

############################# Reviews ############################
# reviews:
# enable: true
# title: "{reviews.title}"
# description: "{reviews.description}"

# items:
#   # review loop
#   - title: "GroupDocs.Viewer"
#     content: "{reviews.review_1.content}"
#     author: "{reviews.review_1.author}"
#     company: "{reviews.review_1.company}"

#   # review loop
#   - title: "GroupDocs.Viewer"
#     content: "{reviews.review_2.content}"
#     author: "{reviews.review_2.author}"
#     company: "{reviews.review_2.company}"
---
