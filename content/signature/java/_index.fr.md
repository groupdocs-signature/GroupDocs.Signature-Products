---
############################# Static ############################
layout: "landing"
date: 2024-07-25T14:25:12
draft: false

lang: fr
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
head_title: "Bibliothèque de signatures numériques Java - GroupDocs.Signature"
head_description: "Renforcez les applications Java grâce aux signatures électroniques avec GroupDocs.Signature. Signez des documents commerciaux rapidement et sans effort."

############################# Header ############################
title: "Signer des documents via l'API Java"
description: "Signez des documents et des images numériques sur n'importe quelle plate-forme à l'aide de nos API flexibles et de nos solutions basées sur des applications pour les programmeurs et les utilisateurs finaux."
words:
  for: "pour"

actions:
  main: "Téléchargement gratuit de Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Licence"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Prêt à commencer?"
  description: "Essayez les fonctionnalités de GroupDocs.Signature gratuitement ou demandez une licence"

release:
  title: "Version {0} publiée"
  notes: "Regardez ce qu'il y a de nouveau"
  downloads: "Téléchargements"

code:
  title: "Signer des fichiers PDF en Java"
  more: "Plus d'exemples"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Sélectionnez un document PDF
    Signature signature = new Signature("sample.pdf");
    
    // Fournir du texte
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Signer le document et l'enregistrer dans un fichier
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Présentation de GroupDocs.Signature"
  description: "API pour effectuer la signature de documents et les opérations associées dans les applications Java"
  features:
    # feature loop
    - title: "Documents commerciaux améliorés avec signatures numériques en Java"
      content: "Signature rapide et personnalisable : GroupDocs.Signature pour Java offre une large gamme d'options de signature numérique pour les PDF, les images et les documents Office. Vous pouvez utiliser du texte, des codes-barres, des codes QR, des certificats numériques, des images ou des métadonnées cachées. Le traitement des documents est rapide et efficace."

    # feature loop
    - title: "Manipulation de documents signés"
      content: "Le traitement avancé des documents implique des opérations puissantes sur les documents signés à l'aide de GroupDocs.Signature pour Java. Vous pouvez rechercher et valider les signatures ajoutées aux documents commerciaux à l'aide de divers critères utiles. De plus, vous pouvez accéder à des informations détaillées sur le document ou obtenir des images d'aperçu de ses pages."

    # feature loop
    - title: "Variété de choix de sortie"
      content: "Des options de signature robustes vous permettent de personnaliser la sortie des documents signés avec GroupDocs.Signature pour Java. Vous pouvez positionner avec précision n'importe quelle signature sur n'importe quelle page de document et configurer son apparence de différentes manières. L'API Java prend en charge l'enregistrement des documents commerciaux signés dans de nombreux formats pris en charge et propose des options pour les sécuriser avec des mots de passe."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Signature pour Java prend en charge les systèmes d'exploitation, frameworks et gestionnaires de packages suivants"
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
  title: "Formats de fichiers pris en charge"
  description: |
    GroupDocs.Signature pour Java prend en charge les opérations avec les [formats de fichiers](https://docs.groupdocs.com/signature/java/supported-document-formats/) suivants.
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formats Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Images et autres formats
        * **Portable:** PDF
        * **Images:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Autres formats de bureaux:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Autres formats
        * **la toile:** HTML, MHTML
        * **Les archives:** ZIP, TAR, 7Z
        * **Certificats:** PFX

############################# Features ############################
features:
  enable: true
  title: "Fonctionnalités GroupDocs.Signature"
  description: "Signature de PDF, de documents Office et d'images avec des signatures numériques"

  items:
    # feature loop
    - icon: "sign"
      title: "Ajout de signatures"
      content: "Signez un document à l'aide de différents types de signature pris en charge en plaçant une signature numérique précisément à n'importe quel endroit de n'importe quelle page."

    # feature loop
    - icon: "custom"
      title: "Personnalisation des résultats"
      content: "Personnalisez l'apparence de la signature en ajustant la couleur, la police, la bordure, la rotation et d'autres fonctionnalités pour obtenir le résultat souhaité."

    # feature loop
    - icon: "password"
      title: "Sécurisation des documents avec mot de passe"
      content: "Pour de nombreux types de documents pris en charge, vous pouvez protéger le document signé avec un mot de passe."

    # feature loop
    - icon: "protect"
      title: "Empêcher les modifications non autorisées"
      content: "Protégez les documents commerciaux importants signés avec un certificat numérique contre les modifications non autorisées."

    # feature loop
    - icon: "convert"
      title: "Obtention des résultats dans les formats souhaités"
      content: "Obtenez facilement des fichiers de résultats signés dans n’importe quel format pris en charge. Vous pouvez également convertir des documents MS Word en PDF sans effort."

    # feature loop
    - icon: "preview"
      title: "Aperçu du document"
      content: "Enregistrez n'importe quelle page d'un document sous forme d'image pour un traitement ultérieur."

    # feature loop
    - icon: "search"
      title: "Recherche de signatures"
      content: "Il est possible d'obtenir des informations sur les signatures précédemment ajoutées dans des documents spécifiques."

    # feature loop
    - icon: "validate"
      title: "Validation des documents"
      content: "Validez l’exactitude des signatures sur tout document signé."

    # feature loop
    - icon: "update"
      title: "Gestion des signatures"
      content: "Une fois qu'une signature est placée sur une page de document, elle peut être supprimée, déplacée ou mise à jour selon les besoins."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de codes"
  description: "Quelques cas d'utilisation d'opérations GroupDocs.Signature typiques pour Java"
  items:
    # code sample loop
    - title: "Améliorez le document PDF avec le code QR"
      content: |
        L'amélioration des processus métier en ajoutant des [codes QR](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) à des pages spécifiques de documents PDF peut s'avérer utile. Il existe un exemple de la façon d'ajouter un code QR à l'aide de GroupDocs.Signature pour Java.
        {{< landing/code title="Améliorez le document PDF avec le code QR">}}
        ```java {style=abap}
        // Chargez le document à signer
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Créer des options de code QR avec du texte prédéfini
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configurer le type d'encodage du code QR et la position sur la page
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Signez le document et enregistrez-le comme fichier de résultat
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Utiliser la signature numérique pour protéger un DOCX"
      content: |
        Vous pouvez [Protéger un document](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) en utilisant des signatures personnelles ou d'entreprise stockées sous forme de certificats numériques. Les documents sécurisés par un certificat ne peuvent être modifiés sans invalider la signature.
        {{< landing/code title="Utiliser la signature numérique pour protéger un DOCX">}}
        ```java {style=abap}   
        // Charger le document à signer numériquement
        Signature signature = new Signature("file_to_sign.docx");
        
        // Spécifiez les options de signature numérique et fournissez le chemin d'accès au fichier de certificat
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Définir le mot de passe du certificat
        options.setPassword("1234567890");

        // Signez le document et enregistrez-le dans le chemin souhaité
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---