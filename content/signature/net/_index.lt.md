---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:50
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: lt
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
head_title: "C# .NET skaitmeninių parašų API – GroupDocs.Signature"
head_description: "Integruokite skaitmeninių parašų apdorojimą į savo .NET programas naudodami GroupDocs.Signature. Greitai ir efektyviai apsaugokite failus parašais."

############################# Header ############################
title: "Pasirašykite dokumentus<br>per .NET API"
description: "Pasirašykite skaitmeninius dokumentus ir vaizdus bet kurioje platformoje naudodami mūsų lanksčias API ir programuotojams ir galutiniams vartotojams skirtus sprendimus."
words:
  for: "dėl"

actions:
  main: "Nemokamas NuGet atsisiuntimas"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licencijavimas"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Pasiruošę pradėti?"
  description: "Išbandykite GroupDocs.Signature funkcijas nemokamai arba paprašykite licencijos"

release:
  title: "Išleista {0} versija"
  notes: "Pažiūrėkite, kas naujo"
  downloads: "Atsisiuntimai"

code:
  title: "Pasirašykite PDF failus C#"
  more: "Daugiau pavyzdžių"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Pasirinkite PDF dokumentą
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Pateikite tekstą
        var options = new TextSignOptions("John Smith")
        {
            // Nustatyti spalvą
            ForeColor = Color.Red
        };
        // Pasirašykite dokumentą ir išsaugokite faile
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Parašo apžvalga"
  description: "API, skirta dokumentų pasirašymui ir susijusioms operacijoms .NET programose atlikti"
  features:
    # feature loop
    - title: "Parašų pridėjimas prie verslo dokumentų C#"
      content: "Dokumentų pasirašymas: Naudodami GroupDocs.Signature, skirtą .NET, galite pridėti įvairių tipų parašų, tokių kaip tekstas, vaizdai, brūkšniniai kodai ir skaitmeniniai sertifikatai, prie PDF ir Office dokumentų. Ši API leidžia pasirašyti dokumentus naudojant beveik bet kokį duomenų tipą, įskaitant paslėptus metaduomenis."

    # feature loop
    - title: "Pasirašytų dokumentų tvarkymas"
      content: "Papildomas apdorojimas: galite atlikti galingas operacijas su pasirašytais dokumentais naudodami GroupDocs.Signature. Tai apima esamų parašų paiešką verslo dokumentuose ir jų patikrinimą pagal konkrečius kriterijus. Be to, naudodami šią .NET API galite gauti dokumento informaciją ir peržiūrėti puslapius."

    # feature loop
    - title: "Rezultatų pritaikymas"
      content: "GroupDocs.Signature for .NET siūlo plačias tinkinimo parinktis. Galite tiksliai išdėstyti parašus bet kurioje dokumento puslapio vietoje ir koreguoti jų išvaizdą naudodami įvairius nustatymus. Be to, ši API palaiko apdorotų dokumentų išsaugojimą įvairiais palaikomais formatais."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platformos nepriklausomybė"
  description: "GroupDocs.Signature for .NET palaiko šias operacines sistemas, sistemas ir paketų tvarkykles"
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
  title: "Palaikomi failų formatai"
  description: |
    GroupDocs.Signature for .NET palaiko operacijas su šiais [failų formatais](https://docs.groupdocs.com/signature/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office formatai
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Vaizdai ir kiti formatai
        * **Nešiojami:** PDF
        * **Vaizdai:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Kiti biuro formatai:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Kiti formatai
        * **Žiniatinklis:** HTML, MHTML
        * **Archyvai:** ZIP, TAR, 7Z
        * **Sertifikatai:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Parašo funkcijos"
  description: "Greitas ir tikslus PDF, biuro dokumentų ir vaizdų pasirašymas"

  items:
    # feature loop
    - icon: "sign"
      title: "Dokumento pasirašymas"
      content: "Tiksliai pridėkite vieną ar kelis palaikomus parašų tipus bet kurioje nurodytoje verslo dokumentų vietoje."

    # feature loop
    - icon: "custom"
      title: "Tinkinkite parašus"
      content: "Norėdami sukonfigūruoti parašų išvaizdą, naudokite tokias funkcijas kaip spalva, šriftas, kraštinė, pasukimas ir kt."

    # feature loop
    - icon: "password"
      title: "Dokumento slaptažodžio apsauga"
      content: "Apsaugokite tam tikrų tipų dokumentus po pasirašymo nustatydami slaptažodį."

    # feature loop
    - icon: "protect"
      title: "Apsauga nuo pokyčių"
      content: "Neleiskite svarbių verslo dokumentų pakeitimų pridėję parašą su skaitmeniniu sertifikatu."

    # feature loop
    - icon: "convert"
      title: "Konvertuoti pasirašytus failus į kitus formatus"
      content: "Konvertuokite pasirašytus failus į norimus formatus, pvz., išsaugokite Word dokumentą kaip PDF."

    # feature loop
    - icon: "preview"
      title: "Ištraukite puslapių peržiūras"
      content: "Išskleiskite puslapius iš pasirašytų dokumentų kaip atskirus vaizdus, ​​​​kad galėtumėte juos apdoroti ateityje."

    # feature loop
    - icon: "search"
      title: "Parašo paieška dokumentuose"
      content: "Gaukite informaciją apie anksčiau pridėtus parašus konkrečiuose dokumentuose."

    # feature loop
    - icon: "validate"
      title: "Patvirtinti pasirašytus dokumentus"
      content: "Patikrinkite, ar tinkamai pasirašyti dokumentai, naudodami patvirtinimo funkcijas."

    # feature loop
    - icon: "update"
      title: "Atnaujinkite arba ištrinkite parašus"
      content: "Lengvai pakeiskite konkrečių parašų vietą puslapyje, keiskite jų tekstą arba ištrinkite juos be jokių problemų."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kodo pavyzdžiai"
  description: "Kai kurie .NET operacijoms naudojami tipiški GroupDocs.Signature atvejai"
  items:
    # code sample loop
    - title: "Pridėkite QR kodą prie PDF"
      content: |
        Pridėjus [QR kodus](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) prie konkrečių PDF dokumentų puslapių galima pagerinti verslo procesus. Toliau pateikiamas pavyzdys, kaip pridėti QR kodą naudojant GroupDocs.Signature.
        {{< landing/code title="Kaip įdėti QR kodą į PDF.">}}
        ```csharp {style=abap}
        // Įdėkite dokumentą pasirašyti
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Sukurkite QR kodo parinktis su iš anksto nustatytu tekstu
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Konfigūruokite QR kodo kodavimo tipą ir vietą puslapyje
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Pasirašykite dokumentą ir išsaugokite jį kaip rezultato failą
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX dokumento apsauga naudojant skaitmeninį sertifikatą"
      content: |
        Galite [Apsaugoti dokumentą](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) naudodami asmeninius arba įmonės parašus, saugomus kaip skaitmeninius sertifikatus. Tokie saugomi dokumentai negali būti modifikuojami nepakeitus parašo negaliojančiu.
        {{< landing/code title="Štai kaip užtikrinti dokumento vientisumą.">}}
        ```csharp {style=abap}   
        // Įkelkite dokumentą, kurį norite pasirašyti skaitmeniniu būdu
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // Nurodykite skaitmeninio pasirašymo parinktis ir nurodykite kelią į sertifikato failą
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Nustatykite sertifikato slaptažodį
                Password = "1234567890"
            };
            // Pasirašykite dokumentą ir išsaugokite jį norimame kelyje
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---
