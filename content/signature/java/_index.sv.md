---
############################# Static ############################
layout: "landing"
date: 2023-10-23T14:58:09
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: sv
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, Cloud API och onlinedokumentsignaturappar"
head_description: "Få en allt-i-ett-dokumentlösning för e-signaturer för .NET, Java och molnbaserade applikationer. Signera vanliga dokumentformat online med en enkel dra och släpp-funktion"

############################# Header ############################
title: "Signera dokument<br>via Java API"
description: "Signera digitala dokument och bilder på vilken plattform som helst med hjälp av våra flexibla API:er och appbaserade lösningar för programmerare och slutanvändare."
words:
  for: "för"

actions:
  main: "Gratis nedladdning av Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Licensiering"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Redo att komma igång?"
  description: "Prova GroupDocs.Signature-funktioner gratis eller begär en licens"

release:
  title: "Version {0} släpptes"
  notes: "Se vad som är nytt"
  downloads: "Nedladdningar"

code:
  title: "Signera PDF-filer i Java"
  more: "Fler exempel"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Välj PDF-dokument
    Signature signature = new Signature("sample.pdf");
    
    // Ge text
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Signera dokument och spara till fil
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Översikt"
  description: "API för att utföra dokumentsignering och relaterade operationer i Java-applikationer"
  features:
    # feature loop
    - title: "Förbättrade affärsdokument med digitala signaturer i Java"
      content: "Snabb och anpassningsbar signering: GroupDocs.Signature för Java erbjuder ett brett utbud av digitala signaturalternativ för PDF-filer, bilder och Office-dokument. Du kan använda text, streckkoder, QR-koder, digitala certifikat, bilder eller dold metadata. Dokumentbehandlingen är snabb och effektiv."

    # feature loop
    - title: "Manipulera undertecknade dokument"
      content: "Avancerad dokumentbehandling involverar kraftfulla operationer på signerade dokument med GroupDocs.Signature för Java. Du kan söka efter och validera signaturer som har lagts till i affärsdokument med hjälp av olika användbara kriterier. Dessutom kan du få tillgång till detaljerad information om dokumentet eller få förhandsvisningsbilder av dess sidor."

    # feature loop
    - title: "Olika utgångsalternativ"
      content: "Robusta signeringsalternativ låter dig anpassa utdata för dokument signerade med GroupDocs.Signature for Java. Du kan placera vilken signatur som helst på vilken dokumentsida som helst och konfigurera dess utseende på olika sätt. Java API stöder att spara signerade affärsdokument i många format som stöds och ger alternativ för att skydda dem med lösenord."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformsoberoende"
  description: "GroupDocs.Signature för Java stöder följande operativsystem, ramverk och pakethanterare"
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
  title: "Filformat som stöds"
  description: |
    GroupDocs.Signature för Java stöder operationer med följande [filformat](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office-format
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Bilder och andra format
        * **Bärbar:** PDF
        * **Bilder:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Andra kontorsformat:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Andra format
        * **webb:** HTML, MHTML
        * **Arkiv:** ZIP, TAR, 7Z
        * **Certifikat:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature-funktioner"
  description: "Signera PDF-filer, Office-dokument och bilder med digitala signaturer"

  items:
    # feature loop
    - icon: "sign"
      title: "Lägga till signaturer"
      content: "Signera ett dokument med olika signaturtyper som stöds genom att placera en digital signatur exakt var som helst på vilken sida som helst."

    # feature loop
    - icon: "custom"
      title: "Anpassa resultat"
      content: "Anpassa signaturutseendet genom att justera färg, teckensnitt, ram, rotation och andra funktioner för att uppnå önskat resultat."

    # feature loop
    - icon: "password"
      title: "Säkra dokument med lösenord"
      content: "För många dokumenttyper som stöds kan du skydda det signerade dokumentet med ett lösenord."

    # feature loop
    - icon: "protect"
      title: "Förhindra obehöriga ändringar"
      content: "Skydda viktiga affärsdokument signerade med ett digitalt certifikat från obehöriga ändringar."

    # feature loop
    - icon: "convert"
      title: "Få resultat i önskade format"
      content: "Få enkelt signerade resultatfiler i alla format som stöds. Du kan också konvertera MS Word-dokument till PDF utan ansträngning."

    # feature loop
    - icon: "preview"
      title: "Förhandsgranskning av dokument"
      content: "Spara vilken sida som helst i ett dokument som en bild för framtida bearbetning."

    # feature loop
    - icon: "search"
      title: "Söker efter signaturer"
      content: "Det är möjligt att få information om tidigare tillagda signaturer i specifika dokument."

    # feature loop
    - icon: "validate"
      title: "Validera dokument"
      content: "Validera riktigheten av underskrifter på alla undertecknade dokument."

    # feature loop
    - icon: "update"
      title: "Hantera signaturer"
      content: "När en signatur väl har placerats på en dokumentsida kan den tas bort, flyttas eller uppdateras efter behov."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kodprover"
  description: "Vissa använder fall av typiska GroupDocs.Signature för Java-operationer"
  items:
    # code sample loop
    - title: "Förbättra PDF-dokument med QR-kod"
      content: |
        Att förbättra affärsprocesser genom att lägga till [QR-koder](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) på specifika sidor i PDF-dokument kan vara värdefullt. Det finns ett exempel på hur man lägger till en QR-kod med GroupDocs.Signature för Java.
        {{< landing/code title="Förbättra PDF-dokument med QR-kod">}}
        ```java {style=abap}
        // Ladda dokumentet för att signera
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Skapa QR-kodalternativ med fördefinierad text
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurera QR-kodskodningstyp och position på sidan
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Signera dokumentet och spara det som resultatfil
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Använd digital signatur för att skydda en DOCX"
      content: |
        Du kan [Skydda ett dokument](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) genom att använda personliga eller företagssignaturer som lagras som digitala certifikat. Dokument säkrade med certifikat kan inte ändras utan att signaturen ogiltigförklaras.
        {{< landing/code title="Använd digital signatur för att skydda en DOCX">}}
        ```java {style=abap}   
        // Ladda dokumentet som ska signeras digitalt
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Ange alternativ för digital signering och ange sökvägen till certifikatfilen
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Ställ in certifikatlösenordet
        options.setPassword("1234567890");

        // Signera dokumentet och spara det på önskad sökväg
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
