---
############################# Static ############################
layout: "landing"
date: 2023-10-23T14:58:09
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
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, API-ji v oblaku in aplikacije za spletno podpisovanje dokumentov"
head_description: "Pridobite vsestransko rešitev za e-podpisovanje dokumentov za .NET, Java in aplikacije v oblaku. Spletno podpišite običajne formate dokumentov s preprosto funkcijo povleci in spusti"

############################# Header ############################
title: "Podpišite dokumente<br>preko Java API"
description: "Podpisujte digitalne dokumente in slike na kateri koli platformi z uporabo naših prilagodljivih API-jev in rešitev, ki temeljijo na aplikacijah, za programerje in končne uporabnike."
words:
  for: "za"

actions:
  main: "Brezplačen prenos Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Licenciranje"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Ste pripravljeni začeti?"
  description: "Preizkusite funkcije GroupDocs.Signature brezplačno ali zahtevajte licenco"

release:
  title: "Izdana različica {0}"
  notes: "Oglejte si, kaj je novega"
  downloads: "Prenosi"

code:
  title: "Podpišite datoteke PDF v Javi"
  more: "Več primerov"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Izberite dokument PDF
    Signature signature = new Signature("sample.pdf");
    
    // Navedite besedilo
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Podpišite dokument in ga shranite v datoteko
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Pregled"
  description: "API za izvajanje podpisovanja dokumentov in povezanih operacij v aplikacijah Java"
  features:
    # feature loop
    - title: "Izboljšani poslovni dokumenti z digitalnimi podpisi v Javi"
      content: "Hitro in prilagodljivo podpisovanje: GroupDocs.Signature for Java ponuja široko paleto možnosti digitalnega podpisovanja za PDF-je, slike in dokumente Office. Uporabite lahko besedilo, črtne kode, QR-kode, digitalna potrdila, slike ali skrite metapodatke. Obdelava dokumentov je hitra in učinkovita."

    # feature loop
    - title: "Manipulacija podpisanih dokumentov"
      content: "Napredna obdelava dokumentov vključuje zmogljive operacije na podpisanih dokumentih z uporabo GroupDocs.Signature for Java. Podpise, ki so bili dodani poslovnim dokumentom, lahko iščete in preverjate z različnimi uporabnimi kriteriji. Poleg tega lahko dostopate do podrobnih informacij o dokumentu ali pridobite slike predogleda njegovih strani."

    # feature loop
    - title: "Raznolikost izbire izhoda"
      content: "Robustne možnosti podpisovanja vam omogočajo, da prilagodite izpis za dokumente, podpisane s GroupDocs.Signature for Java. Vsak podpis lahko natančno postavite na katero koli stran dokumenta in na različne načine konfigurirate njegov videz. Java API podpira shranjevanje podpisanih poslovnih dokumentov v številnih podprtih formatih in ponuja možnosti za njihovo zaščito z gesli."

############################# Platforms ############################
platforms:
  enable: true
  title: "Neodvisnost platforme"
  description: "GroupDocs.Signature for Java podpira naslednje operacijske sisteme, ogrodja in upravitelje paketov"
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
  title: "Podprti formati datotek"
  description: |
    GroupDocs.Signature za Javo podpira operacije z naslednjimi [formati datotek](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  description: "Podpisovanje PDF-jev, pisarniških dokumentov in slik z digitalnimi podpisi"

  items:
    # feature loop
    - icon: "sign"
      title: "Dodajanje podpisov"
      content: "Podpišite dokument z različnimi podprtimi vrstami podpisov tako, da postavite digitalni podpis natančno na poljubno mesto na kateri koli strani."

    # feature loop
    - icon: "custom"
      title: "Prilagajanje rezultatov"
      content: "Prilagodite videz podpisa tako, da prilagodite barvo, pisavo, rob, vrtenje in druge funkcije, da dosežete želeni rezultat."

    # feature loop
    - icon: "password"
      title: "Varovanje dokumentov z geslom"
      content: "Za številne podprte vrste dokumentov lahko podpisan dokument zaščitite z geslom."

    # feature loop
    - icon: "protect"
      title: "Preprečevanje nepooblaščenih sprememb"
      content: "Zaščitite pomembne poslovne dokumente, podpisane z digitalnim potrdilom, pred nepooblaščenimi spremembami."

    # feature loop
    - icon: "convert"
      title: "Pridobivanje rezultatov v želenih oblikah"
      content: "Enostavno pridobite podpisane datoteke rezultatov v katerem koli podprtem formatu. Dokumente MS Word lahko tudi preprosto pretvorite v PDF."

    # feature loop
    - icon: "preview"
      title: "Predogled dokumenta"
      content: "Shranite katero koli stran dokumenta kot sliko za prihodnjo obdelavo."

    # feature loop
    - icon: "search"
      title: "Iskanje podpisov"
      content: "V določenih dokumentih je možno pridobiti podatke o predhodno dodanih podpisih."

    # feature loop
    - icon: "validate"
      title: "Potrjevanje dokumentov"
      content: "Preverite pravilnost podpisov na katerem koli podpisanem dokumentu."

    # feature loop
    - icon: "update"
      title: "Upravljanje podpisov"
      content: "Ko je podpis postavljen na stran dokumenta, ga je mogoče po potrebi izbrisati, premakniti ali posodobiti."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Vzorci kod"
  description: "Nekateri primeri uporabe tipičnih operacij GroupDocs.Signature za Java"
  items:
    # code sample loop
    - title: "Izboljšajte dokument PDF s kodo QR"
      content: |
        Izboljšanje poslovnih procesov z dodajanjem [QR-kod](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) na določene strani dokumentov PDF je lahko koristno. Obstaja primer, kako dodati kodo QR z uporabo GroupDocs.Signature for Java.
        {{< landing/code title="Izboljšajte dokument PDF s kodo QR">}}
        ```java {style=abap}
        // Naložite dokument za podpis
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Ustvarite možnosti kode QR z vnaprej določenim besedilom
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurirajte vrsto in položaj kodiranja kode QR na strani
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Podpišite dokument in ga shranite kot datoteko z rezultati
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Za zaščito DOCX uporabite digitalni podpis"
      content: |
        [Dokument](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) lahko [zaščitite] z uporabo osebnih podpisov ali podpisov podjetij, shranjenih kot digitalna potrdila. Dokumentov, zavarovanih s potrdilom, ni mogoče spremeniti brez razveljavitve podpisa.
        {{< landing/code title="Za zaščito DOCX uporabite digitalni podpis">}}
        ```java {style=abap}   
        // Naložite dokument, ki ga želite digitalno podpisati
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Določite možnosti digitalnega podpisovanja in navedite pot do datoteke potrdila
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Nastavite geslo za potrdilo
        options.setPassword("1234567890");

        // Podpišite dokument in ga shranite na želeno pot
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
