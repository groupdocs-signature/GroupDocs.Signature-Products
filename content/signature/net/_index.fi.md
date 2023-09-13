---
############################# Static ############################
layout: "landing"
date: 2023-09-13T10:36:51
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: fi
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, pilvisovellusliittymät ja online-asiakirjojen allekirjoitussovellukset"
head_description: "Hanki all-in-one asiakirjan sähköinen allekirjoitusratkaisu .NET-, Java- ja pilvipohjaisille sovelluksille. Allekirjoita yleisiä asiakirjamuotoja verkossa yksinkertaisella vedä ja pudota -ominaisuuden avulla"

############################# Header ############################
title: "Allekirjoita asiakirjat<br>.NET API:n kautta"
description: "Allekirjoita digitaalisia asiakirjoja ja kuvia millä tahansa alustalla käyttämällä ohjelmoijille ja loppukäyttäjille joustavia API- ja sovelluspohjaisia ​​ratkaisujamme."
words:
  for: "varten"

actions:
  main: "Ilmainen NuGet-lataus"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Lisensointi"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Oletko valmis aloittamaan?"
  description: "Kokeile GroupDocs.Signature-ominaisuuksia ilmaiseksi tai pyydä lisenssi"

release:
  title: "Versio {0} julkaistu"
  notes: "Katso mitä uutta"
  downloads: "Lataukset"

code:
  title: "Allekirjoita PDF-tiedostot C#:lla"
  more: "Lisää esimerkkejä"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Valitse PDF-dokumentti
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Anna tekstiä
        var options = new TextSignOptions("John Smith")
        {
            // Aseta väri
            ForeColor = Color.Red
        };
        // Allekirjoita asiakirja ja tallenna tiedostoon
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Yleiskatsaus"
  description: "API asiakirjan allekirjoittamiseen ja niihin liittyvien toimintojen suorittamiseen .NET-sovelluksissa"
  features:
    # feature loop
    - title: "Allekirjoitusten lisääminen yritysasiakirjoihin C#:ssa"
      content: "Asiakirjojen allekirjoittaminen: GroupDocs.Signature for .NET -sovelluksella voit lisätä PDF- ja Office-asiakirjoihin erilaisia ​​allekirjoituksia, kuten tekstiä, kuvia, viivakoodeja ja digitaalisia varmenteita. Tämän API:n avulla voit allekirjoittaa asiakirjasi lähes kaikilla tietotyypeillä, mukaan lukien piilotetut metatiedot."

    # feature loop
    - title: "Allekirjoitettujen asiakirjojen käsittely"
      content: "Lisäkäsittely: Voit suorittaa tehokkaita toimintoja allekirjoitetuille asiakirjoille GroupDocs.Signaturen avulla. Tämä sisältää olemassa olevien allekirjoitusten etsimisen yritysasiakirjoista ja niiden tarkistamisen tietyillä kriteereillä. Lisäksi voit hakea asiakirjan tietoja ja esikatsella sivuja tämän .NET API:n kautta."

    # feature loop
    - title: "Tulosten mukauttaminen"
      content: "GroupDocs.Signature for .NET tarjoaa laajat mukautusvaihtoehdot. Voit sijoittaa allekirjoitukset tarkasti mihin tahansa asiakirjan sivulle ja säätää niiden ulkoasua useiden asetusten avulla. Lisäksi tämä API tukee käsiteltyjen asiakirjojen tallentamista useissa tuetuissa muodoissa."

