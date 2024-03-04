---
############################# Static ############################
layout: "landing"
date: 2024-03-04T17:52:03
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: fi
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
head_title: ".NET, Java, pilvisovellusliittymät ja online-asiakirjojen allekirjoitussovellukset"
head_description: "Hanki all-in-one asiakirjan sähköinen allekirjoitusratkaisu .NET-, Java- ja pilvipohjaisille sovelluksille. Allekirjoita yleisiä asiakirjamuotoja verkossa yksinkertaisella vedä ja pudota -ominaisuuden avulla"

############################# Header ############################
title: "Allekirjoita asiakirjat<br>Node.js API:lla"
description: "Allekirjoita digitaalisia asiakirjoja ja kuvia millä tahansa alustalla käyttämällä ohjelmoijille ja loppukäyttäjille joustavia API- ja sovelluspohjaisia ​​ratkaisujamme."
words:
  for: "varten"

actions:
  main: "Lataa NPM:stä"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Lisensointi"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Oletko valmis aloittamaan?"
  description: "Kokeile GroupDocs.Signature-ominaisuuksia ilmaiseksi tai pyydä lisenssi"

release:
  title: "Versio {0} julkaistu"
  notes: "Katso mitä uutta"
  downloads: "Lataukset"

code:
  title: "PDF-tiedostojen allekirjoittaminen Node.js:n avulla"
  more: "Lisää esimerkkejä"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```javascript {style=abap}   
    // Valitse PDF-dokumentti
    let signature = new Signature("sample.pdf");
    
    // Anna tekstiä
    let options = new TextSignOptions("John Smith");
    
    // Aseta väri
    options.ForeColor = Color.Red;
    
    // Allekirjoita asiakirja ja tallenna tiedostoon
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Yleiskatsaus"
  description: "Asiakirjojen allekirjoituskirjasto, joka on valmis käytettäväksi Node.js-sovelluksissa"
  features:
    # feature loop
    - title: "Digitaalisten allekirjoitusten ratkaisu yritysasiakirjoille Node.js:n avulla"
      content: "GroupDocs.Signature for Node.js via Java tarjoaa kattavan joukon digitaalisia allekirjoitusvaihtoehtoja PDF-, Office-asiakirjoille ja kuville. Saatavilla on tekstiä, viivakoodeja, kuvia, digitaalisia varmenteita ja metatietoja. Virtaviivainen asiakirjojen käsittely varmistaa tehokkuuden."

    # feature loop
    - title: "Allekirjoitettujen asiakirjojen edistynyt käsittely"
      content: "GroupDocs.Signature antaa sinulle mahdollisuuden käsitellä allekirjoitettuja asiakirjoja. Etsi ja vahvista allekirjoitukset useilla eri kriteereillä. Lisäksi voit poimia yksityiskohtaisia ​​asiakirjatietoja tai luoda esikatselukuvia sivuista."

    # feature loop
    - title: "Monipuoliset tulostusmuodot"
      content: "Ratkaisumme tarjoaa laajan hallinnan allekirjoitettujen asiakirjojen tulostusmuodolle. Sijoita allekirjoitukset tarkasti mille tahansa sivulle ja muokkaa niiden ulkoasua. Tallenna allekirjoitetut asiakirjat useissa tuetuissa muodoissa ja valinnaisesti suojaa ne salasanoilla."

############################# Platforms ############################
platforms:
  enable: true
  title: "Alustan riippumattomuus"
  description: "GroupDocs.Signature for Node.js via Java käsittelee asiakirjoja eri käyttöjärjestelmissä"
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
  title: "Tuetut tiedostomuodot"
  description: |
    GroupDocs.Signature for Node.js via Java helpottaa [suosittujen tiedostomuotojen](https://docs.groupdocs.com/signature/java/supported-document-formats/) toimintoja.
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office -muodot
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Kuvat ja muut muodot
        * **Kannettava:** PDF
        * **Kuvat:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Muut toimistomuodot:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Muut muodot
        * **Web:** HTML, MHTML
        * **Arkistot:** ZIP, TAR, 7Z
        * **Sertifikaatit:** PFX

############################# Features ############################
features:
  enable: true
  title: "Tuotteen GroupDocs.Signature ominaisuudet"
  description: "Allekirjoita PDF-tiedostot, Office-asiakirjat ja kuvat digitaalisilla allekirjoituksilla"

  items:
    # feature loop
    - icon: "sign"
      title: "Liiketoiminnan allekirjoitukset"
      content: "Käytä erilaisia ​​allekirjoitustyyppejä asiakirjojen allekirjoittamiseen. Aseta digitaaliset allekirjoitukset tarkasti mihin tahansa sivun paikkaan."

    # feature loop
    - icon: "custom"
      title: "Allekirjoituksen ulkoasun mukauttaminen"
      content: "Räätälöi allekirjoitusten visuaalisia näkökohtia säätämällä väriä, fonttia, reunoja, kiertoa ja muuta halutun tuloksen saavuttamiseksi."

    # feature loop
    - icon: "password"
      title: "Salasanalla suojatut asiakirjat"
      content: "Suojaa allekirjoitetut asiakirjat salasanalla monissa tuetuissa asiakirjamuodoissa turvallisuuden lisäämiseksi."

    # feature loop
    - icon: "protect"
      title: "Luvattomien muutosten estäminen"
      content: "Suojaa tärkeät digitaalisilla varmenteilla allekirjoitetut liikeasiakirjat luvattomilta muutoksilta."

    # feature loop
    - icon: "convert"
      title: "Halutut tulostusmuodot"
      content: "Hanki vaivattomasti allekirjoitetut asiakirjat missä tahansa tuetussa muodossa. Muunna MS Word -asiakirjat PDF-muotoon helposti."

    # feature loop
    - icon: "preview"
      title: "Asiakirjojen esikatselu"
      content: "Tallenna yksittäiset asiakirjasivut kuvina tulevia tarpeita varten."

    # feature loop
    - icon: "search"
      title: "Allekirjoitushaku"
      content: "Hae tietoja asiakirjoihin aiemmin lisätyistä allekirjoituksista."

    # feature loop
    - icon: "validate"
      title: "Asiakirjan validointi"
      content: "Tarkista missä tahansa asiakirjassa esitettyjen allekirjoitusten aitous."

    # feature loop
    - icon: "update"
      title: "Allekirjoituksen hallinta"
      content: "Poista, siirrä tai muokkaa mille tahansa asiakirjan sivulle asetettuja allekirjoituksia."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Koodinäytteet"
  description: "Havainnollistavia esimerkkejä, jotka esittelevät tyypillisiä GroupDocs.Signature for Node.js via Java-toimintoja"
  items:
    # code sample loop
    - title: "Merkitse PDF QR-koodeilla"
      content: |
        [Viivakoodien](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) sisällyttäminen tietyille PDF-dokumenttisivuille voi virtaviivaistaa liiketoimintaprosesseja. Tässä osiossa on esimerkki QR-koodin lisäämisestä käyttämällä GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Kuinka laittaa QR-koodi PDF-tiedostoon.">}}
        ```javascript {style=abap}
        // Lataa allekirjoitettava asiakirja
        let signature = new Signature("file_to_sign.pdf");
        
        // Luo QR-koodivaihtoehtoja ennalta määritetyllä tekstillä
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Määritä QR-koodin koodaustyyppi ja sijainti sivulla
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Allekirjoita asiakirja ja tallenna se tulostiedostona
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX:n suojaaminen digitaalisella allekirjoituksella"
      content: |
        [Suojaa asiakirjojasi](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) digitaalisiin varmenteisiin perustuvilla allekirjoituksilla. Digitaalinen allekirjoitus suojaa yrityksesi asiakirjoja sisällön muuttumiselta.
        {{< landing/code title="Näin varmistat asiakirjan eheyden.">}}
        ```javascript {style=abap}   
        // Lataa asiakirja digitaalisesti allekirjoitettavaa varten
        let signature = new Signature("file_to_sign.pdf");
        
        // Määritä digitaalisen allekirjoituksen asetukset ja anna polku varmennetiedostoon
        let options = new DigitalSignOptions("certificate.pfx");

        // Aseta varmenteen salasana
        options.Password = "1234567890";

        // Allekirjoita asiakirja ja tallenna se haluamaasi polkuun
        signature.Sign("digitally_signed.pdf", options);

        ```
        {{< /landing/code >}}

---
