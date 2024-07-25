---
############################# Static ############################
layout: "landing"
date: 2024-07-25T14:25:12
draft: false

lang: fr
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
head_title: "API de signatures numériques C# .NET - GroupDocs.Signature"
head_description: "Intégrez le traitement des signatures numériques dans vos applications .NET à l'aide de GroupDocs.Signature. Sécurisez vos fichiers avec des signatures rapidement et efficacement."

############################# Header ############################
title: "Signer des documents via l'API .NET"
description: "Signez des documents et des images numériques sur n'importe quelle plate-forme à l'aide de nos API flexibles et de nos solutions basées sur des applications pour les programmeurs et les utilisateurs finaux."
words:
  for: "pour"

actions:
  main: "Téléchargement gratuit de NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licence"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net/"
  title: "Prêt à commencer?"
  description: "Essayez les fonctionnalités de GroupDocs.Signature gratuitement ou demandez une licence"

release:
  title: "Version {0} publiée"
  notes: "Regardez ce qu'il y a de nouveau"
  downloads: "Téléchargements"

code:
  title: "Signer des fichiers PDF en C#"
  more: "Plus d'exemples"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Sélectionnez un document PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Fournir du texte
        var options = new TextSignOptions("John Smith")
        {
            // Définir la couleur
            ForeColor = Color.Red
        };
        // Signer le document et l'enregistrer dans un fichier
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Présentation de GroupDocs.Signature"
  description: "API pour effectuer la signature de documents et les opérations associées dans les applications .NET"
  features:
    # feature loop
    - title: "Ajout de signatures aux documents commerciaux en C#"
      content: "Signature de documents : avec GroupDocs.Signature pour .NET, vous pouvez ajouter différents types de signatures, telles que du texte, des images, des codes-barres et des certificats numériques, aux documents PDF et Office. Cette API vous permet de signer vos documents avec presque n'importe quel type de données, y compris les métadonnées cachées."

    # feature loop
    - title: "Traitement des documents signés"
      content: "Traitement supplémentaire : vous pouvez effectuer des opérations puissantes sur des documents signés à l'aide de GroupDocs.Signature. Cela inclut la recherche de signatures existantes dans les documents commerciaux et leur vérification à l'aide de critères spécifiques. De plus, vous pouvez récupérer des informations sur le document et prévisualiser les pages via cette API .NET."

    # feature loop
    - title: "Personnalisation des résultats"
      content: "GroupDocs.Signature pour .NET offre des options de personnalisation étendues. Vous pouvez positionner avec précision les signatures n'importe où sur une page de document et ajuster leur apparence à l'aide de divers paramètres. De plus, cette API prend en charge l'enregistrement des documents traités dans un large éventail de formats pris en charge."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Signature pour .NET prend en charge les systèmes d'exploitation, frameworks et gestionnaires de packages suivants"
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
  title: "Formats de fichiers pris en charge"
  description: |
    GroupDocs.Signature pour .NET prend en charge les opérations avec les [formats de fichiers](https://docs.groupdocs.com/signature/net/supported-document-formats/) suivants.
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
  description: "Signature rapide et précise de PDF, de documents Office et d'images"

  items:
    # feature loop
    - icon: "sign"
      title: "Signature de documents"
      content: "Ajoutez avec précision un ou plusieurs types de signatures pris en charge à n’importe quelle position spécifiée sur les documents commerciaux."

    # feature loop
    - icon: "custom"
      title: "Personnaliser les signatures"
      content: "Utilisez des fonctionnalités telles que la couleur, la police, la bordure, la rotation, etc., pour configurer l'apparence des signatures."

    # feature loop
    - icon: "password"
      title: "Protection par mot de passe des documents"
      content: "Sécurisez certains types de documents en définissant un mot de passe après la signature."

    # feature loop
    - icon: "protect"
      title: "Protection contre les changements"
      content: "Empêchez les modifications apportées aux documents commerciaux importants après avoir apposé une signature avec un certificat numérique."

    # feature loop
    - icon: "convert"
      title: "Convertir les fichiers signés vers d'autres formats"
      content: "Convertissez les fichiers signés aux formats souhaités, par exemple en enregistrant un document Word au format PDF."

    # feature loop
    - icon: "preview"
      title: "Extraire les aperçus des pages"
      content: "Extrayez les pages des documents signés sous forme d’images individuelles pour un traitement ultérieur."

    # feature loop
    - icon: "search"
      title: "Recherche de signature dans les documents"
      content: "Récupérez des informations sur les signatures précédemment ajoutées dans des documents spécifiques."

    # feature loop
    - icon: "validate"
      title: "Valider les documents signés"
      content: "Vérifiez la bonne signature des documents à l’aide des fonctionnalités de validation."

    # feature loop
    - icon: "update"
      title: "Mettre à jour ou supprimer des signatures"
      content: "Repositionnez facilement des signatures spécifiques sur une page, modifiez leur texte ou supprimez-les sans aucun problème."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de codes"
  description: "Quelques cas d'utilisation d'opérations GroupDocs.Signature typiques pour .NET"
  items:
    # code sample loop
    - title: "Ajouter un code QR au PDF"
      content: |
        L'ajout de [QR-codes](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) à des pages spécifiques de documents PDF peut améliorer les processus métier. Vous trouverez ci-dessous un exemple de la façon d'ajouter un code QR à l'aide de GroupDocs.Signature.
        {{< landing/code title="Comment mettre le code QR au format PDF.">}}
        ```csharp {style=abap}
        // Chargez le document à signer
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Créer des options de code QR avec du texte prédéfini
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Configurer le type d'encodage du code QR et la position sur la page
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Signez le document et enregistrez-le comme fichier de résultat
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Protéger un document DOCX à l'aide d'un certificat numérique"
      content: |
        Vous pouvez [Protéger un document](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) en utilisant des signatures personnelles ou d'entreprise stockées sous forme de certificats numériques. Ces documents protégés ne peuvent être modifiés sans invalider la signature.
        {{< landing/code title="Voici comment garantir l’intégrité des documents.">}}
        ```csharp {style=abap}   
        // Charger le document à signer numériquement
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // Spécifiez les options de signature numérique et fournissez le chemin d'accès au fichier de certificat
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Définir le mot de passe du certificat
                Password = "1234567890"
            };
            // Signez le document et enregistrez-le dans le chemin souhaité
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---