############################# Platforms ############################
platforms:
  enable: true
  title: "Alustan riippumattomuus"
  description: "GroupDocs.Signature for .NET tukee seuraavia käyttöjärjestelmiä, kehyksiä ja paketinhallintaohjelmia"
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
    GroupDocs.Signature for .NET tukee toimintoja seuraavilla [tiedostomuodoilla](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  title: "GroupDocs.Signature-ominaisuudet"
  description: "PDF-tiedostojen, Office-asiakirjojen ja kuvien allekirjoittaminen nopeasti ja tarkasti"

  items:
    # feature loop
    - icon: "merge"
      title: "Asiakirjan allekirjoittaminen"
      content: "Lisää yksi tai useita tuettuja allekirjoitustyyppejä tarkasti mihin tahansa määritettyyn paikkaan yritysasiakirjoissa."

    # feature loop
    - icon: "split"
      title: "Muokkaa allekirjoituksia"
      content: "Käytä ominaisuuksia, kuten väriä, fonttia, reunusta, kiertoa jne., määrittääksesi allekirjoitusten ulkoasun."

    # feature loop
    - icon: "move"
      title: "Asiakirjan salasanasuojaus"
      content: "Suojaa tietyt asiakirjatyypit asettamalla salasana allekirjoituksen jälkeen."

    # feature loop
    - icon: "remove"
      title: "Suojaus muutoksilta"
      content: "Estä tärkeiden yritysasiakirjojen muutokset liittämällä allekirjoituksen digitaalisella varmenteella."

    # feature loop
    - icon: "rotate"
      title: "Muunna allekirjoitetut tiedostot muihin muotoihin"
      content: "Muunna allekirjoitetut tiedostot haluttuihin muotoihin, kuten tallenna Word-asiakirja PDF-muodossa."

    # feature loop
    - icon: "swap"
      title: "Pura sivujen esikatselut"
      content: "Poimi sivut allekirjoitetuista asiakirjoista yksittäisinä kuvina tulevaa käsittelyä varten."

    # feature loop
    - icon: "extract"
      title: "Allekirjoitushaku asiakirjoista"
      content: "Hae tiedot aiemmin lisätyistä allekirjoituksista tiettyihin asiakirjoihin."

    # feature loop
    - icon: "orientation"
      title: "Vahvista allekirjoitetut asiakirjat"
      content: "Tarkista asiakirjojen oikea allekirjoitus vahvistusominaisuuksien avulla."

    # feature loop
    - icon: "preview"
      title: "Päivitä tai poista allekirjoituksia"
      content: "Voit helposti sijoittaa tietyt allekirjoitukset sivulle, muokata niiden tekstiä tai poistaa ne ilman ongelmia."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Koodinäytteet"
  description: "Jotkut käyttävät tyypillisiä GroupDocs.Signature-tapauksia .NET-toimintoihin"
  items:
    # code sample loop
    - title: "Lisää QR-koodi PDF-tiedostoon"
      content: |
        [QR-koodien] (https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) lisääminen PDF-dokumenttien tietyille sivuille voi parantaa liiketoimintaprosesseja. Alla on esimerkki QR-koodin lisäämisestä GroupDocs.Signaturen avulla.
        {{< landing/code title="Kuinka laittaa QR-koodi PDF-tiedostoon.">}}
        ```csharp {style=abap}
        // Lataa allekirjoitettava asiakirja
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Luo QR-koodivaihtoehtoja ennalta määritetyllä tekstillä
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Määritä QR-koodin koodaustyyppi ja sijainti sivulla
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Allekirjoita asiakirja ja tallenna se tulostiedostona
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX-asiakirjan suojaaminen digitaalisella varmenteella"
      content: |
        Voit [Protect a Document](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) käyttämällä digitaalisina varmenteina tallennettuja henkilökohtaisia ​​tai yrityksen allekirjoituksia. Tällaisia ​​suojattuja asiakirjoja ei voida muuttaa ilman allekirjoituksen mitätöintiä.
        {{< landing/code title="Näin varmistat asiakirjan eheyden.">}}
        ```csharp {style=abap}   
        // Lataa asiakirja digitaalisesti allekirjoitettavaa varten
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Määritä digitaalisen allekirjoituksen asetukset ja anna polku varmennetiedostoon
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Aseta varmenteen salasana
                Password = "1234567890"
            };
            // Allekirjoita asiakirja ja tallenna se haluamaasi polkuun
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
