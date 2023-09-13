---
############################# Static ############################
layout: "landing"
date: 2023-09-13T10:36:52
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
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, interfejsy API w chmurze i aplikacje do podpisywania dokumentów online"
head_description: "Uzyskaj kompleksowe rozwiązanie do podpisu elektronicznego dokumentów dla aplikacji .NET, Java i opartych na chmurze. Podpisuj online popularne formaty dokumentów za pomocą prostej funkcji przeciągania i upuszczania"

############################# Header ############################
title: "Podpisz dokumenty<br>poprzez API .NET"
description: "Podpisuj cyfrowe dokumenty i obrazy na dowolnej platformie, korzystając z naszych elastycznych interfejsów API i rozwiązań opartych na aplikacjach dla programistów i użytkowników końcowych."
words:
  for: "Do"

actions:
  main: "Bezpłatne pobieranie NuGeta"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Koncesjonowanie"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Gotowy żeby zacząć?"
  description: "Wypróbuj bezpłatnie funkcje GroupDocs.Signature lub poproś o licencję"

release:
  title: "Wydano wersję {0}"
  notes: "Zobacz co nowego"
  downloads: "Pliki do pobrania"

code:
  title: "Podpisuj pliki PDF w C#"
  more: "Więcej przykładów"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Wybierz dokument PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Podaj tekst
        var options = new TextSignOptions("John Smith")
        {
            // Ustaw kolor
            ForeColor = Color.Red
        };
        // Podpisz dokument i zapisz do pliku
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Przegląd GroupDocs.Signature"
  description: "API do wykonywania podpisywania dokumentów i operacji z tym związanych w aplikacjach .NET"
  features:
    # feature loop
    - title: "Dodawanie podpisów do dokumentów biznesowych w C#"
      content: "Podpisywanie dokumentów: Dzięki GroupDocs.Signature for .NET możesz dodawać różne typy podpisów, takie jak tekst, obrazy, kody kreskowe i certyfikaty cyfrowe, do dokumentów PDF i dokumentów pakietu Office. Ten interfejs API umożliwia podpisywanie dokumentów niemal dowolnym typem danych, w tym ukrytymi metadanymi."

    # feature loop
    - title: "Przetwarzanie podpisanych dokumentów"
      content: "Dodatkowe przetwarzanie: możesz wykonywać zaawansowane operacje na podpisanych dokumentach za pomocą GroupDocs.Signature. Obejmuje to wyszukiwanie istniejących podpisów w dokumentach biznesowych i weryfikację ich według określonych kryteriów. Dodatkowo możesz pobierać informacje o dokumentach i przeglądać strony za pośrednictwem tego interfejsu API .NET."

    # feature loop
    - title: "Dostosowywanie wyników"
      content: "GroupDocs.Signature dla .NET oferuje szerokie możliwości dostosowywania. Możesz precyzyjnie umieszczać podpisy w dowolnym miejscu strony dokumentu i dostosowywać ich wygląd, korzystając z różnych ustawień. Co więcej, ten interfejs API obsługuje zapisywanie przetworzonych dokumentów w szerokiej gamie obsługiwanych formatów."

############################# Platforms ############################
platforms:
  enable: true
  title: "Niezależność platformy"
  description: "GroupDocs.Signature for .NET obsługuje następujące systemy operacyjne, struktury i menedżery pakietów"
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
    GroupDocs.Signature for .NET obsługuje operacje na następujących [formatach plików] (https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  description: "Szybkie i dokładne podpisywanie plików PDF, dokumentów biurowych i obrazów"

  items:
    # feature loop
    - icon: "merge"
      title: "Podpisanie dokumentu"
      content: "Dokładne dodawanie jednego lub wielu obsługiwanych typów podpisów w dowolnym określonym miejscu dokumentów biznesowych."

    # feature loop
    - icon: "split"
      title: "Dostosuj podpisy"
      content: "Wykorzystaj funkcje takie jak kolor, czcionka, obramowanie, obrót itp., aby skonfigurować wygląd podpisów."

    # feature loop
    - icon: "move"
      title: "Ochrona hasłem dokumentu"
      content: "Zabezpiecz określone typy dokumentów, ustawiając hasło po podpisaniu."

    # feature loop
    - icon: "remove"
      title: "Ochrona przed zmianami"
      content: "Zapobiegaj zmianom w ważnych dokumentach biznesowych po złożeniu podpisu za pomocą certyfikatu cyfrowego."

    # feature loop
    - icon: "rotate"
      title: "Konwertuj podpisane pliki na inne formaty"
      content: "Konwertuj podpisane pliki do żądanych formatów, na przykład zapisując dokument programu Word jako plik PDF."

    # feature loop
    - icon: "swap"
      title: "Wyodrębnij podglądy stron"
      content: "Wyodrębnij strony z podpisanych dokumentów jako pojedyncze obrazy do przyszłego przetwarzania."

    # feature loop
    - icon: "extract"
      title: "Wyszukiwanie podpisów w dokumentach"
      content: "Odzyskaj informacje o wcześniej dodanych podpisach w konkretnych dokumentach."

    # feature loop
    - icon: "orientation"
      title: "Zweryfikuj podpisane dokumenty"
      content: "Sprawdź poprawność podpisywania dokumentów za pomocą funkcji walidacji."

    # feature loop
    - icon: "preview"
      title: "Zaktualizuj lub usuń podpisy"
      content: "Z łatwością zmieniaj położenie określonych podpisów na stronie, modyfikuj ich tekst lub usuwaj je bez żadnych problemów."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Próbki kodu"
  description: "Niektóre przypadki użycia typowych operacji GroupDocs.Signature dla .NET"
  items:
    # code sample loop
    - title: "Dodaj kod QR do pliku PDF"
      content: |
        Dodanie [kodów QR](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) do określonych stron dokumentów PDF może usprawnić procesy biznesowe. Poniżej znajduje się przykład dodania kodu QR za pomocą GroupDocs.Signature.
        {{< landing/code title="Jak umieścić kod QR w formacie PDF.">}}
        ```csharp {style=abap}
        // Załaduj dokument do podpisu
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Twórz opcje kodów QR z predefiniowanym tekstem
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Skonfiguruj typ i położenie kodowania kodu QR na stronie
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Podpisz dokument i zapisz go jako plik wynikowy
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Ochrona dokumentu DOCX za pomocą certyfikatu cyfrowego"
      content: |
        Możesz [Chroń dokument](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/), używając podpisów osobistych lub firmowych przechowywanych jako certyfikaty cyfrowe. Tak chronionych dokumentów nie można modyfikować bez unieważnienia podpisu.
        {{< landing/code title="Oto, jak zapewnić integralność dokumentów.">}}
        ```csharp {style=abap}   
        // Załaduj dokument, który ma zostać podpisany cyfrowo
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Określ opcje podpisu cyfrowego i podaj ścieżkę do pliku certyfikatu
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Ustaw hasło certyfikatu
                Password = "1234567890"
            };
            // Podpisz dokument i zapisz go w wybranej ścieżce
            signature.Sign("digitally_signed.pdf", options);
        }
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
