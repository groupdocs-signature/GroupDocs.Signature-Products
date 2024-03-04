---
############################# Static ############################
layout: "landing"
date: 2024-03-04T17:52:03
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: et
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
head_title: ".NET, Java, pilve API-d ja veebipõhised dokumendiallkirjarakendused"
head_description: "Hankige kõik-ühes dokumendi e-allkirja lahendus .NET-i, Java- ja pilvepõhiste rakenduste jaoks. Allkirjastage levinud dokumendivormingud veebis, kasutades lihtsat pukseerimisfunktsiooni"

############################# Header ############################
title: "Allkirjastada dokumendid<br>Node.js API-ga"
description: "Allkirjastage digitaalseid dokumente ja pilte mis tahes platvormil, kasutades meie paindlikke API-sid ja rakendusepõhiseid lahendusi programmeerijatele ja lõppkasutajatele."
words:
  for: "jaoks"

actions:
  main: "Laadige alla NPM-ist"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Litsentsi andmine"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Kas olete valmis alustama?"
  description: "Proovige GroupDocs.Signature'i funktsioone tasuta või taotlege litsentsi"

release:
  title: "Välja antud versioon {0}"
  notes: "Vaadake, mis on uut"
  downloads: "Allalaadimised"

code:
  title: "PDF-ide allkirjastamine Node.js-iga"
  more: "Veel näiteid"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```javascript {style=abap}   
    // Valige PDF-dokument
    let signature = new Signature("sample.pdf");
    
    // Esitage tekst
    let options = new TextSignOptions("John Smith");
    
    // Määra värv
    options.ForeColor = Color.Red;
    
    // Allkirjastage dokument ja salvestage faili
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Allkirja ülevaade"
  description: "Dokumentide allkirjastamise teek, mis on Node.js rakendustes kasutamiseks valmis"
  features:
    # feature loop
    - title: "Digiallkirjade lahendus äridokumentidele koos Node.js-iga"
      content: "GroupDocs.Signature for Node.js via Java pakub PDF-i, Office'i dokumentide ja piltide jaoks laiaulatuslikku digitaalallkirja valikute komplekti. Saadaval on tekst, vöötkoodid, pildid, digitaalsed sertifikaadid ja metaandmed. Sujuv dokumenditöötlus tagab tõhususe."

    # feature loop
    - title: "Allkirjastatud dokumentide täiustatud manipuleerimine"
      content: "GroupDocs.Signature annab teile õiguse allkirjastatud dokumente töödelda. Otsige ja kinnitage allkirju erinevate kriteeriumide abil. Lisaks saate eraldada üksikasjalikku dokumenditeavet või luua lehtede eelvaatepilte."

    # feature loop
    - title: "Erinevad väljundvormingud"
      content: "Meie lahendus pakub ulatuslikku kontrolli allkirjastatud dokumentide väljundvormingu üle. Positsioneerige täpselt allkirjad mis tahes lehel ja kohandage nende välimust. Salvestage allkirjastatud dokumente paljudes toetatud vormingutes ja kaitske neid valikuliselt paroolidega."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platvormi sõltumatus"
  description: "GroupDocs.Signature for Node.js via Java töötleb dokumente erinevate operatsioonisüsteemidega"
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
  title: "Toetatud failivormingud"
  description: |
    GroupDocs.Signature for Node.js via Java hõlbustab [populaarsete failivormingute](https://docs.groupdocs.com/signature/java/supported-document-formats/) toiminguid.
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office'i vormingud
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Pildid ja muud vormingud
        * **Kaasaskantav:** PDF
        * **Pildid:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Muud kontorivormingud:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Muud vormingud
        * **võrk:** HTML, MHTML
        * **Arhiivid:** ZIP, TAR, 7Z
        * **Sertifikaadid:** PFX

############################# Features ############################
features:
  enable: true
  title: "Toote GroupDocs.Signature funktsioonid"
  description: "Allkirjastage PDF-faile, Office'i dokumente ja pilte digitaalallkirjadega"

  items:
    # feature loop
    - icon: "sign"
      title: "Äriallkirjad"
      content: "Kasutage dokumentide allkirjastamiseks erinevaid allkirjatüüpe. Asetage digitaalallkirjad täpselt mis tahes lehe asukohta."

    # feature loop
    - icon: "custom"
      title: "Allkirja välimuse kohandamine"
      content: "Kohandage allkirjade visuaalseid aspekte, kohandades soovitud tulemuse saavutamiseks värvi, fonti, ääriseid, pööramist ja muud."

    # feature loop
    - icon: "password"
      title: "Parooliga kaitstud dokumendid"
      content: "Paljude toetatud dokumendivormingute puhul kaitske allkirjastatud dokumente turvalisuse suurendamiseks parooliga."

    # feature loop
    - icon: "protect"
      title: "Volitamata muudatuste vältimine"
      content: "Kaitske olulisi digisertifikaatidega allkirjastatud äridokumente volitamata muutmise eest."

    # feature loop
    - icon: "convert"
      title: "Soovitud väljundvormingud"
      content: "Hankige hõlpsasti allkirjastatud dokumente mis tahes toetatud vormingus. Teisendage MS Wordi dokumendid hõlpsalt PDF-vormingusse."

    # feature loop
    - icon: "preview"
      title: "Dokumentide eelvaade"
      content: "Salvestage üksikud dokumendilehed piltidena tulevaste vajaduste jaoks."

    # feature loop
    - icon: "search"
      title: "Allkirja otsing"
      content: "Saate hankida teavet oma dokumentides varem lisatud allkirjade kohta."

    # feature loop
    - icon: "validate"
      title: "Dokumendi kinnitamine"
      content: "Kontrollige mis tahes dokumendis esitatud allkirjade autentsust."

    # feature loop
    - icon: "update"
      title: "Allkirjahaldus"
      content: "Kustutage, paigutage ümber või muutke mis tahes dokumendi lehele pandud allkirju."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Koodi näidised"
  description: "Illustreerivad näited, mis näitavad tüüpilisi GroupDocs.Signature for Node.js via Java toiminguid"
  items:
    # code sample loop
    - title: "Märkige PDF QR-koodidega"
      content: |
        [Vöötkoodide](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) lisamine konkreetsetele PDF-dokumendi lehtedele võib äriprotsesse sujuvamaks muuta. Selles jaotises on näide QR-koodi lisamisest, kasutades GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Kuidas panna QR-kood PDF-i.">}}
        ```javascript {style=abap}
        // Laadige alla allkirjastatav dokument
        let signature = new Signature("file_to_sign.pdf");
        
        // Looge QR-koodi valikud eelnevalt määratletud tekstiga
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigureerige QR-koodi kodeeringu tüüp ja asukoht lehel
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Allkirjastage dokument ja salvestage see tulemusfailina
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX-i kaitsmine digitaalallkirjaga"
      content: |
        [Kaitske oma dokumente](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) digitaalsetel sertifikaatidel põhinevate allkirjadega. Digiallkiri kaitseb teie äridokumente sisu muutumise eest.
        {{< landing/code title="Siin on, kuidas tagada dokumendi terviklikkus.">}}
        ```javascript {style=abap}   
        // Laadige digitaalselt allkirjastatav dokument
        let signature = new Signature("file_to_sign.pdf");
        
        // Määrake digitaalse allkirjastamise suvandid ja määrake sertifikaadi faili tee
        let options = new DigitalSignOptions("certificate.pfx");

        // Määrake sertifikaadi parool
        options.Password = "1234567890";

        // Allkirjastage dokument ja salvestage see soovitud teele
        signature.Sign("digitally_signed.pdf", options);

        ```
        {{< /landing/code >}}

---
