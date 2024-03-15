---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:51
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: sv
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
head_title: "Node.js Digital Signature API - GroupDocs.Signature"
head_description: "Integrera säkra e-signaturer i Node.js-appar med GroupDocs.Signature. Effektivisera arbetsflöden för dokumentsignering enkelt och effektivt."

############################# Header ############################
title: "Signera dokument<br>med Node.js API"
description: "Signera digitala dokument och bilder på vilken plattform som helst med hjälp av våra flexibla API:er och appbaserade lösningar för programmerare och slutanvändare."
words:
  for: "för"

actions:
  main: "Ladda ner från NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licensiering"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Redo att komma igång?"
  description: "Prova GroupDocs.Signature-funktioner gratis eller begär en licens"

release:
  title: "Version {0} släpptes"
  notes: "Se vad som är nytt"
  downloads: "Nedladdningar"

code:
  title: "Signera PDF-filer av Node.js"
  more: "Fler exempel"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Välj PDF-dokument
    let signature = new Signature("sample.pdf");
    
    // Ge text
    let options = new TextSignOptions("John Smith");
    
    // Ställ in färg
    options.ForeColor = Color.Red;
    
    // Signera dokument och spara till fil
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Översikt"
  description: "Dokumentsigneringsbibliotek som är redo att användas i Node.js-applikationer"
  features:
    # feature loop
    - title: "Digital signaturlösning för affärsdokument med Node.js"
      content: "GroupDocs.Signature for Node.js via Java erbjuder en omfattande uppsättning digitala signaturalternativ för PDF, Office-dokument och bilder. Text, streckkoder, bilder, digitala certifikat och metadata finns tillgängliga. Effektiviserad dokumentbehandling säkerställer effektivitet."

    # feature loop
    - title: "Avancerad manipulering av signerade dokument"
      content: "GroupDocs.Signature ger dig befogenhet att behandla undertecknade dokument. Sök och validera signaturer med hjälp av olika kriterier. Extrahera dessutom detaljerad dokumentinformation eller generera förhandsvisningsbilder av sidor."

    # feature loop
    - title: "Olika utdataformat"
      content: "Vår lösning ger omfattande kontroll över utdataformatet för signerade dokument. Placera signaturer exakt på vilken sida som helst och anpassa deras utseende. Spara undertecknade dokument i flera format som stöds och säkra dem eventuellt med lösenord."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformsoberoende"
  description: "GroupDocs.Signature for Node.js via Java utför dokumentbehandling med olika operativsystem"
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
    GroupDocs.Signature for Node.js via Java underlättar operationer för [populära filformat](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "Funktioner hos GroupDocs.Signature"
  description: "Signera PDF-filer, Office-dokument och bilder med digitala signaturer"

  items:
    # feature loop
    - icon: "sign"
      title: "Affärssignaturer"
      content: "Använd olika signaturtyper för att signera dokument. Placera digitala signaturer exakt på vilken sida som helst."

    # feature loop
    - icon: "custom"
      title: "Anpassa signaturens utseende"
      content: "Skräddarsy de visuella aspekterna av signaturer genom att justera färg, teckensnitt, ramar, rotation och mer för att uppnå önskat resultat."

    # feature loop
    - icon: "password"
      title: "Lösenordsskyddade dokument"
      content: "För många dokumentformat som stöds, skydda signerade dokument med ett lösenord för ökad säkerhet."

    # feature loop
    - icon: "protect"
      title: "Förhindra obehöriga ändringar"
      content: "Skydda viktiga affärsdokument signerade med digitala certifikat från obehöriga ändringar."

    # feature loop
    - icon: "convert"
      title: "Önskade utdataformat"
      content: "Få signerade dokument utan ansträngning i alla format som stöds. Konvertera MS Word-dokument till PDF-format med lätthet."

    # feature loop
    - icon: "preview"
      title: "Förhandsgranskning av dokument"
      content: "Spara enskilda dokumentsidor som bilder för framtida behov."

    # feature loop
    - icon: "search"
      title: "Signatursökning"
      content: "Hämta information om tidigare tillagda signaturer i dina dokument."

    # feature loop
    - icon: "validate"
      title: "Dokumentvalidering"
      content: "Verifiera äktheten av signaturer som presenteras i alla dokument."

    # feature loop
    - icon: "update"
      title: "Signaturhantering"
      content: "Ta bort, flytta eller ändra alla signaturer som placerats på en dokumentsida."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kodprover"
  description: "Illustrativa exempel som visar typiska GroupDocs.Signature for Node.js via Java-operationer"
  items:
    # code sample loop
    - title: "Markera PDF med QR-koder"
      content: |
        Att integrera [streckkoder](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) i specifika PDF-dokumentsidor kan effektivisera affärsprocesser. Det här avsnittet ger ett exempel på hur du lägger till en QR-kod med GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Hur man lägger QR-kod till PDF.">}}
        ```javascript {style=abap}
        // Ladda dokumentet för att signera
        let signature = new Signature("file_to_sign.pdf");
        
        // Skapa QR-kodalternativ med fördefinierad text
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurera QR-kodskodningstyp och position på sidan
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Signera dokumentet och spara det som resultatfil
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Skydda en DOCX med en digital signatur"
      content: |
        [Skydda dina dokument](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) genom signaturer baserade på digitala certifikat. Digital signatur skyddar dina affärsdokument mot att innehållet ändras.
        {{< landing/code title="Så här säkerställer du dokumentintegritet.">}}
        ```javascript {style=abap}   
        // Ladda dokumentet som ska signeras digitalt
        let signature = new Signature("file_to_sign.docx");
        
        // Ange alternativ för digital signering och ange sökvägen till certifikatfilen
        let options = new DigitalSignOptions("certificate.pfx");

        // Ställ in certifikatlösenordet
        options.Password = "1234567890";

        // Signera dokumentet och spara det på önskad sökväg
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
