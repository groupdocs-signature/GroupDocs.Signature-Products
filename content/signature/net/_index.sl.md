---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: sl
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
head_title: ".NET, Java, API-ji v oblaku in aplikacije za spletno podpisovanje dokumentov"
head_description: "Pridobite vsestransko rešitev za e-podpisovanje dokumentov za .NET, Java in aplikacije v oblaku. Spletno podpišite običajne formate dokumentov s preprosto funkcijo povleci in spusti"

############################# Header ############################
title: "Podpišite dokumente<br>preko .NET API"
description: "Podpisujte digitalne dokumente in slike na kateri koli platformi z uporabo naših prilagodljivih API-jev in rešitev, ki temeljijo na aplikacijah, za programerje in končne uporabnike."
words:
  for: "za"

actions:
  main: "Brezplačen prenos NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licenciranje"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Ste pripravljeni začeti?"
  description: "Preizkusite funkcije GroupDocs.Signature brezplačno ali zahtevajte licenco"

release:
  title: "Izdana različica {0}"
  notes: "Oglejte si, kaj je novega"
  downloads: "Prenosi"

code:
  title: "Podpišite datoteke PDF v C#"
  more: "Več primerov"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Izberite dokument PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Navedite besedilo
        var options = new TextSignOptions("John Smith")
        {
            // Nastavite barvo
            ForeColor = Color.Red
        };
        // Podpišite dokument in ga shranite v datoteko
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Pregled"
  description: "API za izvajanje podpisovanja dokumentov in povezanih operacij v aplikacijah .NET"
  features:
    # feature loop
    - title: "Dodajanje podpisov poslovnim dokumentom v C#"
      content: "Podpisovanje dokumentov: Z GroupDocs.Signature za .NET lahko dokumentom PDF in Office dodate različne vrste podpisov, kot so besedilo, slike, črtne kode in digitalna potrdila. Ta API vam omogoča podpisovanje dokumentov s skoraj vsemi vrstami podatkov, vključno s skritimi metapodatki."

    # feature loop
    - title: "Obdelava podpisanih dokumentov"
      content: "Dodatna obdelava: z GroupDocs.Signature lahko izvajate zmogljive operacije na podpisanih dokumentih. To vključuje iskanje obstoječih podpisov v poslovnih dokumentih in njihovo preverjanje z uporabo posebnih kriterijev. Poleg tega lahko prek tega API-ja .NET pridobite informacije o dokumentu in predogledate strani."

    # feature loop
    - title: "Prilagajanje rezultatov"
      content: "GroupDocs.Signature za .NET ponuja obsežne možnosti prilagajanja. Podpise lahko natančno postavite kamor koli na strani dokumenta in prilagodite njihov videz z različnimi nastavitvami. Poleg tega ta API podpira shranjevanje obdelanih dokumentov v številnih podprtih formatih."

############################# Platforms ############################
platforms:
  enable: true
  title: "Neodvisnost platforme"
  description: "GroupDocs.Signature za .NET podpira naslednje operacijske sisteme, ogrodja in upravitelje paketov"
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
  title: "Podprti formati datotek"
  description: |
    GroupDocs.Signature za .NET podpira operacije z naslednjimi [formati datotek](https://docs.groupdocs.com/signature/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office formati
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Slike in drugi formati
        * **Prenosni:** PDF
        * **Slike:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Drugi pisarniški formati:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Drugi formati
        * **Splet:** HTML, MHTML
        * **Arhivi:** ZIP, TAR, 7Z
        * **Certifikati:** PFX

############################# Features ############################
features:
  enable: true
  title: "Funkcije GroupDocs.Signature"
  description: "Hitro in natančno podpisovanje PDF-jev, pisarniških dokumentov in slik"

  items:
    # feature loop
    - icon: "sign"
      title: "Podpisovanje dokumentov"
      content: "Natančno dodajte eno ali več podprtih vrst podpisov na katerem koli določenem mestu v poslovnih dokumentih."

    # feature loop
    - icon: "custom"
      title: "Prilagodite podpise"
      content: "Uporabite funkcije, kot so barva, pisava, obroba, vrtenje itd., da konfigurirate videz podpisov."

    # feature loop
    - icon: "password"
      title: "Zaščita dokumenta z geslom"
      content: "Zavarujte določene vrste dokumentov z nastavitvijo gesla po podpisu."

    # feature loop
    - icon: "protect"
      title: "Zaščita pred spremembami"
      content: "Preprečite spremembe pomembnih poslovnih dokumentov po podpisu z digitalnim potrdilom."

    # feature loop
    - icon: "convert"
      title: "Pretvorite podpisane datoteke v druge formate"
      content: "Pretvorite podpisane datoteke v želene formate, kot je shranjevanje Wordovega dokumenta kot PDF."

    # feature loop
    - icon: "preview"
      title: "Izvleček predogledov strani"
      content: "Izvlecite strani iz podpisanih dokumentov kot posamezne slike za prihodnjo obdelavo."

    # feature loop
    - icon: "search"
      title: "Iskanje podpisov v dokumentih"
      content: "Pridobite informacije o predhodno dodanih podpisih v določenih dokumentih."

    # feature loop
    - icon: "validate"
      title: "Potrdite podpisane dokumente"
      content: "Preverite pravilno podpisovanje dokumentov s funkcijami za preverjanje veljavnosti."

    # feature loop
    - icon: "update"
      title: "Posodobite ali izbrišite podpise"
      content: "Preprosto prestavite določene podpise na strani, spremenite njihovo besedilo ali jih izbrišite brez težav."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Vzorci kod"
  description: "Nekateri primeri uporabe tipičnega GroupDocs.Signature za operacije .NET"
  items:
    # code sample loop
    - title: "Dodajte kodo QR v PDF"
      content: |
        Dodajanje [QR-kod](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) na določene strani dokumentov PDF lahko izboljša poslovne procese. Spodaj je primer dodajanja kode QR z uporabo GroupDocs.Signature.
        {{< landing/code title="Kako vstaviti QR kodo v PDF.">}}
        ```csharp {style=abap}
        // Naložite dokument za podpis
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Ustvarite možnosti kode QR z vnaprej določenim besedilom
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Konfigurirajte vrsto in položaj kodiranja kode QR na strani
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Podpišite dokument in ga shranite kot datoteko z rezultati
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Zaščita DOCX dokumenta z digitalnim potrdilom"
      content: |
        [Dokument](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) lahko [zaščitite] z uporabo osebnih podpisov ali podpisov podjetij, shranjenih kot digitalna potrdila. Takšnih zaščitenih dokumentov ni mogoče spremeniti brez razveljavitve podpisa.
        {{< landing/code title="Tukaj je opisano, kako zagotoviti celovitost dokumenta.">}}
        ```csharp {style=abap}   
        // Naložite dokument, ki ga želite digitalno podpisati
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // Določite možnosti digitalnega podpisovanja in navedite pot do datoteke potrdila
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Nastavite geslo za potrdilo
                Password = "1234567890"
            };
            // Podpišite dokument in ga shranite na želeno pot
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---
