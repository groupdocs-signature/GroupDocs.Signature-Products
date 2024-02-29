---
############################# Static ############################
layout: "landing"
date: 2024-02-29T14:43:07
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
head_title: ".NET, Java, pilve API-d ja veebipõhised dokumendiallkirjarakendused"
head_description: "Hankige kõik-ühes dokumendi e-allkirja lahendus .NET-i, Java- ja pilvepõhiste rakenduste jaoks. Allkirjastage levinud dokumendivormingud veebis, kasutades lihtsat pukseerimisfunktsiooni"

############################# Header ############################
title: "Allkirjastada dokumendid<br>.NET API kaudu"
description: "Allkirjastage digitaalseid dokumente ja pilte mis tahes platvormil, kasutades meie paindlikke API-sid ja rakendusepõhiseid lahendusi programmeerijatele ja lõppkasutajatele."
words:
  for: "jaoks"

actions:
  main: "Tasuta NuGeti allalaadimine"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Litsentsi andmine"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Kas olete valmis alustama?"
  description: "Proovige GroupDocs.Signature'i funktsioone tasuta või taotlege litsentsi"

release:
  title: "Välja antud versioon {0}"
  notes: "Vaadake, mis on uut"
  downloads: "Allalaadimised"

code:
  title: "PDF-failide allkirjastamine C#-s"
  more: "Veel näiteid"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Valige PDF-dokument
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Esitage tekst
        var options = new TextSignOptions("John Smith")
        {
            // Määra värv
            ForeColor = Color.Red
        };
        // Allkirjastage dokument ja salvestage faili
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Allkirja ülevaade"
  description: "API dokumentide allkirjastamiseks ja sellega seotud toimingute tegemiseks .NET-i rakendustes"
  features:
    # feature loop
    - title: "Allkirjade lisamine äridokumentidele C#-s"
      content: "Dokumentide allkirjastamine: GroupDocs.Signature for .NET abil saate PDF- ja Office'i dokumentidele lisada erinevat tüüpi allkirju, näiteks teksti, pilte, vöötkoode ja digitaalseid sertifikaate. See API võimaldab teil oma dokumente allkirjastada peaaegu iga andmetüübiga, sealhulgas peidetud metaandmetega."

    # feature loop
    - title: "Allkirjastatud dokumentide töötlemine"
      content: "Täiendav töötlemine: saate teha võimsaid toiminguid allkirjastatud dokumentidega, kasutades GroupDocs.Signature'i. See hõlmab olemasolevate allkirjade otsimist äridokumentides ja nende kontrollimist konkreetsete kriteeriumide alusel. Lisaks saate selle .NET API kaudu hankida dokumenditeavet ja vaadata lehti."

    # feature loop
    - title: "Tulemuste kohandamine"
      content: "GroupDocs.Signature for .NET pakub ulatuslikke kohandamisvõimalusi. Saate täpselt paigutada allkirjad kõikjal dokumendilehel ja kohandada nende välimust, kasutades erinevaid seadeid. Lisaks toetab see API töödeldud dokumentide salvestamist paljudes toetatud vormingutes."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platvormi sõltumatus"
  description: "GroupDocs.Signature for .NET toetab järgmisi operatsioonisüsteeme, raamistikke ja paketihaldureid"
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
    GroupDocs.Signature for .NET toetab toiminguid järgmiste [failivormingutega](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  description: "PDF-ide, Office'i dokumentide ja piltide kiire ja täpne allkirjastamine"

  items:
    # feature loop
    - icon: "sign"
      title: "Dokumendi allkirjastamine"
      content: "Lisage täpselt üks või mitu toetatud allkirjatüüpi äridokumentide mis tahes määratud kohta."

    # feature loop
    - icon: "custom"
      title: "Kohandage allkirju"
      content: "Kasutage allkirjade välimuse konfigureerimiseks selliseid funktsioone nagu värv, font, ääris, pööramine jne."

    # feature loop
    - icon: "password"
      title: "Dokumentide paroolikaitse"
      content: "Kaitske teatud tüüpi dokumendid, määrates pärast allkirjastamist parooli."

    # feature loop
    - icon: "protect"
      title: "Kaitse muutuste eest"
      content: "Vältige oluliste äridokumentide muutmist pärast digitaalse sertifikaadiga allkirja lisamist."

    # feature loop
    - icon: "convert"
      title: "Teisendage allkirjastatud failid muudesse vormingutesse"
      content: "Teisendage allkirjastatud failid soovitud vormingusse, näiteks salvestage Wordi dokument PDF-vormingus."

    # feature loop
    - icon: "preview"
      title: "Ekstraktige lehe eelvaated"
      content: "Eraldage allkirjastatud dokumentidest lehed üksikute piltidena edaspidiseks töötlemiseks."

    # feature loop
    - icon: "search"
      title: "Allkirjaotsing dokumentides"
      content: "Hankige teavet konkreetsetes dokumentides varem lisatud allkirjade kohta."

    # feature loop
    - icon: "validate"
      title: "Kinnitage allkirjastatud dokumendid"
      content: "Kontrollige dokumentide õiget allkirjastamist valideerimisfunktsioonide abil."

    # feature loop
    - icon: "update"
      title: "Allkirjade värskendamine või kustutamine"
      content: "Saate hõlpsalt lehel konkreetseid allkirju ümber paigutada, nende teksti muuta või kustutada ilma probleemideta."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Koodi näidised"
  description: "Mõned tüüpilised GroupDocs.Signature'i kasutamise juhtumid .NET-i toimingute jaoks"
  items:
    # code sample loop
    - title: "Lisage PDF-i QR-kood"
      content: |
        [QR-koodide](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) lisamine PDF-dokumentide konkreetsetele lehtedele võib äriprotsesse täiustada. Allpool on näide QR-koodi lisamisest GroupDocs.Signature abil.
        {{< landing/code title="Kuidas panna QR-kood PDF-i.">}}
        ```csharp {style=abap}
        // Laadige alla allkirjastatav dokument
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Looge QR-koodi valikud eelnevalt määratletud tekstiga
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Konfigureerige QR-koodi kodeeringu tüüp ja asukoht lehel
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Allkirjastage dokument ja salvestage see tulemusfailina
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX-dokumendi kaitsmine digitaalse sertifikaadi abil"
      content: |
        Saate [dokumenti kaitsta](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/), kasutades digitaalsete sertifikaatidena salvestatud isiklikke või ettevõtte allkirju. Selliseid kaitstud dokumente ei saa muuta ilma allkirja kehtetuks tunnistamata.
        {{< landing/code title="Siin on, kuidas tagada dokumendi terviklikkus.">}}
        ```csharp {style=abap}   
        // Laadige digitaalselt allkirjastatav dokument
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Määrake digitaalse allkirjastamise suvandid ja määrake sertifikaadi faili tee
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Määrake sertifikaadi parool
                Password = "1234567890"
            };
            // Allkirjastage dokument ja salvestage see soovitud teele
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
