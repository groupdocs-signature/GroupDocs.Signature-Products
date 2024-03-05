---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:01
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
head_title: ".NET, Java, API de núvol i aplicacions de signatura de documents en línia"
head_description: "Obteniu una solució de signatura electrònica de documents tot en un per a aplicacions .NET, Java i basades en núvol. Signeu formats de document habituals en línia mitjançant la funció d'arrossegar i deixar anar"

############################# Header ############################
title: "Signar documents<br>mitjançant .NET API"
description: "Signa documents i imatges digitals a qualsevol plataforma utilitzant les nostres API flexibles i solucions basades en aplicacions per a programadors i usuaris finals."
words:
  for: "per"

actions:
  main: "Descàrrega gratuïta de NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Llicència"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Preparat per començar?"
  description: "Proveu les funcions de GroupDocs.Signature de manera gratuïta o sol·liciteu una llicència"

release:
  title: "S'ha publicat la versió {0}"
  notes: "Mira què hi ha de nou"
  downloads: "Descàrregues"

code:
  title: "Signar fitxers PDF en C#"
  more: "Més exemples"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Seleccioneu el document PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Proporcioneu text
        var options = new TextSignOptions("John Smith")
        {
            // Estableix el color
            ForeColor = Color.Red
        };
        // Signa el document i desa al fitxer
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Visió general de GroupDocs.Signature"
  description: "API per realitzar la signatura de documents i operacions relacionades en aplicacions .NET"
  features:
    # feature loop
    - title: "Afegir signatures als documents empresarials en C#"
      content: "Signatura de documents: amb GroupDocs.Signature per a .NET, podeu afegir diversos tipus de signatures, com ara text, imatges, codis de barres i certificats digitals, als documents PDF i Office. Aquesta API us permet signar els vostres documents amb gairebé qualsevol tipus de dades, incloses les metadades ocultes."

    # feature loop
    - title: "Tramitació de documents signats"
      content: "Processament addicional: podeu realitzar operacions potents en documents signats mitjançant GroupDocs.Signature. Això inclou la cerca de signatures existents als documents empresarials i verificar-les mitjançant criteris específics. A més, podeu recuperar la informació del document i les pàgines de vista prèvia mitjançant aquesta API .NET."

    # feature loop
    - title: "Personalització dels resultats"
      content: "GroupDocs.Signature per a .NET ofereix àmplies opcions de personalització. Podeu col·locar signatures amb precisió a qualsevol lloc de la pàgina del document i ajustar-ne l'aparença mitjançant una varietat de paràmetres. A més, aquesta API admet desar documents processats en una àmplia gamma de formats compatibles."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independència de la plataforma"
  description: "GroupDocs.Signature per a .NET admet els següents sistemes operatius, marcs i gestors de paquets"
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
    GroupDocs.Signature per a .NET admet operacions amb els següents [formats de fitxer](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  description: "Signar PDF, documents d'oficina i imatges de manera ràpida i precisa"

  items:
    # feature loop
    - icon: "sign"
      title: "Signatura de documents"
      content: "Afegiu un o diversos tipus de signatures compatibles amb precisió a qualsevol posició especificada dels documents empresarials."

    # feature loop
    - icon: "custom"
      title: "Personalitza les signatures"
      content: "Utilitzeu funcions com ara el color, el tipus de lletra, la vora, la rotació, etc., per configurar l'aspecte de les signatures."

    # feature loop
    - icon: "password"
      title: "Protecció amb contrasenya de documents"
      content: "Assegureu certs tipus de documents establint una contrasenya després de signar."

    # feature loop
    - icon: "protect"
      title: "Protecció davant els canvis"
      content: "Eviteu canvis en documents empresarials importants després d'afegir una signatura amb un certificat digital."

    # feature loop
    - icon: "convert"
      title: "Converteix fitxers signats a altres formats"
      content: "Converteix fitxers signats als formats desitjats, com ara desar un document de Word com a PDF."

    # feature loop
    - icon: "preview"
      title: "Extreu visualitzacions prèvies de la pàgina"
      content: "Extraieu pàgines de documents signats com a imatges individuals per a un processament futur."

    # feature loop
    - icon: "search"
      title: "Cerca de signatures als documents"
      content: "Recuperar informació sobre signatures afegides anteriorment en documents específics."

    # feature loop
    - icon: "validate"
      title: "Validació dels documents signats"
      content: "Verifiqueu la signatura correcta dels documents mitjançant funcions de validació."

    # feature loop
    - icon: "update"
      title: "Actualitzar o eliminar signatures"
      content: "Canvieu fàcilment signatures específiques en una pàgina, modifiqueu-ne el text o suprimiu-les sense cap problema."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de codi"
  description: "Alguns casos d'ús de GroupDocs.Signature típics per a operacions .NET"
  items:
    # code sample loop
    - title: "Afegeix el codi QR al PDF"
      content: |
        Afegir [codis QR](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) a pàgines específiques de documents PDF pot millorar els processos empresarials. A continuació es mostra un exemple de com afegir un codi QR mitjançant GroupDocs.Signature.
        {{< landing/code title="Com posar codi QR a PDF.">}}
        ```csharp {style=abap}
        // Carregueu el document per signar
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Creeu opcions de codi QR amb text predefinit
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Configura el tipus i la posició de codificació del codi QR a la pàgina
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Signeu el document i deseu-lo com a fitxer de resultats
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Protecció d'un document DOCX mitjançant un certificat digital"
      content: |
        Podeu [Protegir un document](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) utilitzant signatures personals o corporatives emmagatzemades com a certificats digitals. Aquests documents protegits no es poden modificar sense invalidar la signatura.
        {{< landing/code title="A continuació s'explica com garantir la integritat del document.">}}
        ```csharp {style=abap}   
        // Carregueu el document per signar digitalment
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // Especifiqueu les opcions de signatura digital i proporcioneu el camí al fitxer de certificat
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Establiu la contrasenya del certificat
                Password = "1234567890"
            };
            // Signeu el document i deseu-lo al camí desitjat
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---
