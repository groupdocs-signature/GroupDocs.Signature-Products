---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:21
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
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, pilvisovellusliittymät ja online-asiakirjojen allekirjoitussovellukset"
head_description: "Hanki all-in-one asiakirjan sähköinen allekirjoitusratkaisu .NET-, Java- ja pilvipohjaisille sovelluksille. Allekirjoita yleisiä asiakirjamuotoja verkossa yksinkertaisella vedä ja pudota -ominaisuuden avulla"

############################# Header ############################
title: "Allekirjoita asiakirjat<br>Java API:n kautta"
description: "Allekirjoita digitaalisia asiakirjoja ja kuvia millä tahansa alustalla käyttämällä ohjelmoijille ja loppukäyttäjille joustavia API- ja sovelluspohjaisia ​​ratkaisujamme."
words:
  for: "varten"

actions:
  main: "Ilmainen Maven lataus"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Lisensointi"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Oletko valmis aloittamaan?"
  description: "Kokeile GroupDocs.Signature-ominaisuuksia ilmaiseksi tai pyydä lisenssi"

release:
  title: "Versio {0} julkaistu"
  notes: "Katso mitä uutta"
  downloads: "Lataukset"

code:
  title: "Allekirjoita PDF-tiedostoja Javalla"
  more: "Lisää esimerkkejä"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Valitse PDF-dokumentti
    Signature signature = new Signature("sample.pdf");
    
    // Anna tekstiä
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Allekirjoita asiakirja ja tallenna tiedostoon
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Yleiskatsaus"
  description: "API dokumenttien allekirjoittamiseen ja siihen liittyvien toimintojen suorittamiseen Java-sovelluksissa"
  features:
    # feature loop
    - title: "Parannetut yritysasiakirjat digitaalisilla allekirjoituksilla Javassa"
      content: "Nopea ja muokattavissa oleva allekirjoitus: GroupDocs.Signature for Java tarjoaa laajan valikoiman digitaalisia allekirjoitusvaihtoehtoja PDF-tiedostoille, kuville ja Office-asiakirjoille. Voit käyttää tekstiä, viivakoodeja, QR-koodeja, digitaalisia varmenteita, kuvia tai piilotettuja metatietoja. Asiakirjojen käsittely on nopeaa ja tehokasta."

    # feature loop
    - title: "Allekirjoitettujen asiakirjojen käsittely"
      content: "Edistyksellinen asiakirjojen käsittely sisältää tehokkaita toimintoja allekirjoitetuille asiakirjoille käyttäen GroupDocs.Signature for Javaa. Voit etsiä ja vahvistaa yritysasiakirjoihin lisättyjä allekirjoituksia useilla hyödyllisillä kriteereillä. Lisäksi voit tarkastella asiakirjan yksityiskohtaisia ​​tietoja tai saada esikatselukuvia sen sivuista."

    # feature loop
    - title: "Erilaisia ​​lähtövaihtoehtoja"
      content: "Vahvat allekirjoitusasetukset mahdollistavat GroupDocs.Signature for Java -sovelluksella allekirjoitettujen asiakirjojen tulosteen mukauttamisen. Voit sijoittaa minkä tahansa allekirjoituksen tarkasti mille tahansa asiakirjasivulle ja määrittää sen ulkoasun eri tavoin. Java API tukee allekirjoitettujen yritysasiakirjojen tallentamista useissa tuetuissa muodoissa ja tarjoaa vaihtoehtoja niiden suojaamiseen salasanoilla."

