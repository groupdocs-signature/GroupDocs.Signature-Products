---
############################# Static ############################
layout: "landing"
date: 2024-02-29T14:43:07
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: no
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
head_title: ".NET, Java, Cloud APIer og nettbaserte dokumentsignaturapper"
head_description: "Få alt-i-ett dokument-e-signaturløsning for .NET, Java og skybaserte applikasjoner. Signer vanlige dokumentformater på nettet ved hjelp av enkel dra og slipp-funksjon"

############################# Header ############################
title: "Signer dokumenter<br>via .NET API"
description: "Signer digitale dokumenter og bilder på hvilken som helst plattform ved å bruke våre fleksible APIer og appbaserte løsninger for programmerere og sluttbrukere."
words:
  for: "til"

actions:
  main: "Gratis nedlasting av NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Lisensering"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Klar til å komme i gang?"
  description: "Prøv GroupDocs.Signature-funksjonene gratis eller be om en lisens"

release:
  title: "Versjon {0} utgitt"
  notes: "Se hva som er nytt"
  downloads: "Nedlastinger"

code:
  title: "Signer PDF-filer i C#"
  more: "Flere eksempler"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Velg PDF-dokument
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Gi tekst
        var options = new TextSignOptions("John Smith")
        {
            // Sett farge
            ForeColor = Color.Red
        };
        // Signer dokument og lagre til fil
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Oversikt"
  description: "API for å utføre dokumentsignering og relaterte operasjoner i .NET-applikasjoner"
  features:
    # feature loop
    - title: "Legge til signaturer til forretningsdokumenter i C#"
      content: "Dokumentsignering: Med GroupDocs.Signature for .NET kan du legge til ulike typer signaturer, som tekst, bilder, strekkoder og digitale sertifikater, til PDF- og Office-dokumenter. Denne API-en lar deg signere dokumentene dine med nesten alle typer data, inkludert skjulte metadata."

    # feature loop
    - title: "Behandling av signerte dokumenter"
      content: "Ytterligere behandling: Du kan utføre kraftige operasjoner på signerte dokumenter ved å bruke GroupDocs.Signature. Dette inkluderer å søke etter eksisterende signaturer i forretningsdokumenter og verifisere dem ved å bruke spesifikke kriterier. I tillegg kan du hente dokumentinformasjon og forhåndsvise sider gjennom denne .NET API."

    # feature loop
    - title: "Tilpasse resultater"
      content: "GroupDocs.Signature for .NET tilbyr omfattende tilpasningsmuligheter. Du kan plassere signaturer nøyaktig hvor som helst på en dokumentside og justere utseendet ved hjelp av en rekke innstillinger. Videre støtter denne API-en lagring av behandlede dokumenter i et bredt spekter av støttede formater."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformuavhengighet"
  description: "GroupDocs.Signature for .NET støtter følgende operativsystemer, rammeverk og pakkeadministratorer"
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
  title: "Støttede filformater"
  description: |
    GroupDocs.Signature for .NET støtter operasjoner med følgende [filformater](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
        ### Bilder og andre formater
        * **Bærbar:** PDF
        * **Bilder:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Andre kontorformater:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Andre formater
        * **Web:** HTML, MHTML
        * **Arkiv:** ZIP, TAR, 7Z
        * **Sertifikater:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature-funksjoner"
  description: "Signering av PDF-er, Office-dokumenter og bilder raskt og nøyaktig"

  items:
    # feature loop
    - icon: "sign"
      title: "Dokumentsignering"
      content: "Legg til én eller flere støttede typer signaturer nøyaktig på en hvilken som helst spesifisert posisjon på forretningsdokumenter."

    # feature loop
    - icon: "custom"
      title: "Tilpass signaturer"
      content: "Bruk funksjoner som farge, font, kantlinje, rotasjon osv. for å konfigurere utseendet til signaturer."

    # feature loop
    - icon: "password"
      title: "Dokumentpassordbeskyttelse"
      content: "Sikre visse dokumenttyper ved å angi et passord etter signering."

    # feature loop
    - icon: "protect"
      title: "Beskyttelse mot endringer"
      content: "Forhindre endringer i viktige forretningsdokumenter etter å ha lagt til en signatur med et digitalt sertifikat."

    # feature loop
    - icon: "convert"
      title: "Konverter signerte filer til andre formater"
      content: "Konverter signerte filer til ønskede formater, for eksempel å lagre et Word-dokument som en PDF."

    # feature loop
    - icon: "preview"
      title: "Trekk ut forhåndsvisninger av siden"
      content: "Trekk ut sider fra signerte dokumenter som individuelle bilder for fremtidig behandling."

    # feature loop
    - icon: "search"
      title: "Signatursøk i dokumenter"
      content: "Hent informasjon om tidligere lagt til signaturer i spesifikke dokumenter."

    # feature loop
    - icon: "validate"
      title: "Validere signerte dokumenter"
      content: "Bekreft riktig signering av dokumenter ved hjelp av valideringsfunksjoner."

    # feature loop
    - icon: "update"
      title: "Oppdater eller slett signaturer"
      content: "Flytt enkelt spesifikke signaturer på en side, endre teksten eller slett dem uten problemer."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kodeprøver"
  description: "Noen bruker tilfeller av typiske GroupDocs.Signature for .NET-operasjoner"
  items:
    # code sample loop
    - title: "Legg til QR-kode i PDF"
      content: |
        Å legge til [QR-koder](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) til bestemte sider med PDF-dokumenter kan forbedre forretningsprosessene. Nedenfor er et eksempel på hvordan du legger til en QR-kode ved hjelp av GroupDocs.Signature.
        {{< landing/code title="Hvordan sette QR-kode til PDF.">}}
        ```csharp {style=abap}
        // Last inn dokumentet for å signere
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Lag QR-kodealternativer med forhåndsdefinert tekst
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Konfigurer QR-kodekodingstype og plassering på siden
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Signer dokumentet og lagre det som resultatfil
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Beskytte et DOCX-dokument ved hjelp av et digitalt sertifikat"
      content: |
        Du kan [Beskytt et dokument](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) ved å bruke personlige eller bedriftssignaturer lagret som digitale sertifikater. Slike beskyttede dokumenter kan ikke endres uten å ugyldiggjøre signaturen.
        {{< landing/code title="Slik sikrer du dokumentets integritet.">}}
        ```csharp {style=abap}   
        // Last inn dokumentet som skal signeres digitalt
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Angi alternativer for digital signering og oppgi banen til sertifikatfilen
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Angi sertifikatpassordet
                Password = "1234567890"
            };
            // Signer dokumentet og lagre det på ønsket bane
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
