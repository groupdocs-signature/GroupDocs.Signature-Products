---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:21
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: da
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, Cloud API'er og online dokumentsignaturapps"
head_description: "Få alt-i-et dokument-e-signaturløsning til .NET, Java og cloud-baserede applikationer. Signer almindelige dokumentformater online ved hjælp af simpel træk og slip-funktion"

############################# Header ############################
title: "Underskriv dokumenter<br>via Java API"
description: "Signer digitale dokumenter og billeder på enhver platform ved hjælp af vores fleksible API'er og app-baserede løsninger til programmører og slutbrugere."
words:
  for: "til"

actions:
  main: "Gratis download af Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Licensering"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Klar til at komme i gang?"
  description: "Prøv GroupDocs.Signature-funktioner gratis, eller anmod om en licens"

release:
  title: "Version {0} frigivet"
  notes: "Se, hvad der er nyt"
  downloads: "Downloads"

code:
  title: "Signer PDF-filer i Java"
  more: "Flere eksempler"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Vælg PDF-dokument
    Signature signature = new Signature("sample.pdf");
    
    // Giv tekst
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Underskriv dokument og gem til fil
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signatur Oversigt"
  description: "API til udførelse af dokumentsignering og relaterede handlinger i Java-applikationer"
  features:
    # feature loop
    - title: "Forbedrede forretningsdokumenter med digitale signaturer i Java"
      content: "Hurtig og tilpasselig signering: GroupDocs.Signature til Java tilbyder en bred vifte af digitale signaturmuligheder til PDF'er, billeder og Office-dokumenter. Du kan bruge tekst, stregkoder, QR-koder, digitale certifikater, billeder eller skjulte metadata. Dokumentbehandlingen er hurtig og effektiv."

    # feature loop
    - title: "Manipulering af underskrevne dokumenter"
      content: "Avanceret dokumentbehandling involverer kraftfulde operationer på signerede dokumenter ved hjælp af GroupDocs.Signature til Java. Du kan søge efter og validere signaturer, der er blevet tilføjet til forretningsdokumenter, ved hjælp af forskellige nyttige kriterier. Derudover kan du få adgang til detaljerede oplysninger om dokumentet eller få forhåndsvisningsbilleder af dets sider."

    # feature loop
    - title: "Forskellige outputvalg"
      content: "Robuste signeringsmuligheder giver dig mulighed for at tilpasse outputtet til dokumenter, der er signeret med GroupDocs.Signature til Java. Du kan præcist placere enhver signatur på enhver dokumentside og konfigurere dens udseende på forskellige måder. Java API understøtter lagring af signerede forretningsdokumenter i adskillige understøttede formater og giver muligheder for at sikre dem med adgangskoder."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platformens uafhængighed"
  description: "GroupDocs.Signature til Java understøtter følgende operativsystemer, rammer og pakkeadministratorer"
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
  title: "Understøttede filformater"
  description: |
    GroupDocs.Signature til Java understøtter operationer med følgende [filformater](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office-formater
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Billeder og andre formater
        * **Transportabel:** PDF
        * **Billeder:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Andre kontorformater:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Andre formater
        * **Web:** HTML, MHTML
        * **Arkiv:** ZIP, TAR, 7Z
        * **Certifikater:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature funktioner"
  description: "Signering af PDF'er, Office-dokumenter og billeder med digitale signaturer"

  items:
    # feature loop
    - icon: "sign"
      title: "Tilføjelse af signaturer"
      content: "Underskriv et dokument ved hjælp af forskellige understøttede signaturtyper ved at placere en digital signatur præcis på en hvilken som helst position på enhver side."

    # feature loop
    - icon: "custom"
      title: "Tilpasning af resultater"
      content: "Tilpas signaturudseendet ved at justere farve, skrifttype, kant, rotation og andre funktioner for at opnå det ønskede resultat."

    # feature loop
    - icon: "password"
      title: "Sikring af dokumenter med adgangskode"
      content: "For mange understøttede dokumenttyper kan du beskytte det signerede dokument med en adgangskode."

    # feature loop
    - icon: "protect"
      title: "Forebyggelse af uautoriserede ændringer"
      content: "Beskyt vigtige forretningsdokumenter, der er underskrevet med et digitalt certifikat, mod uautoriserede ændringer."

    # feature loop
    - icon: "convert"
      title: "Opnå resultater i ønskede formater"
      content: "Få nemt signerede resultatfiler i ethvert understøttet format. Du kan også konvertere MS Word-dokumenter til PDF uden besvær."

    # feature loop
    - icon: "preview"
      title: "Forhåndsvisning af dokument"
      content: "Gem en hvilken som helst side i et dokument som et billede til fremtidig behandling."

    # feature loop
    - icon: "search"
      title: "Søger efter signaturer"
      content: "Det er muligt at få information om tidligere tilføjede signaturer i specifikke dokumenter."

    # feature loop
    - icon: "validate"
      title: "Validering af dokumenter"
      content: "Godkend rigtigheden af ​​underskrifter på ethvert underskrevet dokument."

    # feature loop
    - icon: "update"
      title: "Håndtering af signaturer"
      content: "Når en signatur er placeret på en dokumentside, kan den slettes, flyttes eller opdateres efter behov."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kodeprøver"
  description: "Nogle bruger tilfælde af typiske GroupDocs.Signature til Java-operationer"
  items:
    # code sample loop
    - title: "Forbedr PDF-dokument med QR-kode"
      content: |
        Det kan være værdifuldt at forbedre forretningsprocesser ved at tilføje [QR-koder](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) til specifikke sider af PDF-dokumenter. Der er et eksempel på, hvordan man tilføjer en QR-kode ved hjælp af GroupDocs.Signature til Java.
        {{< landing/code title="Forbedr PDF-dokument med QR-kode">}}
        ```java {style=abap}
        // Indlæs dokumentet for at underskrive
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Opret QR-kodeindstillinger med foruddefineret tekst
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurer QR-kodekodningstype og position på siden
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Underskriv dokumentet og gem det som resultatfil
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Brug digital signatur til at beskytte en DOCX"
      content: |
        Du kan [Beskyt et dokument](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) ved at bruge personlige eller virksomhedssignaturer gemt som digitale certifikater. Dokumenter sikret med certifikat kan ikke ændres uden at ugyldiggøre signaturen.
        {{< landing/code title="Brug digital signatur til at beskytte en DOCX">}}
        ```java {style=abap}   
        // Indlæs dokumentet, der skal signeres digitalt
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Angiv muligheder for digital signering, og angiv stien til certifikatfilen
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Indstil certifikatets adgangskode
        options.setPassword("1234567890");

        // Underskriv dokumentet og gem det på den ønskede sti
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