############################# Platforms ############################
platforms:
  enable: true
  title: "Alustan riippumattomuus"
  description: "GroupDocs.Signature for Java tukee seuraavia käyttöjärjestelmiä, kehyksiä ja paketinhallintaohjelmia"
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Tuetut tiedostomuodot"
  description: |
    GroupDocs.Signature for Java tukee toimintoja seuraavilla [tiedostomuodoilla](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  description: "PDF-tiedostojen, Office-asiakirjojen ja kuvien allekirjoittaminen digitaalisilla allekirjoituksilla"

  items:
    # feature loop
    - icon: "sign"
      title: "Allekirjoitusten lisääminen"
      content: "Allekirjoita asiakirja käyttämällä erilaisia ​​tuettuja allekirjoitustyyppejä asettamalla digitaalinen allekirjoitus tarkasti mihin tahansa kohtaan millä tahansa sivulla."

    # feature loop
    - icon: "custom"
      title: "Tulosten mukauttaminen"
      content: "Mukauta allekirjoituksen ulkoasua säätämällä väriä, fonttia, reunusta, kiertoa ja muita ominaisuuksia halutun tuloksen saavuttamiseksi."

    # feature loop
    - icon: "password"
      title: "Asiakirjojen suojaaminen salasanalla"
      content: "Monissa tuetuissa asiakirjatyypeissä voit suojata allekirjoitetun asiakirjan salasanalla."

    # feature loop
    - icon: "protect"
      title: "Estä luvattomat muutokset"
      content: "Suojaa tärkeät digitaalisella varmenteella allekirjoitetut liikeasiakirjat luvattomilta muutoksilta."

    # feature loop
    - icon: "convert"
      title: "Tulosten saaminen halutussa muodossa"
      content: "Hanki allekirjoitetut tulostiedostot helposti missä tahansa tuetussa muodossa. Voit myös muuntaa MS Word -asiakirjoja PDF-muotoon vaivattomasti."

    # feature loop
    - icon: "preview"
      title: "Asiakirjan esikatselu"
      content: "Tallenna mikä tahansa asiakirjan sivu kuvana myöhempää käsittelyä varten."

    # feature loop
    - icon: "search"
      title: "Allekirjoituksia etsimässä"
      content: "Tiettyihin asiakirjoihin on mahdollista saada tietoa aiemmin lisätyistä allekirjoituksista."

    # feature loop
    - icon: "validate"
      title: "Asiakirjojen vahvistaminen"
      content: "Tarkista minkä tahansa allekirjoitetun asiakirjan allekirjoitusten oikeellisuus."

    # feature loop
    - icon: "update"
      title: "Allekirjoitusten hallinta"
      content: "Kun allekirjoitus on asetettu asiakirjan sivulle, se voidaan poistaa, siirtää tai päivittää tarpeen mukaan."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Koodinäytteet"
  description: "Jotkut käyttävät tyypillisiä GroupDocs.Signature-tapauksia Java-operaatioille"
  items:
    # code sample loop
    - title: "Paranna PDF-dokumenttia QR-koodilla"
      content: |
        Liiketoimintaprosessien parantaminen lisäämällä [QR-koodeja](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) PDF-dokumenttien tietyille sivuille voi olla arvokasta. Tässä on esimerkki QR-koodin lisäämisestä GroupDocs.Signature for Java -sovelluksella.
        {{< landing/code title="Paranna PDF-dokumenttia QR-koodilla">}}
        ```java {style=abap}
        // Lataa allekirjoitettava asiakirja
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Luo QR-koodivaihtoehtoja ennalta määritetyllä tekstillä
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Määritä QR-koodin koodaustyyppi ja sijainti sivulla
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Allekirjoita asiakirja ja tallenna se tulostiedostona
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Suojaa DOCX käyttämällä digitaalista allekirjoitusta"
      content: |
        Voit [suojata asiakirjan](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) käyttämällä digitaalisina varmenteina tallennettuja henkilökohtaisia ​​tai yrityksen allekirjoituksia. Varmenteella suojattuja asiakirjoja ei voi muuttaa ilman allekirjoitusta mitätöimättä.
        {{< landing/code title="Suojaa DOCX käyttämällä digitaalista allekirjoitusta">}}
        ```java {style=abap}   
        // Lataa asiakirja digitaalisesti allekirjoitettavaa varten
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Määritä digitaalisen allekirjoituksen asetukset ja anna polku varmennetiedostoon
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Aseta varmenteen salasana
        options.setPassword("1234567890");

        // Allekirjoita asiakirja ja tallenna se haluamaasi polkuun
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
