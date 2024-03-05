---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: ca
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: ".NET, Java, API de núvol i aplicacions de signatura de documents en línia"
head_description: "Obteniu una solució de signatura electrònica de documents tot en un per a aplicacions .NET, Java i basades en núvol. Signeu formats de document habituals en línia mitjançant la funció d'arrossegar i deixar anar"

############################# Header ############################
title: "Signar documents<br>amb l'API Node.js"
description: "Signa documents i imatges digitals a qualsevol plataforma utilitzant les nostres API flexibles i solucions basades en aplicacions per a programadors i usuaris finals."
words:
  for: "per"

actions:
  main: "Descarrega des de NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Llicència"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Preparat per començar?"
  description: "Proveu les funcions de GroupDocs.Signature de manera gratuïta o sol·liciteu una llicència"

release:
  title: "S'ha publicat la versió {0}"
  notes: "Mira què hi ha de nou"
  downloads: "Descàrregues"

code:
  title: "Signatura de PDF per Node.js"
  more: "Més exemples"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Seleccioneu el document PDF
    let signature = new Signature("sample.pdf");
    
    // Proporcioneu text
    let options = new TextSignOptions("John Smith");
    
    // Estableix el color
    options.ForeColor = Color.Red;
    
    // Signa el document i desa al fitxer
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Visió general de GroupDocs.Signature"
  description: "Biblioteca de signatura de documents a punt per utilitzar-se a les aplicacions Node.js"
  features:
    # feature loop
    - title: "Solució de signatures digitals per a documents empresarials amb Node.js"
      content: "GroupDocs.Signature for Node.js via Java ofereix un conjunt complet d'opcions de signatura digital per a documents PDF, Office i imatges. Hi ha text, codis de barres, imatges, certificats digitals i metadades disponibles. El processament de documents racionalitzat garanteix l'eficiència."

    # feature loop
    - title: "Manipulació avançada de documents signats"
      content: "GroupDocs.Signature us permet processar documents signats. Cerca i valida les signatures utilitzant diversos criteris. A més, extreu informació detallada del document o genereu imatges de vista prèvia de pàgines."

    # feature loop
    - title: "Formats de sortida diversos"
      content: "La nostra solució proporciona un control ampli sobre el format de sortida dels documents signats. Col·loqueu les signatures amb precisió a qualsevol pàgina i personalitzeu-ne l'aspecte. Deseu documents signats en nombrosos formats compatibles i, opcionalment, protegiu-los amb contrasenyes."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independència de la plataforma"
  description: "GroupDocs.Signature for Node.js via Java realitza el processament de documents amb diversos sistemes operatius"
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
  title: "Formats de fitxer compatibles"
  description: |
    GroupDocs.Signature for Node.js via Java facilita les operacions per als [formats de fitxer populars](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "Característiques de GroupDocs.Signature"
  description: "Signa PDF, documents d'Office i imatges amb signatures digitals"

  items:
    # feature loop
    - icon: "sign"
      title: "Signatures comercials"
      content: "Utilitzeu diversos tipus de signatura per signar documents. Col·loqueu signatures digitals amb precisió a qualsevol ubicació de la pàgina."

    # feature loop
    - icon: "custom"
      title: "Personalització de l'aparença de la signatura"
      content: "Adapteu els aspectes visuals de les signatures ajustant el color, el tipus de lletra, les vores, la rotació i més per aconseguir el resultat desitjat."

    # feature loop
    - icon: "password"
      title: "Documents protegits amb contrasenya"
      content: "Per a molts formats de documents admesos, protegiu els documents signats amb una contrasenya per a més seguretat."

    # feature loop
    - icon: "protect"
      title: "Prevenció de modificacions no autoritzades"
      content: "Protegiu els documents empresarials crucials signats amb certificats digitals d'alteracions no autoritzades."

    # feature loop
    - icon: "convert"
      title: "Formats de sortida desitjats"
      content: "Obteniu documents signats sense esforç en qualsevol format compatible. Converteix documents de MS Word a format PDF amb facilitat."

    # feature loop
    - icon: "preview"
      title: "Previsualització de documents"
      content: "Deseu pàgines de documents individuals com a imatges per a necessitats futures."

    # feature loop
    - icon: "search"
      title: "Cerca de signatures"
      content: "Recupereu informació sobre signatures afegides anteriorment als vostres documents."

    # feature loop
    - icon: "validate"
      title: "Validació de documents"
      content: "Verificar l'autenticitat de les signatures presentades en qualsevol document."

    # feature loop
    - icon: "update"
      title: "Gestió de signatures"
      content: "Suprimiu, canvieu o modifiqueu les signatures col·locades a qualsevol pàgina del document."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de codi"
  description: "Exemples il·lustratius que mostren les operacions típiques de GroupDocs.Signature for Node.js via Java"
  items:
    # code sample loop
    - title: "Marqueu PDF amb codis QR"
      content: |
        La incorporació de [codis de barres](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) a pàgines específiques de documents PDF pot agilitzar els processos empresarials. Aquesta secció ofereix un exemple d'afegir un codi QR amb GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Com posar codi QR a PDF.">}}
        ```javascript {style=abap}
        // Carregueu el document per signar
        let signature = new Signature("file_to_sign.pdf");
        
        // Creeu opcions de codi QR amb text predefinit
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configura el tipus i la posició de codificació del codi QR a la pàgina
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Signeu el document i deseu-lo com a fitxer de resultats
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Protecció d'un DOCX amb una signatura digital"
      content: |
        [Protegiu els vostres documents](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) mitjançant signatures basades en certificats digitals. La signatura digital protegeix els documents empresarials contra els canvis de contingut.
        {{< landing/code title="A continuació s'explica com garantir la integritat del document.">}}
        ```javascript {style=abap}   
        // Carregueu el document per signar digitalment
        let signature = new Signature("file_to_sign.docx");
        
        // Especifiqueu les opcions de signatura digital i proporcioneu el camí al fitxer de certificat
        let options = new DigitalSignOptions("certificate.pfx");

        // Establiu la contrasenya del certificat
        options.Password = "1234567890";

        // Signeu el document i deseu-lo al camí desitjat
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
