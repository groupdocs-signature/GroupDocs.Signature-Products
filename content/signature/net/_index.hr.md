---
############################# Static ############################
layout: "landing"
date: 2024-02-29T14:43:07
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: hr
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

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
head_title: ".NET, Java, Cloud API-ji i online aplikacije za potpisivanje dokumenata"
head_description: "Nabavite sveobuhvatno rješenje za e-potpis dokumenata za .NET, Java i aplikacije temeljene na oblaku. Potpišite uobičajene formate dokumenata na mreži koristeći jednostavnu značajku povlačenja i ispuštanja"

############################# Header ############################
title: "Potpišite dokumente<br>putem .NET API-ja"
description: "Potpišite digitalne dokumente i slike na bilo kojoj platformi koristeći naše fleksibilne API-je i rješenja temeljena na aplikacijama za programere i krajnje korisnike."
words:
  for: "za"

actions:
  main: "Besplatno preuzimanje NuGet-a"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licenciranje"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Jeste li spremni za početak?"
  description: "Isprobajte značajke GroupDocs.Signature besplatno ili zatražite licencu"

release:
  title: "Objavljena verzija {0}"
  notes: "Pogledajte što je novo"
  downloads: "Preuzimanja"

code:
  title: "Potpišite PDF datoteke u C#"
  more: "Više primjera"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Odaberite PDF dokument
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Navedite tekst
        var options = new TextSignOptions("John Smith")
        {
            // Postavite boju
            ForeColor = Color.Red
        };
        // Potpišite dokument i spremite ga u datoteku
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Pregled GroupDocs.Signature"
  description: "API za izvođenje potpisivanja dokumenata i povezanih operacija u .NET aplikacijama"
  features:
    # feature loop
    - title: "Dodavanje potpisa poslovnim dokumentima u C#"
      content: "Potpisivanje dokumenata: s GroupDocs.Signature za .NET možete dodati različite vrste potpisa, kao što su tekst, slike, crtični kodovi i digitalni certifikati, u PDF i Office dokumente. Ovaj API omogućuje potpisivanje dokumenata s gotovo svim vrstama podataka, uključujući skrivene metapodatke."

    # feature loop
    - title: "Obrada potpisanih dokumenata"
      content: "Dodatna obrada: Možete izvoditi moćne operacije na potpisanim dokumentima pomoću GroupDocs.Signature. To uključuje traženje postojećih potpisa unutar poslovnih dokumenata i njihovu provjeru pomoću posebnih kriterija. Osim toga, možete dohvatiti informacije o dokumentu i pregledati stranice putem ovog .NET API-ja."

    # feature loop
    - title: "Prilagodba rezultata"
      content: "GroupDocs.Signature za .NET nudi opsežne mogućnosti prilagodbe. Potpise možete precizno pozicionirati bilo gdje na stranici dokumenta i prilagoditi njihov izgled pomoću raznih postavki. Nadalje, ovaj API podržava spremanje obrađenih dokumenata u širokom rasponu podržanih formata."

############################# Platforms ############################
platforms:
  enable: true
  title: "Neovisnost o platformi"
  description: "GroupDocs.Signature za .NET podržava sljedeće operativne sustave, okvire i upravitelje paketa"
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
  title: "Podržani formati datoteka"
  description: |
    GroupDocs.Signature za .NET podržava rad sa sljedećim [formatima datoteka](https://docs.groupdocs.com/signature/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office formati
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Slike i drugi formati
        * **Prijenosni:** PDF
        * **Slike:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Ostali uredski formati:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Ostali formati
        * **mreža:** HTML, MHTML
        * **Arhiva:** ZIP, TAR, 7Z
        * **Certifikati:** PFX

############################# Features ############################
features:
  enable: true
  title: "Značajke GroupDocs.Signature"
  description: "Potpisivanje PDF-ova, Office dokumenata i slika brzo i točno"

  items:
    # feature loop
    - icon: "sign"
      title: "Potpisivanje dokumenata"
      content: "Dodajte jednu ili više podržanih vrsta potpisa točno na bilo koje određeno mjesto u poslovnim dokumentima."

    # feature loop
    - icon: "custom"
      title: "Prilagodite potpise"
      content: "Upotrijebite značajke kao što su boja, font, obrub, rotacija itd. za konfiguraciju izgleda potpisa."

    # feature loop
    - icon: "password"
      title: "Zaštita dokumenta lozinkom"
      content: "Osigurajte određene vrste dokumenata postavljanjem lozinke nakon potpisivanja."

    # feature loop
    - icon: "protect"
      title: "Zaštita od promjena"
      content: "Spriječite izmjene važnih poslovnih dokumenata nakon dodavanja potpisa digitalnim certifikatom."

    # feature loop
    - icon: "convert"
      title: "Pretvorite potpisane datoteke u druge formate"
      content: "Pretvorite potpisane datoteke u željene formate, kao što je spremanje Word dokumenta kao PDF."

    # feature loop
    - icon: "preview"
      title: "Izdvojite preglede stranica"
      content: "Izdvojite stranice iz potpisanih dokumenata kao pojedinačne slike za buduću obradu."

    # feature loop
    - icon: "search"
      title: "Pretraga potpisa u dokumentima"
      content: "Dohvaćanje informacija o prethodno dodanim potpisima u određenim dokumentima."

    # feature loop
    - icon: "validate"
      title: "Potvrdite potpisane dokumente"
      content: "Provjerite ispravno potpisivanje dokumenata pomoću značajki provjere valjanosti."

    # feature loop
    - icon: "update"
      title: "Ažurirajte ili izbrišite potpise"
      content: "Jednostavno promijenite položaj određenih potpisa na stranici, izmijenite njihov tekst ili ih izbrišite bez ikakvih problema."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Uzorci kodova"
  description: "Neki slučajevi upotrebe tipičnog GroupDocs.Signature za .NET operacije"
  items:
    # code sample loop
    - title: "Dodajte QR kod u PDF"
      content: |
        Dodavanje [QR kodova](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) određenim stranicama PDF dokumenata može poboljšati poslovne procese. Ispod je primjer kako dodati QR kod pomoću GroupDocs.Signature.
        {{< landing/code title="Kako staviti QR kod u PDF.">}}
        ```csharp {style=abap}
        // Učitajte dokument za potpisivanje
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Stvorite opcije QR koda s unaprijed definiranim tekstom
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Konfigurirajte vrstu kodiranja QR koda i položaj na stranici
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Potpišite dokument i spremite ga kao datoteku rezultata
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Zaštita DOCX dokumenta pomoću digitalnog certifikata"
      content: |
        Možete [zaštititi dokument](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) pomoću osobnih ili korporativnih potpisa pohranjenih kao digitalni certifikati. Takvi zaštićeni dokumenti ne mogu se mijenjati bez poništavanja potpisa.
        {{< landing/code title="Evo kako osigurati integritet dokumenta.">}}
        ```csharp {style=abap}   
        // Učitajte dokument koji želite digitalno potpisati
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Navedite opcije digitalnog potpisivanja i navedite put do datoteke certifikata
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Postavite lozinku certifikata
                Password = "1234567890"
            };
            // Potpišite dokument i spremite ga na željenu putanju
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
