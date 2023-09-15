---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:21
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: et
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, pilve API-d ja veebipõhised dokumendiallkirjarakendused"
head_description: "Hankige kõik-ühes dokumendi e-allkirja lahendus .NET-i, Java- ja pilvepõhiste rakenduste jaoks. Allkirjastage levinud dokumendivormingud veebis, kasutades lihtsat pukseerimisfunktsiooni"

############################# Header ############################
title: "Allkirjastada dokumendid<br>Java API kaudu"
description: "Allkirjastage digitaalseid dokumente ja pilte mis tahes platvormil, kasutades meie paindlikke API-sid ja rakendusepõhiseid lahendusi programmeerijatele ja lõppkasutajatele."
words:
  for: "jaoks"

actions:
  main: "Tasuta Maveni allalaadimine"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Litsentsi andmine"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Kas olete valmis alustama?"
  description: "Proovige GroupDocs.Signature'i funktsioone tasuta või taotlege litsentsi"

release:
  title: "Välja antud versioon {0}"
  notes: "Vaadake, mis on uut"
  downloads: "Allalaadimised"

code:
  title: "PDF-failide allkirjastamine Javas"
  more: "Veel näiteid"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Valige PDF-dokument
    Signature signature = new Signature("sample.pdf");
    
    // Esitage tekst
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Allkirjastage dokument ja salvestage faili
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Allkirja ülevaade"
  description: "API dokumentide allkirjastamiseks ja sellega seotud toimingute tegemiseks Java rakendustes"
  features:
    # feature loop
    - title: "Täiustatud äridokumendid Java digiallkirjadega"
      content: "Kiire ja kohandatav allkirjastamine: GroupDocs.Signature for Java pakub PDF-ide, piltide ja Office'i dokumentide jaoks laias valikus digitaalallkirjade valikuid. Saate kasutada teksti, vöötkoode, QR-koode, digitaalseid sertifikaate, pilte või peidetud metaandmeid. Dokumentide töötlemine on kiire ja tõhus."

    # feature loop
    - title: "Allkirjastatud dokumentidega manipuleerimine"
      content: "Täiustatud dokumenditöötlus hõlmab võimsaid toiminguid allkirjastatud dokumentidega, kasutades Java jaoks mõeldud GroupDocs.Signature'i. Saate otsida ja kinnitada äridokumentidele lisatud allkirju, kasutades erinevaid kasulikke kriteeriume. Lisaks pääsete juurde üksikasjalikule teabele dokumendi kohta või saate selle lehtede eelvaatepilte."

    # feature loop
    - title: "Erinevad väljundi valikud"
      content: "Tugevad allkirjastamisvalikud võimaldavad teil kohandada GroupDocs.Signature for Java-ga allkirjastatud dokumentide väljundit. Saate täpselt paigutada mis tahes allkirja mis tahes dokumendi lehele ja konfigureerida selle välimust mitmel viisil. Java API toetab allkirjastatud äridokumentide salvestamist paljudes toetatud vormingutes ja pakub võimalusi nende turvamiseks paroolidega."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platvormi sõltumatus"
  description: "GroupDocs.Signature for Java toetab järgmisi operatsioonisüsteeme, raamistikke ja paketihaldureid"
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
  title: "Toetatud failivormingud"
  description: |
    GroupDocs.Signature for Java toetab toiminguid järgmiste [failivormingutega](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "GroupDocs.Allkirja funktsioonid"
  description: "PDF-ide, Office'i dokumentide ja piltide allkirjastamine digitaalallkirjadega"

  items:
    # feature loop
    - icon: "sign"
      title: "Allkirjade lisamine"
      content: "Allkirjastage dokument, kasutades erinevaid toetatud allkirjatüüpe, asetades digitaalallkirja täpselt mis tahes lehe mis tahes kohta."

    # feature loop
    - icon: "custom"
      title: "Tulemuste kohandamine"
      content: "Kohandage allkirja välimust, kohandades soovitud tulemuse saavutamiseks värvi, fonti, äärist, pööramist ja muid funktsioone."

    # feature loop
    - icon: "password"
      title: "Dokumentide turvamine parooliga"
      content: "Paljude toetatud dokumenditüüpide puhul saate allkirjastatud dokumenti kaitsta parooliga."

    # feature loop
    - icon: "protect"
      title: "Volitamata muudatuste vältimine"
      content: "Kaitske digitaalse sertifikaadiga allkirjastatud olulisi äridokumente volitamata muutmise eest."

    # feature loop
    - icon: "convert"
      title: "Tulemuste saamine soovitud vormingus"
      content: "Hankige hõlpsasti allkirjastatud tulemusfailid mis tahes toetatud vormingus. Samuti saate MS Wordi dokumente hõlpsalt PDF-vormingusse teisendada."

    # feature loop
    - icon: "preview"
      title: "Dokumendi eelvaade"
      content: "Salvestage dokumendi mis tahes leht pildina edaspidiseks töötlemiseks."

    # feature loop
    - icon: "search"
      title: "Allkirjade otsimine"
      content: "Varem lisatud allkirjade kohta on võimalik saada infot konkreetsetes dokumentides."

    # feature loop
    - icon: "validate"
      title: "Dokumentide kinnitamine"
      content: "Kontrollige mis tahes allkirjastatud dokumendi allkirjade õigsust."

    # feature loop
    - icon: "update"
      title: "Allkirjade haldamine"
      content: "Kui allkiri on dokumendi lehele pandud, saab seda vastavalt vajadusele kustutada, teisaldada või värskendada."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Koodi näidised"
  description: "Mõned kasutavad tüüpilisi GroupDocs.Signature'i Java-operatsioonide jaoks"
  items:
    # code sample loop
    - title: "Täiustage PDF-dokumenti QR-koodiga"
      content: |
        Äriprotsesside täiustamine PDF-dokumentide konkreetsetele lehtedele [QR-koodide](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) lisamisega võib olla väärtuslik. Seal on näide QR-koodi lisamise kohta, kasutades GroupDocs.Signature for Java.
        {{< landing/code title="Täiustage PDF-dokumenti QR-koodiga">}}
        ```java {style=abap}
        // Laadige alla allkirjastatav dokument
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Looge QR-koodi valikud eelnevalt määratletud tekstiga
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigureerige QR-koodi kodeeringu tüüp ja asukoht lehel
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Allkirjastage dokument ja salvestage see tulemusfailina
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Kasutage DOCX-i kaitsmiseks digitaalallkirja"
      content: |
        Saate [dokumenti kaitsta](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/), kasutades digitaalsete sertifikaatidena salvestatud isiklikke või ettevõtte allkirju. Sertifikaadiga tagatud dokumente ei saa muuta ilma allkirja kehtetuks tunnistamata.
        {{< landing/code title="Kasutage DOCX-i kaitsmiseks digitaalallkirja">}}
        ```java {style=abap}   
        // Laadige digitaalselt allkirjastatav dokument
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Määrake digitaalse allkirjastamise suvandid ja määrake sertifikaadi faili tee
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Määrake sertifikaadi parool
        options.setPassword("1234567890");

        // Allkirjastage dokument ja salvestage see soovitud teele
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
