---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:51
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: is
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
head_description: "Samþættu öruggar rafrænar undirskriftir í Node.js öppum með GroupDocs.Signature. Straumræða verkflæði undirritunar skjala á auðveldan og skilvirkan hátt."

############################# Header ############################
title: "Skrifaðu undir skjöl<br>með Node.js API"
description: "Skrifaðu undir stafræn skjöl og myndir á hvaða vettvang sem er með því að nota sveigjanleg API og app byggðar lausnir fyrir forritara og endanotendur."
words:
  for: "fyrir"

actions:
  main: "Sækja frá NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Leyfisveitingar"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Tilbúinn til að byrja?"
  description: "Prófaðu GroupDocs.Signature eiginleika ókeypis eða biddu um leyfi"

release:
  title: "Útgáfa {0} gefin út"
  notes: "Sjáðu hvað er nýtt"
  downloads: "Niðurhal"

code:
  title: "Að undirrita PDF-skjöl eftir Node.js"
  more: "Fleiri dæmi"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Veldu PDF skjal
    let signature = new Signature("sample.pdf");
    
    // Gefðu upp texta
    let options = new TextSignOptions("John Smith");
    
    // Stilltu lit
    options.ForeColor = Color.Red;
    
    // Skrifaðu undir skjal og vistaðu í skrá
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Yfirlit"
  description: "Skjöl undirritunarsafn sem er tilbúið til notkunar í Node.js forritum"
  features:
    # feature loop
    - title: "Stafræn undirskriftarlausn fyrir viðskiptaskjöl með Node.js"
      content: "GroupDocs.Signature for Node.js via Java býður upp á yfirgripsmikið sett af valkostum fyrir stafræna undirskrift fyrir PDF, Office skjöl og myndir. Texti, strikamerki, myndir, stafræn skilríki og lýsigögn eru í boði. Straumlínulagað skjalavinnsla tryggir skilvirkni."

    # feature loop
    - title: "Ítarleg meðferð á undirrituðum skjölum"
      content: "GroupDocs.Signature veitir þér heimild til að vinna úr undirrituðum skjölum. Leitaðu að og staðfestu undirskriftir með ýmsum forsendum. Að auki skaltu draga út nákvæmar skjalaupplýsingar eða búa til forskoðunarmyndir af síðum."

    # feature loop
    - title: "Fjölbreytt úttakssnið"
      content: "Lausnin okkar veitir víðtæka stjórn á framleiðslusniði undirritaðra skjala. Staðsetjið undirskriftir nákvæmlega á hvaða síðu sem er og sérsniðið útlit þeirra. Vistaðu undirrituð skjöl á fjölmörgum studdum sniðum og tryggðu þau mögulega með lykilorðum."

############################# Platforms ############################
platforms:
  enable: true
  title: "Sjálfstæði vettvangs"
  description: "GroupDocs.Signature for Node.js via Java framkvæmir skjalavinnslu með ýmsum stýrikerfum"
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
  title: "Stutt skráarsnið"
  description: |
    GroupDocs.Signature for Node.js via Java auðveldar aðgerðir fyrir [vinsæl skráarsnið](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office snið
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Myndir og önnur snið
        * **Færanlegt:** PDF
        * **Myndir:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Önnur skrifstofusnið:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Önnur snið
        * **vefur:** HTML, MHTML
        * **Skjalasafn:** ZIP, TAR, 7Z
        * **Skírteini:** PFX

############################# Features ############################
features:
  enable: true
  title: "Eiginleikar GroupDocs.Signature"
  description: "Skrifaðu undir PDF, Office skjöl og myndir með stafrænum undirskriftum"

  items:
    # feature loop
    - icon: "sign"
      title: "Undirskrift viðskipta"
      content: "Notaðu ýmsar undirskriftargerðir til að undirrita skjöl. Settu stafrænar undirskriftir nákvæmlega á hvaða síðu sem er."

    # feature loop
    - icon: "custom"
      title: "Sérsníða undirskriftarútlit"
      content: "Sérsníðaðu sjónræna þætti undirskrifta með því að stilla lit, leturgerð, ramma, snúning og fleira til að ná tilætluðum árangri."

    # feature loop
    - icon: "password"
      title: "Skjöl með lykilorði"
      content: "Fyrir mörg studd skjalasnið, vernda undirrituð skjöl með lykilorði til að auka öryggi."

    # feature loop
    - icon: "protect"
      title: "Koma í veg fyrir óleyfilegar breytingar"
      content: "Verndaðu mikilvæg viðskiptaskjöl undirrituð með stafrænum skilríkjum fyrir óheimilum breytingum."

    # feature loop
    - icon: "convert"
      title: "Æskileg úttakssnið"
      content: "Fáðu áreynslulaust undirrituð skjöl á hvaða studdu sniði sem er. Umbreyttu MS Word skjölum í PDF snið með auðveldum hætti."

    # feature loop
    - icon: "preview"
      title: "Skjalaforskoðun"
      content: "Vistaðu einstakar skjalasíður sem myndir fyrir framtíðarþarfir."

    # feature loop
    - icon: "search"
      title: "Undirskriftarleit"
      content: "Sæktu upplýsingar um áður bættar undirskriftir í skjölunum þínum."

    # feature loop
    - icon: "validate"
      title: "Staðfesting skjala"
      content: "Staðfestu áreiðanleika undirskrifta sem fram koma í hvaða skjali sem er."

    # feature loop
    - icon: "update"
      title: "Undirskriftarstjórnun"
      content: "Eyða, flytja eða breyta hvaða undirskrift sem er sett á hvaða skjalasíðu sem er."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kóða sýnishorn"
  description: "Lýsandi dæmi sem sýna dæmigerðar GroupDocs.Signature for Node.js via Java aðgerðir"
  items:
    # code sample loop
    - title: "Merktu PDF með QR kóða"
      content: |
        Með því að fella [strikamerkja](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) inn í sérstakar PDF skjalasíður getur það hagrætt viðskiptaferlum. Þessi hluti gefur dæmi um að bæta við QR kóða með því að nota GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Hvernig á að setja QR kóða á PDF.">}}
        ```javascript {style=abap}
        // Hladdu skjalinu til að undirrita
        let signature = new Signature("file_to_sign.pdf");
        
        // Búðu til QR kóða valkosti með fyrirfram skilgreindum texta
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Stilltu QR kóða kóðun gerð og staðsetningu á síðunni
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Skrifaðu undir skjalið og vistaðu það sem niðurstöðuskrá
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Að vernda DOCX með stafrænni undirskrift"
      content: |
        [Verndaðu skjölin þín](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) með undirskriftum byggðar á stafrænum skilríkjum. Stafræn undirskrift verndar viðskiptaskjölin þín gegn efnisbreytingum.
        {{< landing/code title="Hér er hvernig á að tryggja heilindi skjalsins.">}}
        ```javascript {style=abap}   
        // Hladdu skjalinu sem á að skrifa undir stafrænt
        let signature = new Signature("file_to_sign.docx");
        
        // Tilgreindu valkosti fyrir stafræna undirskrift og gefðu upp slóðina að vottorðaskránni
        let options = new DigitalSignOptions("certificate.pfx");

        // Stilltu lykilorð vottorðsins
        options.Password = "1234567890";

        // Skrifaðu undir skjalið og vistaðu það á viðkomandi slóð
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
