---
############################# Static ############################
layout: "landing"
date: 2024-02-29T14:43:07
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: da
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
head_title: ".NET, Java, Cloud API'er og online dokumentsignaturapps"
head_description: "Få alt-i-et dokument-e-signaturløsning til .NET, Java og cloud-baserede applikationer. Signer almindelige dokumentformater online ved hjælp af simpel træk og slip-funktion"

############################# Header ############################
title: "Underskriv dokumenter<br>via .NET API"
description: "Signer digitale dokumenter og billeder på enhver platform ved hjælp af vores fleksible API'er og app-baserede løsninger til programmører og slutbrugere."
words:
  for: "til"

actions:
  main: "Gratis download af NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licensering"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Klar til at komme i gang?"
  description: "Prøv GroupDocs.Signature-funktioner gratis, eller anmod om en licens"

release:
  title: "Version {0} frigivet"
  notes: "Se, hvad der er nyt"
  downloads: "Downloads"

code:
  title: "Signer PDF-filer i C#"
  more: "Flere eksempler"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Vælg PDF-dokument
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Giv tekst
        var options = new TextSignOptions("John Smith")
        {
            // Indstil farve
            ForeColor = Color.Red
        };
        // Underskriv dokument og gem til fil
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signatur Oversigt"
  description: "API til udførelse af dokumentsignering og relaterede operationer i .NET-applikationer"
  features:
    # feature loop
    - title: "Tilføjelse af signaturer til forretningsdokumenter i C#"
      content: "Dokumentsignering: Med GroupDocs.Signature til .NET kan du tilføje forskellige typer signaturer, såsom tekst, billeder, stregkoder og digitale certifikater, til PDF- og Office-dokumenter. Denne API giver dig mulighed for at signere dine dokumenter med næsten enhver datatype, inklusive skjulte metadata."

    # feature loop
    - title: "Behandling af underskrevne dokumenter"
      content: "Yderligere behandling: Du kan udføre kraftfulde handlinger på signerede dokumenter ved hjælp af GroupDocs.Signature. Dette omfatter søgning efter eksisterende signaturer i forretningsdokumenter og verificering af dem ved hjælp af specifikke kriterier. Derudover kan du hente dokumentoplysninger og forhåndsvise sider gennem denne .NET API."

    # feature loop
    - title: "Tilpasning af resultater"
      content: "GroupDocs.Signature til .NET tilbyder omfattende tilpasningsmuligheder. Du kan præcist placere signaturer hvor som helst på en dokumentside og justere deres udseende ved hjælp af en række forskellige indstillinger. Desuden understøtter denne API lagring af behandlede dokumenter i en lang række understøttede formater."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platformens uafhængighed"
  description: "GroupDocs.Signature til .NET understøtter følgende operativsystemer, rammer og pakkeadministratorer"
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
  title: "Understøttede filformater"
  description: |
    GroupDocs.Signature til .NET understøtter operationer med følgende [filformater](https://docs.groupdocs.com/signature/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office-formater
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Billeder og andre formater
        * **Transportabel:** PDF
        * **Billeder:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Andre kontorformater:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Andre formater
        * **Web:** HTML, MHTML
        * **Arkiv:** ZIP, TAR, 7Z
        * **Certifikater:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature funktioner"
  description: "Signering af PDF'er, Office-dokumenter og billeder hurtigt og præcist"

  items:
    # feature loop
    - icon: "sign"
      title: "Dokumentunderskrivelse"
      content: "Tilføj en eller flere understøttede typer signaturer nøjagtigt på enhver specificeret position på forretningsdokumenter."

    # feature loop
    - icon: "custom"
      title: "Tilpas signaturer"
      content: "Brug funktioner som farve, skrifttype, kant, rotation osv. til at konfigurere udseendet af signaturer."

    # feature loop
    - icon: "password"
      title: "Dokumentadgangskodebeskyttelse"
      content: "Sikre visse dokumenttyper ved at angive en adgangskode efter signering."

    # feature loop
    - icon: "protect"
      title: "Beskyttelse mod ændringer"
      content: "Forhindr ændringer af vigtige forretningsdokumenter efter tilføjelse af en signatur med et digitalt certifikat."

    # feature loop
    - icon: "convert"
      title: "Konverter signerede filer til andre formater"
      content: "Konverter signerede filer til ønskede formater, såsom at gemme et Word-dokument som en PDF."

    # feature loop
    - icon: "preview"
      title: "Uddrag sideforhåndsvisninger"
      content: "Uddrag sider fra underskrevne dokumenter som individuelle billeder til fremtidig behandling."

    # feature loop
    - icon: "search"
      title: "Signatursøgning i dokumenter"
      content: "Hent information om tidligere tilføjede signaturer i specifikke dokumenter."

    # feature loop
    - icon: "validate"
      title: "Validere underskrevne dokumenter"
      content: "Bekræft den korrekte underskrift af dokumenter ved hjælp af valideringsfunktioner."

    # feature loop
    - icon: "update"
      title: "Opdater eller slet signaturer"
      content: "Flyt nemt bestemte signaturer på en side, rediger deres tekst eller slet dem uden problemer."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kodeprøver"
  description: "Nogle bruger eksempler på typiske GroupDocs.Signature til .NET-operationer"
  items:
    # code sample loop
    - title: "Tilføj QR-kode til PDF"
      content: |
        Tilføjelse af [QR-koder](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) til specifikke sider med PDF-dokumenter kan forbedre forretningsprocesser. Nedenfor er et eksempel på, hvordan man tilføjer en QR-kode ved hjælp af GroupDocs.Signature.
        {{< landing/code title="Sådan sætter du QR-kode til PDF.">}}
        ```csharp {style=abap}
        // Indlæs dokumentet for at underskrive
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Opret QR-kodeindstillinger med foruddefineret tekst
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Konfigurer QR-kodekodningstype og position på siden
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Underskriv dokumentet og gem det som resultatfil
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Beskyttelse af et DOCX-dokument ved hjælp af et digitalt certifikat"
      content: |
        Du kan [Beskyt et dokument](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) ved hjælp af personlige eller virksomhedssignaturer gemt som digitale certifikater. Sådanne beskyttede dokumenter kan ikke ændres uden at gøre signaturen ugyldig.
        {{< landing/code title="Sådan sikrer du dokumentets integritet.">}}
        ```csharp {style=abap}   
        // Indlæs dokumentet, der skal signeres digitalt
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Angiv muligheder for digital signering, og angiv stien til certifikatfilen
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Indstil certifikatets adgangskode
                Password = "1234567890"
            };
            // Underskriv dokumentet og gem det på den ønskede sti
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
