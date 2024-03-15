---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:49
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: ca
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
head_title: "Biblioteca de signatures digitals de Java - GroupDocs.Signature"
head_description: "Potencia les aplicacions Java mitjançant signatures electròniques amb GroupDocs.Signature. Signeu documents comercials de manera ràpida i senzilla."

############################# Header ############################
title: "Signar documents<br>mitjançant l'API de Java"
description: "Signa documents i imatges digitals a qualsevol plataforma utilitzant les nostres API flexibles i solucions basades en aplicacions per a programadors i usuaris finals."
words:
  for: "per"

actions:
  main: "Descàrrega gratuïta de Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Llicència"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Preparat per començar?"
  description: "Proveu les funcions de GroupDocs.Signature de manera gratuïta o sol·liciteu una llicència"

release:
  title: "S'ha publicat la versió {0}"
  notes: "Mira què hi ha de nou"
  downloads: "Descàrregues"

code:
  title: "Signar fitxers PDF en Java"
  more: "Més exemples"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Seleccioneu el document PDF
    Signature signature = new Signature("sample.pdf");
    
    // Proporcioneu text
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Signa el document i desa al fitxer
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Visió general de GroupDocs.Signature"
  description: "API per dur a terme la signatura de documents i operacions relacionades en aplicacions Java"
  features:
    # feature loop
    - title: "Documents empresarials millorats amb signatures digitals en Java"
      content: "Signatura ràpida i personalitzable: GroupDocs.Signature per a Java ofereix una àmplia gamma d'opcions de signatura digital per a PDF, imatges i documents d'Office. Podeu utilitzar text, codis de barres, codis QR, certificats digitals, imatges o metadades ocultes. El processament de documents és ràpid i eficient."

    # feature loop
    - title: "Manipulació de documents signats"
      content: "El processament avançat de documents implica operacions potents en documents signats mitjançant GroupDocs.Signature per a Java. Podeu cercar i validar signatures que s'han afegit als documents empresarials mitjançant diversos criteris útils. A més, podeu accedir a informació detallada sobre el document o obtenir imatges de vista prèvia de les seves pàgines."

    # feature loop
    - title: "Varietat d'opcions de sortida"
      content: "Les opcions de signatura sòlides us permeten personalitzar la sortida dels documents signats amb GroupDocs.Signature per a Java. Podeu col·locar amb precisió qualsevol signatura a qualsevol pàgina del document i configurar-ne l'aparença de diverses maneres. L'API de Java admet desar documents comercials signats en nombrosos formats compatibles i ofereix opcions per protegir-los amb contrasenyes."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independència de la plataforma"
  description: "GroupDocs.Signature per a Java admet els següents sistemes operatius, marcs i gestors de paquets"
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
  title: "Formats de fitxer compatibles"
  description: |
    GroupDocs.Signature per a Java admet operacions amb els següents [formats de fitxer](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formats de Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Imatges i altres formats
        * **Portàtil:** PDF
        * **Imatges:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Altres formats d'oficina:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Altres formats
        * **Web:** HTML, MHTML
        * **Arxius:** ZIP, TAR, 7Z
        * **Certificats:** PFX

############################# Features ############################
features:
  enable: true
  title: "Funcions de GroupDocs.Signature"
  description: "Signatura de PDF, documents d'oficina i imatges amb signatures digitals"

  items:
    # feature loop
    - icon: "sign"
      title: "Afegir signatures"
      content: "Signeu un document amb diversos tipus de signatura compatibles col·locant una signatura digital precisament en qualsevol posició de qualsevol pàgina."

    # feature loop
    - icon: "custom"
      title: "Personalització dels resultats"
      content: "Personalitzeu l'aspecte de la signatura ajustant el color, el tipus de lletra, la vora, la rotació i altres funcions per aconseguir el resultat desitjat."

    # feature loop
    - icon: "password"
      title: "Protecció de documents amb contrasenya"
      content: "Per a molts tipus de documents admesos, podeu protegir el document signat amb una contrasenya."

    # feature loop
    - icon: "protect"
      title: "Prevenció de canvis no autoritzats"
      content: "Protegiu els documents comercials importants signats amb un certificat digital de modificacions no autoritzades."

    # feature loop
    - icon: "convert"
      title: "Obtenció de resultats en els formats desitjats"
      content: "Obteniu fàcilment fitxers de resultats signats en qualsevol format compatible. També podeu convertir documents de MS Word a PDF sense esforç."

    # feature loop
    - icon: "preview"
      title: "Vista prèvia del document"
      content: "Deseu qualsevol pàgina d'un document com a imatge per a un processament futur."

    # feature loop
    - icon: "search"
      title: "Recerca de signatures"
      content: "És possible obtenir informació sobre signatures afegides anteriorment en documents específics."

    # feature loop
    - icon: "validate"
      title: "Validació de documents"
      content: "Valida la correcció de les signatures en qualsevol document signat."

    # feature loop
    - icon: "update"
      title: "Gestió de signatures"
      content: "Un cop s'ha col·locat una signatura a la pàgina d'un document, es pot esborrar, moure o actualitzar segons sigui necessari."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de codi"
  description: "Alguns casos d'ús de les operacions típiques de GroupDocs.Signature per a Java"
  items:
    # code sample loop
    - title: "Millora el document PDF amb el codi QR"
      content: |
        Millorar els processos empresarials afegint [codis QR](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) a pàgines específiques de documents PDF pot ser valuós. Hi ha un exemple de com afegir un codi QR amb GroupDocs.Signature per a Java.
        {{< landing/code title="Millora el document PDF amb el codi QR">}}
        ```java {style=abap}
        // Carregueu el document per signar
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Creeu opcions de codi QR amb text predefinit
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configura el tipus i la posició de codificació del codi QR a la pàgina
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Signeu el document i deseu-lo com a fitxer de resultats
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Utilitzeu la signatura digital per protegir un DOCX"
      content: |
        Podeu [protegir un document](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) utilitzant signatures personals o corporatives emmagatzemades com a certificats digitals. Els documents assegurats amb certificat no es poden alterar sense invalidar la signatura.
        {{< landing/code title="Utilitzeu la signatura digital per protegir un DOCX">}}
        ```java {style=abap}   
        // Carregueu el document per signar digitalment
        Signature signature = new Signature("file_to_sign.docx");
        
        // Especifiqueu les opcions de signatura digital i proporcioneu el camí al fitxer de certificat
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Establiu la contrasenya del certificat
        options.setPassword("1234567890");

        // Signeu el document i deseu-lo al camí desitjat
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---
