---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: lv
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
head_title: ".NET, Java, mākoņa API un tiešsaistes dokumentu parakstu lietotnes"
head_description: "Iegūstiet visu vienā dokumentu e-paraksta risinājumu .NET, Java un mākoņa lietojumprogrammām. Parakstiet izplatītos dokumentu formātus tiešsaistē, izmantojot vienkāršu vilkšanas un nomešanas funkciju"

############################# Header ############################
title: "Parakstiet dokumentus<br>ar Node.js API"
description: "Parakstiet digitālos dokumentus un attēlus jebkurā platformā, izmantojot mūsu elastīgās API un uz lietotnēm balstītus risinājumus programmētājiem un galalietotājiem."
words:
  for: "priekš"

actions:
  main: "Lejupielādēt no NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licencēšana"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Vai esat gatavs sākt?"
  description: "Izmēģiniet GroupDocs.Signature funkcijas bez maksas vai pieprasiet licenci"

release:
  title: "Izlaista versija {0}"
  notes: "Skatiet, kas jauns"
  downloads: "Lejupielādes"

code:
  title: "PDF failu parakstīšana, izmantojot Node.js"
  more: "Vairāk piemēru"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Atlasiet PDF dokumentu
    let signature = new Signature("sample.pdf");
    
    // Sniedziet tekstu
    let options = new TextSignOptions("John Smith");
    
    // Iestatīt krāsu
    options.ForeColor = Color.Red;
    
    // Parakstiet dokumentu un saglabājiet to failā
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Paraksta pārskats"
  description: "Dokumentu parakstīšanas bibliotēka, kas ir gatava lietošanai Node.js lietojumprogrammās"
  features:
    # feature loop
    - title: "Digitālā paraksta risinājums biznesa dokumentiem ar Node.js"
      content: "GroupDocs.Signature for Node.js via Java piedāvā plašu digitālā paraksta opciju kopumu PDF, Office dokumentiem un attēliem. Ir pieejams teksts, svītrkodi, attēli, digitālie sertifikāti un metadati. Racionalizēta dokumentu apstrāde nodrošina efektivitāti."

    # feature loop
    - title: "Uzlabotas manipulācijas ar parakstītiem dokumentiem"
      content: "GroupDocs.Signature sniedz jums iespēju apstrādāt parakstītus dokumentus. Meklējiet un apstipriniet parakstus, izmantojot dažādus kritērijus. Turklāt izņemiet detalizētu dokumenta informāciju vai ģenerējiet lapu priekšskatījuma attēlus."

    # feature loop
    - title: "Dažādi izvades formāti"
      content: "Mūsu risinājums nodrošina plašu parakstīto dokumentu izvades formāta kontroli. Precīzi novietojiet parakstus jebkurā lapā un pielāgojiet to izskatu. Saglabājiet parakstītos dokumentus daudzos atbalstītos formātos un pēc izvēles nostipriniet tos ar parolēm."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platformas neatkarība"
  description: "GroupDocs.Signature for Node.js via Java veic dokumentu apstrādi ar dažādām operētājsistēmām"
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
    GroupDocs.Signature for Node.js via Java atvieglo [populāro failu formātu](https://docs.groupdocs.com/signature/java/supported-document-formats/) darbības.
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
  title: "GroupDocs.Signature funkcijas"
  description: "Parakstiet PDF failus, Office dokumentus un attēlus ar ciparparakstiem"

  items:
    # feature loop
    - icon: "sign"
      title: "Biznesa paraksti"
      content: "Dokumentu parakstīšanai izmantojiet dažādus parakstu veidus. Precīzi ievietojiet ciparparakstus jebkurā lapas vietā."

    # feature loop
    - icon: "custom"
      title: "Paraksta izskata pielāgošana"
      content: "Pielāgojiet parakstu vizuālos aspektus, pielāgojot krāsu, fontu, apmales, rotāciju un daudz ko citu, lai sasniegtu vēlamo rezultātu."

    # feature loop
    - icon: "password"
      title: "Ar paroli aizsargāti dokumenti"
      content: "Daudziem atbalstītajiem dokumentu formātiem parakstītos dokumentus aizsargājiet ar paroli, lai nodrošinātu papildu drošību."

    # feature loop
    - icon: "protect"
      title: "Neatļautu modifikāciju novēršana"
      content: "Aizsargājiet svarīgus biznesa dokumentus, kas parakstīti ar digitālajiem sertifikātiem, no nesankcionētām izmaiņām."

    # feature loop
    - icon: "convert"
      title: "Vēlamie izvades formāti"
      content: "Bez pūlēm iegūstiet parakstītus dokumentus jebkurā atbalstītā formātā. Ērti konvertējiet MS Word dokumentus PDF formātā."

    # feature loop
    - icon: "preview"
      title: "Dokumentu priekšskatīšana"
      content: "Saglabājiet atsevišķas dokumentu lapas kā attēlus nākotnes vajadzībām."

    # feature loop
    - icon: "search"
      title: "Parakstu meklēšana"
      content: "Izgūstiet informāciju par iepriekš pievienotajiem parakstiem savos dokumentos."

    # feature loop
    - icon: "validate"
      title: "Dokumentu apstiprināšana"
      content: "Pārbaudiet jebkurā dokumentā uzrādīto parakstu autentiskumu."

    # feature loop
    - icon: "update"
      title: "Parakstu pārvaldība"
      content: "Dzēsiet, pārvietojiet vai modificējiet parakstus, kas ievietoti jebkurā dokumenta lapā."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Koda paraugi"
  description: "Ilustratīvi piemēri, kas parāda tipiskas GroupDocs.Signature for Node.js via Java darbības"
  items:
    # code sample loop
    - title: "Atzīmējiet PDF ar QR kodiem"
      content: |
        [Svītrkodu](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) iekļaušana konkrētās PDF dokumentu lapās var racionalizēt biznesa procesus. Šajā sadaļā ir sniegts piemērs QR koda pievienošanai, izmantojot GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Kā ievietot QR kodu PDF failā.">}}
        ```javascript {style=abap}
        // Ievietojiet dokumentu parakstīšanai
        let signature = new Signature("file_to_sign.pdf");
        
        // Izveidojiet QR koda opcijas ar iepriekš definētu tekstu
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurējiet QR koda kodēšanas veidu un pozīciju lapā
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Parakstiet dokumentu un saglabājiet to kā rezultāta failu
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX aizsardzība ar digitālo parakstu"
      content: |
        [Aizsargājiet savus dokumentus](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) ar parakstiem, kuru pamatā ir ciparsertifikāti. Digitālais paraksts aizsargā jūsu biznesa dokumentus pret satura izmaiņām.
        {{< landing/code title="Lūk, kā nodrošināt dokumenta integritāti.">}}
        ```javascript {style=abap}   
        // Ielādējiet dokumentu, kas jāparaksta digitāli
        let signature = new Signature("file_to_sign.docx");
        
        // Norādiet ciparparaksta opcijas un norādiet ceļu uz sertifikāta failu
        let options = new DigitalSignOptions("certificate.pfx");

        // Iestatiet sertifikāta paroli
        options.Password = "1234567890";

        // Parakstiet dokumentu un saglabājiet to vajadzīgajā ceļā
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
