---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:22
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: lt
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, debesies API ir internetinių dokumentų parašų programos"
head_description: "Gaukite „viskas viename“ dokumentų el. parašo sprendimą, skirtą .NET, „Java“ ir debesies programoms. Pasirašykite įprastus dokumentų formatus internete naudodami paprastą vilkimo ir nuleidimo funkciją"

############################# Header ############################
title: "Pasirašykite dokumentus<br>per Java API"
description: "Pasirašykite skaitmeninius dokumentus ir vaizdus bet kurioje platformoje naudodami mūsų lanksčias API ir programuotojams ir galutiniams vartotojams skirtus sprendimus."
words:
  for: "dėl"

actions:
  main: "Nemokamas Maven atsisiuntimas"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Licencijavimas"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Pasiruošę pradėti?"
  description: "Išbandykite GroupDocs.Signature funkcijas nemokamai arba paprašykite licencijos"

release:
  title: "Išleista {0} versija"
  notes: "Pažiūrėkite, kas naujo"
  downloads: "Atsisiuntimai"

code:
  title: "Pasirašykite PDF failus Java"
  more: "Daugiau pavyzdžių"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Pasirinkite PDF dokumentą
    Signature signature = new Signature("sample.pdf");
    
    // Pateikite tekstą
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Pasirašykite dokumentą ir išsaugokite faile
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Parašo apžvalga"
  description: "API, skirta dokumentų pasirašymui ir susijusioms operacijoms atlikti Java programose"
  features:
    # feature loop
    - title: "Patobulinti verslo dokumentai su skaitmeniniu parašu Java"
      content: "Greitas ir pritaikomas pasirašymas: „GroupDocs.Signature“, skirta „Java“, siūlo daugybę skaitmeninio parašo parinkčių PDF rinkmenoms, vaizdams ir „Office“ dokumentams. Galite naudoti tekstą, brūkšninius kodus, QR kodus, skaitmeninius sertifikatus, paveikslėlius arba paslėptus metaduomenis. Dokumentų tvarkymas yra greitas ir efektyvus."

    # feature loop
    - title: "Manipuliavimas pasirašytais dokumentais"
      content: "Išplėstinis dokumentų apdorojimas apima galingas operacijas su pasirašytais dokumentais naudojant GroupDocs.Signature for Java. Galite ieškoti ir patvirtinti parašus, kurie buvo pridėti prie verslo dokumentų, naudodami įvairius naudingus kriterijus. Be to, galite pasiekti išsamią informaciją apie dokumentą arba peržiūrėti jo puslapių vaizdus."

    # feature loop
    - title: "Išvesties pasirinkimų įvairovė"
      content: "Tvirtas pasirašymo parinktys leidžia tinkinti su GroupDocs.Signature for Java pasirašytų dokumentų išvestį. Galite tiksliai išdėstyti bet kurį parašą bet kuriame dokumento puslapyje ir įvairiais būdais konfigūruoti jo išvaizdą. „Java“ API palaiko pasirašytų verslo dokumentų išsaugojimą įvairiais palaikomais formatais ir suteikia galimybes apsaugoti juos slaptažodžiais."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platformos nepriklausomybė"
  description: "GroupDocs.Signature for Java palaiko šias operacines sistemas, sistemas ir paketų tvarkykles"
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
  title: "Palaikomi failų formatai"
  description: |
    GroupDocs.Signature for Java palaiko operacijas su šiais [failų formatais](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office formatai
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Vaizdai ir kiti formatai
        * **Nešiojami:** PDF
        * **Vaizdai:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Kiti biuro formatai:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Kiti formatai
        * **Žiniatinklis:** HTML, MHTML
        * **Archyvai:** ZIP, TAR, 7Z
        * **Sertifikatai:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Parašo funkcijos"
  description: "PDF, Office dokumentų ir vaizdų pasirašymas skaitmeniniais parašais"

  items:
    # feature loop
    - icon: "sign"
      title: "Parašų pridėjimas"
      content: "Pasirašykite dokumentą naudodami įvairius palaikomus parašo tipus, tiksliai padėdami skaitmeninį parašą bet kurioje bet kurio puslapio vietoje."

    # feature loop
    - icon: "custom"
      title: "Rezultatų pritaikymas"
      content: "Tinkinkite parašo išvaizdą koreguodami spalvą, šriftą, kraštinę, pasukimą ir kitas funkcijas, kad pasiektumėte norimą rezultatą."

    # feature loop
    - icon: "password"
      title: "Dokumentų apsauga slaptažodžiu"
      content: "Daugelio palaikomų dokumentų tipų atveju pasirašytą dokumentą galite apsaugoti slaptažodžiu."

    # feature loop
    - icon: "protect"
      title: "Neleistinų pakeitimų prevencija"
      content: "Apsaugokite svarbius verslo dokumentus, pasirašytus skaitmeniniu sertifikatu, nuo neteisėtų pakeitimų."

    # feature loop
    - icon: "convert"
      title: "Rezultatų gavimas norimais formatais"
      content: "Lengvai gaukite pasirašytus rezultatų failus bet kokiu palaikomu formatu. Taip pat galite lengvai konvertuoti MS Word dokumentus į PDF."

    # feature loop
    - icon: "preview"
      title: "Dokumento peržiūra"
      content: "Išsaugokite bet kurį dokumento puslapį kaip vaizdą, kad galėtumėte jį apdoroti ateityje."

    # feature loop
    - icon: "search"
      title: "Parašų paieška"
      content: "Informaciją apie anksčiau pridėtus parašus galima gauti konkrečiuose dokumentuose."

    # feature loop
    - icon: "validate"
      title: "Dokumentų tvirtinimas"
      content: "Patvirtinkite parašų teisingumą ant bet kurio pasirašyto dokumento."

    # feature loop
    - icon: "update"
      title: "Parašų tvarkymas"
      content: "Įdėjus parašą dokumento puslapyje, jį galima ištrinti, perkelti arba atnaujinti, jei reikia."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kodo pavyzdžiai"
  description: "Kai kurie naudoja tipinius GroupDocs.Signature Java operacijoms atvejus"
  items:
    # code sample loop
    - title: "Patobulinkite PDF dokumentą su QR kodu"
      content: |
        Verslo procesų tobulinimas pridedant [QR kodus](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) prie konkrečių PDF dokumentų puslapių gali būti naudingas. Yra pavyzdys, kaip pridėti QR kodą naudojant GroupDocs.Signature for Java.
        {{< landing/code title="Patobulinkite PDF dokumentą su QR kodu">}}
        ```java {style=abap}
        // Įdėkite dokumentą pasirašyti
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Sukurkite QR kodo parinktis su iš anksto nustatytu tekstu
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigūruokite QR kodo kodavimo tipą ir vietą puslapyje
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Pasirašykite dokumentą ir išsaugokite jį kaip rezultato failą
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Norėdami apsaugoti DOCX, naudokite skaitmeninį parašą"
      content: |
        Galite [Apsaugoti dokumentą](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) naudodami asmeninius arba įmonės parašus, saugomus kaip skaitmeninius sertifikatus. Sertifikatu apsaugoti dokumentai negali būti keičiami nepažeidžiant parašo.
        {{< landing/code title="Norėdami apsaugoti DOCX, naudokite skaitmeninį parašą">}}
        ```java {style=abap}   
        // Įkelkite dokumentą, kurį norite pasirašyti skaitmeniniu būdu
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Nurodykite skaitmeninio pasirašymo parinktis ir nurodykite kelią į sertifikato failą
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Nustatykite sertifikato slaptažodį
        options.setPassword("1234567890");

        // Pasirašykite dokumentą ir išsaugokite jį norimame kelyje
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
