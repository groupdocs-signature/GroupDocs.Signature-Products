---
############################# Static ############################
layout: "landing"
date: 2024-02-29T14:43:07
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: lv
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
head_title: ".NET, Java, mākoņa API un tiešsaistes dokumentu parakstu lietotnes"
head_description: "Iegūstiet visu vienā dokumentu e-paraksta risinājumu .NET, Java un mākoņa lietojumprogrammām. Parakstiet izplatītos dokumentu formātus tiešsaistē, izmantojot vienkāršu vilkšanas un nomešanas funkciju"

############################# Header ############################
title: "Parakstiet dokumentus<br>izmantojot .NET API"
description: "Parakstiet digitālos dokumentus un attēlus jebkurā platformā, izmantojot mūsu elastīgās API un uz lietotnēm balstītus risinājumus programmētājiem un galalietotājiem."
words:
  for: "priekš"

actions:
  main: "Bezmaksas NuGet lejupielāde"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licencēšana"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Vai esat gatavs sākt?"
  description: "Izmēģiniet GroupDocs.Signature funkcijas bez maksas vai pieprasiet licenci"

release:
  title: "Izlaista versija {0}"
  notes: "Skatiet, kas jauns"
  downloads: "Lejupielādes"

code:
  title: "Parakstīt PDF failus C#"
  more: "Vairāk piemēru"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Atlasiet PDF dokumentu
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Sniedziet tekstu
        var options = new TextSignOptions("John Smith")
        {
            // Iestatīt krāsu
            ForeColor = Color.Red
        };
        // Parakstiet dokumentu un saglabājiet to failā
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Paraksta pārskats"
  description: "API dokumentu parakstīšanas un saistīto darbību veikšanai .NET lietojumprogrammās"
  features:
    # feature loop
    - title: "Parakstu pievienošana biznesa dokumentiem C#"
      content: "Dokumentu parakstīšana: Izmantojot GroupDocs.Signature for .NET, varat pievienot dažādu veidu parakstus, piemēram, tekstu, attēlus, svītrkodus un digitālos sertifikātus, PDF un Office dokumentiem. Šī API ļauj parakstīt dokumentus ar gandrīz jebkura veida datiem, tostarp slēptiem metadatiem."

    # feature loop
    - title: "Parakstīto dokumentu apstrāde"
      content: "Papildu apstrāde: varat veikt spēcīgas darbības ar parakstītiem dokumentiem, izmantojot GroupDocs.Signature. Tas ietver esošo parakstu meklēšanu biznesa dokumentos un to pārbaudi, izmantojot īpašus kritērijus. Turklāt, izmantojot šo .NET API, varat izgūt dokumenta informāciju un priekšskatīt lapas."

    # feature loop
    - title: "Rezultātu pielāgošana"
      content: "GroupDocs.Signature for .NET piedāvā plašas pielāgošanas iespējas. Varat precīzi novietot parakstus jebkurā dokumenta lapā un pielāgot to izskatu, izmantojot dažādus iestatījumus. Turklāt šī API atbalsta apstrādāto dokumentu saglabāšanu plašā atbalstīto formātu klāstā."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platformas neatkarība"
  description: "GroupDocs.Signature for .NET atbalsta šādas operētājsistēmas, ietvarus un pakotņu pārvaldniekus"
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
  title: "Atbalstītie failu formāti"
  description: |
    GroupDocs.Signature for .NET atbalsta darbības ar šādiem [failu formātiem](https://docs.groupdocs.com/signature/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office formāti
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Attēli un citi formāti
        * **Pārnēsājams:** PDF
        * **Attēli:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Citi biroja formāti:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Citi formāti
        * **Web:** HTML, MHTML
        * **Arhīvi:** ZIP, TAR, 7Z
        * **Sertifikāti:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Paraksta funkcijas"
  description: "Ātra un precīza PDF, Office dokumentu un attēlu parakstīšana"

  items:
    # feature loop
    - icon: "sign"
      title: "Dokumentu parakstīšana"
      content: "Precīzi pievienojiet vienu vai vairākus atbalstītos parakstu veidus jebkurā norādītajā biznesa dokumentu pozīcijā."

    # feature loop
    - icon: "custom"
      title: "Pielāgojiet parakstus"
      content: "Izmantojiet tādas funkcijas kā krāsa, fonts, apmale, pagriešana utt., lai konfigurētu parakstu izskatu."

    # feature loop
    - icon: "password"
      title: "Dokumenta paroles aizsardzība"
      content: "Nodrošiniet noteiktus dokumentu veidus, pēc parakstīšanas iestatot paroli."

    # feature loop
    - icon: "protect"
      title: "Aizsardzība pret izmaiņām"
      content: "Novērsiet izmaiņas svarīgos biznesa dokumentos pēc paraksta pievienošanas ar digitālo sertifikātu."

    # feature loop
    - icon: "convert"
      title: "Konvertējiet parakstītos failus citos formātos"
      content: "Konvertējiet parakstītos failus vajadzīgajos formātos, piemēram, saglabājiet Word dokumentu kā PDF."

    # feature loop
    - icon: "preview"
      title: "Izvilkt lapu priekšskatījumus"
      content: "Izņemiet lapas no parakstītiem dokumentiem kā atsevišķus attēlus turpmākai apstrādei."

    # feature loop
    - icon: "search"
      title: "Parakstu meklēšana dokumentos"
      content: "Izgūt informāciju par iepriekš pievienotajiem parakstiem konkrētos dokumentos."

    # feature loop
    - icon: "validate"
      title: "Apstipriniet parakstītos dokumentus"
      content: "Pārbaudiet dokumentu pareizu parakstīšanu, izmantojot validācijas līdzekļus."

    # feature loop
    - icon: "update"
      title: "Atjauniniet vai dzēsiet parakstus"
      content: "Ērti pārvietojiet konkrētus parakstus lapā, mainiet to tekstu vai izdzēsiet tos bez problēmām."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Koda paraugi"
  description: "Daži tipiski GroupDocs.Signature izmantošanas gadījumi .NET operācijām"
  items:
    # code sample loop
    - title: "Pievienojiet QR kodu PDF failam"
      content: |
        [QR-kodu](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) pievienošana noteiktām PDF dokumentu lapām var uzlabot biznesa procesus. Tālāk ir sniegts piemērs, kā pievienot QR kodu, izmantojot GroupDocs.Signature.
        {{< landing/code title="Kā ievietot QR kodu PDF failā.">}}
        ```csharp {style=abap}
        // Ievietojiet dokumentu parakstīšanai
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Izveidojiet QR koda opcijas ar iepriekš definētu tekstu
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Konfigurējiet QR koda kodēšanas veidu un pozīciju lapā
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Parakstiet dokumentu un saglabājiet to kā rezultāta failu
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX dokumenta aizsardzība, izmantojot digitālo sertifikātu"
      content: |
        Varat [Aizsargāt dokumentu](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/), izmantojot personiskos vai korporatīvos parakstus, kas saglabāti kā ciparsertifikāti. Šādus aizsargātus dokumentus nevar mainīt, nepadarot parakstu par nederīgu.
        {{< landing/code title="Lūk, kā nodrošināt dokumenta integritāti.">}}
        ```csharp {style=abap}   
        // Ielādējiet dokumentu, kas jāparaksta digitāli
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Norādiet ciparparaksta opcijas un norādiet ceļu uz sertifikāta failu
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Iestatiet sertifikāta paroli
                Password = "1234567890"
            };
            // Parakstiet dokumentu un saglabājiet to vajadzīgajā ceļā
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
