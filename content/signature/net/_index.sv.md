---
############################# Static ############################
layout: "landing"
date: 2023-09-13T10:36:52
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: sv
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, Cloud API och onlinedokumentsignaturappar"
head_description: "Få en allt-i-ett-dokumentlösning för e-signaturer för .NET, Java och molnbaserade applikationer. Signera vanliga dokumentformat online med en enkel dra och släpp-funktion"

############################# Header ############################
title: "Signera dokument<br>via .NET API"
description: "Signera digitala dokument och bilder på vilken plattform som helst med hjälp av våra flexibla API:er och appbaserade lösningar för programmerare och slutanvändare."
words:
  for: "för"

actions:
  main: "Gratis nedladdning av NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licensiering"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Redo att komma igång?"
  description: "Prova GroupDocs.Signature-funktioner gratis eller begär en licens"

release:
  title: "Version {0} släpptes"
  notes: "Se vad som är nytt"
  downloads: "Nedladdningar"

code:
  title: "Signera PDF-filer i C#"
  more: "Fler exempel"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Välj PDF-dokument
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Ge text
        var options = new TextSignOptions("John Smith")
        {
            // Ställ in färg
            ForeColor = Color.Red
        };
        // Signera dokument och spara till fil
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Översikt"
  description: "API för att utföra dokumentsignering och relaterade operationer i .NET-applikationer"
  features:
    # feature loop
    - title: "Lägga till signaturer till affärsdokument i C#"
      content: "Dokumentsignering: Med GroupDocs.Signature för .NET kan du lägga till olika typer av signaturer, som text, bilder, streckkoder och digitala certifikat, till PDF- och Office-dokument. Detta API låter dig signera dina dokument med nästan vilken datatyp som helst, inklusive dolda metadata."

    # feature loop
    - title: "Bearbetar undertecknade dokument"
      content: "Ytterligare bearbetning: Du kan utföra kraftfulla operationer på signerade dokument med GroupDocs.Signature. Detta inkluderar att söka efter befintliga signaturer i affärsdokument och verifiera dem med hjälp av specifika kriterier. Dessutom kan du hämta dokumentinformation och förhandsgranska sidor genom detta .NET API."

    # feature loop
    - title: "Anpassa resultat"
      content: "GroupDocs.Signature för .NET erbjuder omfattande anpassningsmöjligheter. Du kan exakt placera signaturer var som helst på en dokumentsida och justera deras utseende med en mängd olika inställningar. Dessutom stöder detta API att spara bearbetade dokument i ett brett utbud av format som stöds."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformsoberoende"
  description: "GroupDocs.Signature för .NET stöder följande operativsystem, ramverk och pakethanterare"
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
  title: "Filformat som stöds"
  description: |
    GroupDocs.Signature for .NET stöder operationer med följande [filformat](https://docs.groupdocs.com/signature/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office-format
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Bilder och andra format
        * **Bärbar:** PDF
        * **Bilder:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Andra kontorsformat:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Andra format
        * **webb:** HTML, MHTML
        * **Arkiv:** ZIP, TAR, 7Z
        * **Certifikat:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature-funktioner"
  description: "Signera PDF-filer, Office-dokument och bilder snabbt och exakt"

  items:
    # feature loop
    - icon: "merge"
      title: "Dokumentsignering"
      content: "Lägg till en eller flera typer av signaturer som stöds exakt på valfri specificerad plats på affärsdokument."

    # feature loop
    - icon: "split"
      title: "Anpassa signaturer"
      content: "Använd funktioner som färg, typsnitt, kantlinje, rotation etc. för att konfigurera utseendet på signaturer."

    # feature loop
    - icon: "move"
      title: "Dokumentlösenordsskydd"
      content: "Säkra vissa dokumenttyper genom att ange ett lösenord efter signering."

    # feature loop
    - icon: "remove"
      title: "Skydd mot förändringar"
      content: "Förhindra ändringar i viktiga affärsdokument efter att du har lagt till en signatur med ett digitalt certifikat."

    # feature loop
    - icon: "rotate"
      title: "Konvertera signerade filer till andra format"
      content: "Konvertera signerade filer till önskade format, till exempel att spara ett Word-dokument som en PDF."

    # feature loop
    - icon: "swap"
      title: "Extrahera förhandsvisningar av sidan"
      content: "Extrahera sidor från signerade dokument som individuella bilder för framtida bearbetning."

    # feature loop
    - icon: "extract"
      title: "Signatursökning i dokument"
      content: "Hämta information om tidigare tillagda signaturer i specifika dokument."

    # feature loop
    - icon: "orientation"
      title: "Validera undertecknade dokument"
      content: "Verifiera korrekt signering av dokument med hjälp av valideringsfunktioner."

    # feature loop
    - icon: "preview"
      title: "Uppdatera eller ta bort signaturer"
      content: "Placera enkelt specifika signaturer på en sida, ändra deras text eller ta bort dem utan problem."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kodprover"
  description: "Vissa använder fall av typiska GroupDocs.Signature för .NET-operationer"
  items:
    # code sample loop
    - title: "Lägg till QR-kod till PDF"
      content: |
        Att lägga till [QR-koder](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) på specifika sidor med PDF-dokument kan förbättra affärsprocesserna. Nedan är ett exempel på hur man lägger till en QR-kod med GroupDocs.Signature.
        {{< landing/code title="Hur man lägger QR-kod till PDF.">}}
        ```csharp {style=abap}
        // Ladda dokumentet för att signera
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Skapa QR-kodalternativ med fördefinierad text
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Konfigurera QR-kodskodningstyp och position på sidan
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Signera dokumentet och spara det som resultatfil
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Skydda ett DOCX-dokument med ett digitalt certifikat"
      content: |
        Du kan [Skydda ett dokument](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) genom att använda personliga eller företagssignaturer lagrade som digitala certifikat. Sådana skyddade dokument kan inte ändras utan att signaturen ogiltigförklaras.
        {{< landing/code title="Så här säkerställer du dokumentintegritet.">}}
        ```csharp {style=abap}   
        // Ladda dokumentet som ska signeras digitalt
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Ange alternativ för digital signering och ange sökvägen till certifikatfilen
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Ställ in certifikatlösenordet
                Password = "1234567890"
            };
            // Signera dokumentet och spara det på önskad sökväg
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
