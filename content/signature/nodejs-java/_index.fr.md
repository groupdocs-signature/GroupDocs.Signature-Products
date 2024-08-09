---
############################# Static ############################
layout: "landing"
date: 2024-07-25T14:25:12
draft: false

lang: fr
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
head_title: "API de signature numérique Node.js - GroupDocs.Signature"
head_description: "Intégrez des signatures électroniques sécurisées dans les applications Node.js avec GroupDocs.Signature. Rationalisez les flux de signature de documents de manière simple et efficace."

############################# Header ############################
title: "Signer des documents avec l'API Node.js"
description: "Signez des documents et des images numériques sur n'importe quelle plate-forme à l'aide de nos API flexibles et de nos solutions basées sur des applications pour les programmeurs et les utilisateurs finaux."
words:
  for: "pour"

actions:
  main: "Télécharger depuis NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licence"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
  title: "Prêt à commencer?"
  description: "Essayez les fonctionnalités de GroupDocs.Signature gratuitement ou demandez une licence"

release:
  title: "Version {0} publiée"
  notes: "Regardez ce qu'il y a de nouveau"
  downloads: "Téléchargements"

code:
  title: "Signature de PDF par Node.js"
  more: "Plus d'exemples"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Sélectionnez un document PDF
    let signature = new Signature("sample.pdf");
    
    // Fournir du texte
    let options = new TextSignOptions("John Smith");
    
    // Définir la couleur
    options.ForeColor = Color.Red;
    
    // Signer le document et l'enregistrer dans un fichier
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Présentation de GroupDocs.Signature"
  description: "Bibliothèque de signature de documents prête à être utilisée dans les applications Node.js"
  features:
    # feature loop
    - title: "Solution de signatures numériques pour les documents commerciaux avec Node.js"
      content: "GroupDocs.Signature for Node.js via Java propose un ensemble complet d'options de signature numérique pour les documents PDF, Office et les images. Texte, codes-barres, images, certificats numériques et métadonnées sont disponibles. Le traitement rationalisé des documents garantit l’efficacité."

    # feature loop
    - title: "Manipulation avancée des documents signés"
      content: "GroupDocs.Signature vous permet de traiter les documents signés. Recherchez et validez les signatures selon divers critères. De plus, extrayez des informations détaillées sur le document ou générez des images d’aperçu des pages."

    # feature loop
    - title: "Divers formats de sortie"
      content: "Notre solution offre un contrôle étendu sur le format de sortie des documents signés. Positionnez avec précision les signatures sur n'importe quelle page et personnalisez leur apparence. Enregistrez les documents signés dans de nombreux formats pris en charge et sécurisez-les éventuellement avec des mots de passe."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Signature for Node.js via Java effectue le traitement des documents avec différents systèmes d'exploitation"
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
    GroupDocs.Signature for Node.js via Java facilite les opérations pour les [formats de fichiers populaires](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "Fonctionnalités de GroupDocs.Signature"
  description: "Signez des PDF, des documents Office et des images avec des signatures numériques"

  items:
    # feature loop
    - icon: "sign"
      title: "Signature d'entreprise"
      content: "Utilisez différents types de signature pour signer des documents. Placez des signatures numériques précisément à n’importe quel emplacement de page."

    # feature loop
    - icon: "custom"
      title: "Personnalisation de l'apparence de la signature"
      content: "Adaptez les aspects visuels des signatures en ajustant la couleur, la police, les bordures, la rotation, etc. pour obtenir le résultat souhaité."

    # feature loop
    - icon: "password"
      title: "Documents protégés par mot de passe"
      content: "Pour de nombreux formats de documents pris en charge, protégez les documents signés avec un mot de passe pour plus de sécurité."

    # feature loop
    - icon: "protect"
      title: "Prévenir les modifications non autorisées"
      content: "Protégez les documents commerciaux cruciaux signés avec des certificats numériques contre les modifications non autorisées."

    # feature loop
    - icon: "convert"
      title: "Formats de sortie souhaités"
      content: "Obtenez sans effort des documents signés dans n’importe quel format pris en charge. Convertissez facilement des documents MS Word au format PDF."

    # feature loop
    - icon: "preview"
      title: "Aperçu des documents"
      content: "Enregistrez des pages de document individuelles sous forme d’images pour vos besoins futurs."

    # feature loop
    - icon: "search"
      title: "Recherche de signatures"
      content: "Récupérez des informations sur les signatures précédemment ajoutées dans vos documents."

    # feature loop
    - icon: "validate"
      title: "Validation des documents"
      content: "Vérifier l'authenticité des signatures présentées dans tout document."

    # feature loop
    - icon: "update"
      title: "Gestion des signatures"
      content: "Supprimez, déplacez ou modifiez toutes les signatures placées sur n'importe quelle page de document."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de codes"
  description: "Exemples illustrant les opérations GroupDocs.Signature for Node.js via Java typiques"
  items:
    # code sample loop
    - title: "Marquer un PDF avec des codes QR"
      content: |
        L'intégration de [codes-barres](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) dans des pages de documents PDF spécifiques peut rationaliser les processus métier. Cette section fournit un exemple d'ajout d'un code QR à l'aide de GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Comment mettre le code QR au format PDF.">}}
        ```javascript {style=abap}
        // Chargez le document à signer
        let signature = new Signature("file_to_sign.pdf");
        
        // Créer des options de code QR avec du texte prédéfini
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configurer le type d'encodage du code QR et la position sur la page
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Signez le document et enregistrez-le comme fichier de résultat
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Protéger un DOCX avec une signature numérique"
      content: |
        [Protégez vos documents](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) par des signatures basées sur des certificats numériques. La signature numérique protège vos documents professionnels contre les modifications de contenu.
        {{< landing/code title="Voici comment garantir l’intégrité des documents.">}}
        ```javascript {style=abap}   
        // Charger le document à signer numériquement
        let signature = new Signature("file_to_sign.docx");
        
        // Spécifiez les options de signature numérique et fournissez le chemin d'accès au fichier de certificat
        let options = new DigitalSignOptions("certificate.pfx");

        // Définir le mot de passe du certificat
        options.Password = "1234567890";

        // Signez le document et enregistrez-le dans le chemin souhaité
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
