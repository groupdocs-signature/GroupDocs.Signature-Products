---
############################# Static ############################
layout: "landing"
date: 2024-02-29T14:43:05
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: hr
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

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
head_title: ".NET, Java, Cloud API-ji i online aplikacije za potpisivanje dokumenata"
head_description: "Nabavite sveobuhvatno rješenje za e-potpis dokumenata za .NET, Java i aplikacije temeljene na oblaku. Potpišite uobičajene formate dokumenata na mreži koristeći jednostavnu značajku povlačenja i ispuštanja"

############################# Header ############################
title: "Potpišite dokumente<br>putem Java API-ja"
description: "Potpišite digitalne dokumente i slike na bilo kojoj platformi koristeći naše fleksibilne API-je i rješenja temeljena na aplikacijama za programere i krajnje korisnike."
words:
  for: "za"

actions:
  main: "Besplatno preuzimanje Mavena"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Licenciranje"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Jeste li spremni za početak?"
  description: "Isprobajte značajke GroupDocs.Signature besplatno ili zatražite licencu"

release:
  title: "Objavljena verzija {0}"
  notes: "Pogledajte što je novo"
  downloads: "Preuzimanja"

code:
  title: "Potpišite PDF datoteke u Javi"
  more: "Više primjera"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Odaberite PDF dokument
    Signature signature = new Signature("sample.pdf");
    
    // Navedite tekst
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Potpišite dokument i spremite ga u datoteku
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Pregled GroupDocs.Signature"
  description: "API za izvođenje potpisivanja dokumenata i povezanih operacija u Java aplikacijama"
  features:
    # feature loop
    - title: "Poboljšani poslovni dokumenti s digitalnim potpisima u Javi"
      content: "Brzo i prilagodljivo potpisivanje: GroupDocs.Signature za Javu nudi širok raspon opcija digitalnog potpisa za PDF-ove, slike i Office dokumente. Možete koristiti tekst, crtične kodove, QR kodove, digitalne certifikate, slike ili skrivene metapodatke. Obrada dokumenata je brza i učinkovita."

    # feature loop
    - title: "Manipuliranje potpisanim dokumentima"
      content: "Napredna obrada dokumenata uključuje moćne operacije na potpisanim dokumentima pomoću GroupDocs.Signature za Javu. Potpise koji su dodani poslovnim dokumentima možete pretraživati ​​i provjeravati pomoću različitih korisnih kriterija. Osim toga, možete pristupiti detaljnim informacijama o dokumentu ili dobiti pregled slika njegovih stranica."

    # feature loop
    - title: "Raznolikost izbora izlaza"
      content: "Robusne opcije potpisivanja omogućuju vam da prilagodite izlaz za dokumente potpisane s GroupDocs.Signature for Java. Možete precizno postaviti bilo koji potpis na bilo koju stranicu dokumenta i konfigurirati njegov izgled na razne načine. Java API podržava spremanje potpisanih poslovnih dokumenata u brojnim podržanim formatima i pruža opcije za njihovu zaštitu lozinkama."

############################# Platforms ############################
platforms:
  enable: true
  title: "Neovisnost o platformi"
  description: "GroupDocs.Signature za Javu podržava sljedeće operativne sustave, okvire i upravitelje paketa"
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
  title: "Podržani formati datoteka"
  description: |
    GroupDocs.Signature za Javu podržava rad sa sljedećim [formatima datoteka](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
        ### Slike i drugi formati
        * **Prijenosni:** PDF
        * **Slike:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Ostali uredski formati:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Ostali formati
        * **mreža:** HTML, MHTML
        * **Arhiva:** ZIP, TAR, 7Z
        * **Certifikati:** PFX

############################# Features ############################
features:
  enable: true
  title: "Značajke GroupDocs.Signature"
  description: "Potpisivanje PDF-ova, Office dokumenata i slika digitalnim potpisima"

  items:
    # feature loop
    - icon: "sign"
      title: "Dodavanje potpisa"
      content: "Potpišite dokument pomoću različitih podržanih vrsta potpisa postavljanjem digitalnog potpisa precizno na bilo koje mjesto na bilo kojoj stranici."

    # feature loop
    - icon: "custom"
      title: "Prilagodba rezultata"
      content: "Prilagodite izgled potpisa podešavanjem boje, fonta, obruba, rotacije i drugih značajki kako biste postigli željeni rezultat."

    # feature loop
    - icon: "password"
      title: "Zaštita dokumenata lozinkom"
      content: "Za mnoge podržane vrste dokumenata možete zaštititi potpisani dokument lozinkom."

    # feature loop
    - icon: "protect"
      title: "Sprječavanje neovlaštenih promjena"
      content: "Zaštitite važne poslovne dokumente potpisane digitalnim certifikatom od neovlaštenih izmjena."

    # feature loop
    - icon: "convert"
      title: "Dobivanje rezultata u željenim formatima"
      content: "Jednostavno nabavite potpisane datoteke rezultata u bilo kojem podržanom formatu. Također možete pretvoriti MS Word dokumente u PDF bez napora."

    # feature loop
    - icon: "preview"
      title: "Pregled dokumenta"
      content: "Spremite bilo koju stranicu dokumenta kao sliku za buduću obradu."

    # feature loop
    - icon: "search"
      title: "Traženje potpisa"
      content: "Moguće je dobiti podatke o prethodno dodanim potpisima u određenim dokumentima."

    # feature loop
    - icon: "validate"
      title: "Potvrđivanje dokumenata"
      content: "Potvrdite ispravnost potpisa na svakom potpisanom dokumentu."

    # feature loop
    - icon: "update"
      title: "Upravljanje potpisima"
      content: "Nakon što se potpis postavi na stranicu dokumenta, može se po potrebi izbrisati, premjestiti ili ažurirati."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Uzorci kodova"
  description: "Neki slučajevi upotrebe tipičnih GroupDocs.Signature za Java operacije"
  items:
    # code sample loop
    - title: "Poboljšajte PDF dokument QR kodom"
      content: |
        Poboljšanje poslovnih procesa dodavanjem [QR-kodova](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) na određene stranice PDF dokumenata može biti dragocjeno. Postoji primjer kako dodati QR kod pomoću GroupDocs.Signature za Javu.
        {{< landing/code title="Poboljšajte PDF dokument QR kodom">}}
        ```java {style=abap}
        // Učitajte dokument za potpisivanje
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Stvorite opcije QR koda s unaprijed definiranim tekstom
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurirajte vrstu kodiranja QR koda i položaj na stranici
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Potpišite dokument i spremite ga kao datoteku rezultata
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Koristite digitalni potpis za zaštitu DOCX-a"
      content: |
        Možete [zaštititi dokument](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) pomoću osobnih ili korporativnih potpisa pohranjenih kao digitalni certifikati. Dokumenti osigurani certifikatom ne mogu se mijenjati bez poništavanja potpisa.
        {{< landing/code title="Koristite digitalni potpis za zaštitu DOCX-a">}}
        ```java {style=abap}   
        // Učitajte dokument koji želite digitalno potpisati
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Navedite opcije digitalnog potpisivanja i navedite put do datoteke certifikata
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Postavite lozinku certifikata
        options.setPassword("1234567890");

        // Potpišite dokument i spremite ga na željenu putanju
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
