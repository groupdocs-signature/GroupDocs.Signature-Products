---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API de signature numérique Java, ajouter une signature électronique à une image PDF Word Excel"
head_description: "API de signature numérique Java. Bibliothèque de signatures électroniques pour signer numériquement des PDF, Microsoft Word, des feuilles de calcul Excel, des présentations PowerPoint et des formats de documents image."

############################# Header ############################
title: "API Java pour gérer les signatures numériques"
description: "Gérez la signature électronique des types d'image, de code QR, de code-barres, de métadonnées, de texte et de tampon dans les applications Java pour la signature d'images et de formats de fichiers de documents numériques."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Aperçu"

            # button loop
            - link: "#features"
              text: "Caractéristiques"

            # button loop
            - link: "#support"
              text: "Soutien"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Démo en direct"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Tarification"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      L'API GroupDocs.Signature pour Java vous aide à développer des applications Java avec des fonctionnalités de signatures électroniques pour signer des documents numériques aux formats pris en charge sans installer de logiciel externe. Il prend en charge la manipulation et la gestion de divers types de signatures électroniques telles que l'image, le code-barres, le code QR, le tampon, le texte, l'optique et les métadonnées. Tous vos documents commerciaux électroniques tels que Microsoft Office Word, les présentations PowerPoint, les feuilles de calcul Excel, les images et les fichiers PDF peuvent être signés numériquement en personnalisant les propriétés de signature, par ex. ombre, dimensions, alignement et plus selon vos besoins. La bibliothèque de signature numérique est simple et légère, consistant en un seul fichier DLL qui peut être facilement intégré dans une application Java nouvelle ou existante.  

      Grâce à l'API GroupDocs.Signature pour Java, vous pouvez charger tous les certificats enregistrés à partir du système ou localiser les signatures existantes à l'aide d'une recherche simple et avancée. Les options pour travailler avec des documents protégés par mot de passe, en spécifiant les propriétés de signature communes (taille du texte, opacité, rotation, vérification, propriétés de la police, options de couleur, numéro de page, largeur, haut, gauche, etc.) et la prise en charge de la mise en œuvre de différents types de signature électronique en font un outil fiable. Solution de gestion des signatures électroniques pour les documents numériques.  

      GroupDocs.Signature pour Java est compatible avec toutes les versions de Java et prend en charge les systèmes d'exploitation courants (Windows, Linux, MacOS) capables d'exécuter Java Runtime
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Voici un aperçu des fonctionnalités de GroupDocs.Signature pour Java :
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Types de signatures"
          content: |
            * Signature de texte
            * Signature d'image
            * Signatures numériques
            * Signature du code QR
            * Signature du code-barres
            * Cachet Signature
            * Formulaire-champ Signature
      
      ## TAB TWO ##
      tab_two:
        description: |
          L'API de signature électronique Java prend en charge les [formats de fichier de document](https://docs.groupdocs.com/signature/java/supported-document-formats/) comme indiqué ci-dessous.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Other Formats"
              content: |
                * **Images**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Métafichiers**: EMF, WMF, CMX
                * **Portable**: PDF
                * **Image Vectorielle**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Autres**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature pour Java prend en charge les systèmes d'exploitation, frameworks et gestionnaires de packages suivants :
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Systèmes d'exploitation"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Cadres pris en charge"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Environnements de développement"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Outil d'automatisation de construction"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature pour les fonctionnalités Java"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Créer, lire, modifier, masquer et supprimer des signatures électroniques à partir de formats de documents pris en charge"

      # feature loop
      - icon: "fas fa-eye"
        content: "Accès au document signé à partir du flux, du chemin relatif ou du chemin absolu"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Appliquer la signature de texte aux documents, feuilles de calcul, présentations, images et fichiers PDF"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Ajouter une signature de texte comme annotation, autocollant, image aux fichiers PDF également configurer le style et la couleur"

      # feature loop
      - icon: "fas fa-code"
        content: "Signez un document PDF, un fichier image et obtenez une sortie dans un format de fichier différent"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Signez numériquement des images avec une signature textuelle en filigrane et ajoutez de la transparence, une rotation à la signature électronique"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Rechercher des certificats et signer des documents Microsoft Word, Excel et PDF avec des certificats numériques"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Signer les formats de documents de traitement de texte avec des filigranes de texte natifs"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Utilisez le code QR, le code-barres pour signer des fichiers Word, Slide, Cell, PDF et Image"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Configurer et appliquer des signatures de tampon pour sécuriser les formats de fichiers pris en charge"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Configurer et attribuer des signatures d'image aux documents, feuilles de calcul, présentations, images et fichiers PDF"

      # feature loop
      - icon: "fas fa-columns"
        content: "Configurez les propriétés de la signature, par exemple, l'aspect et la convivialité, les marges, l'alignement, etc."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Appliquer la signature numérique au document protégé par mot de passe"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Effectuer la vérification du texte des documents PDF à l'aide du gestionnaire de signature"

      # feature loop
      - icon: "fas fa-print"
        content: "Vérification numérique de documents Word, cellulaires et PDF avec des conteneurs de certificats .CER et .PFX"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Spécifiez différents types d'unités de mesure (par exemple, millimètres, pixels, etc.) pour les signatures de texte PDF"

      # feature loop
      - icon: "fas fa-lock"
        content: "Obtenir des informations sur le document via un fichier ou une URL - Ajouter des signatures de champ de formulaire aux documents PDF"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Ajouter un objet de données personnalisé, une VCard intégrée, un e-mail, un EPC, une MeCard ou un objet d'événement au code QR"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Appliquer différents styles de pinceaux aux signatures, par exemple, pinceau dégradé, radial, solide et texture"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Signer le document situé sur FTP ou Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Définir l'alignement du texte dans les formes pour les documents, les diapositives, les images et les fichiers PDF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Rechercher, vérifier et signer numériquement des documents de présentation PowerPoint"

      # feature loop
      - icon: "fas fa-cube"
        content: "Placer la signature à l'aide de pixels dans les documents cellulaires et le positionnement du texte pour les signatures de tampon"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Mettre en œuvre une signature de tampon rectangulaire avec des coins arrondis"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Étendez les signatures de codes-barres et de codes QR avec le contenu des données d'image"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Ajouter des signatures de métadonnées cryptées tout en travaillant avec les options de signature et de recherche"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Intégrez des objets personnalisés aux signatures de métadonnées dans Word, Excel et les présentations"

    more_feature:
      # more_feature_loop
      - title: "Configurez et appliquez facilement des signatures électroniques"
        content: |
          L'API GroupDocs.Signature pour Java permet de configurer et d'ajouter des signatures électroniques aux formats de document pris en charge. Voici un exemple de code qui montre à quel point il est simple d'appliquer une signature de texte à un fichier PDF :

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // définir la position de la signature
          options.setLeft(100);
          options.setTop(100);
          
          // définir un rectangle de signature
          options.setWidth(100);
          options.setHeight(30);

          // définir la couleur et la police du texte
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // signer le document à classer
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Types d'encodage de code-barres pris en charge pour la signature électronique"
        content: |
          À l'aide de GroupDocs.Signature pour l'API Java, vous pouvez appliquer des signatures de code-barres et de code QR aux formats de fichiers pris en charge. GroupDocs.Signature pour Java prend en charge une vaste gamme de types d'encodage de codes-barres pour répondre à la plupart des exigences. Les types d'encodage de code-barres pris en charge incluent, Code 11, Code 128, Code 16K/32, Codes Databar, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard et Code39 étendu.

          De même, l'API GroupDocs.Signature pour Java vous permet d'utiliser des types de code QR, tels que QR, Aztec et Data Matrix. Les types d'encodage QR-Code pris en charge incluent Aztec, DataMatrix, GS1 DataMatrix et GS1 QR.

      # more_feature_loop
      - title: "Rechercher des signatures et des certificats"
        content: |
          Grâce à l'API GroupDocs.Signature pour Java, vous pouvez rechercher des signatures QR-Code et Barcode dans n'importe quel document, présentation, feuille de calcul, image, ainsi que dans un fichier PDF, et récupérer le résultat de la recherche. Vous pouvez également rechercher un objet de données personnalisé à partir de documents signés avec une signature QR-Code ainsi que rechercher une carte virtuelle standard et un objet de courrier électronique à partir de documents signés avec un code QR. La vérification du texte crypté des signatures QR-Code ainsi que la recherche de signature de métadonnées dans les documents PDF sont également prises en charge. Appliquer des critères de recherche supplémentaires pour les signatures numériques des documents Words & Cells.  

          L'option de recherche est également disponible pour la signature des métadonnées pour les documents Word, les diapositives et les feuilles de calcul, tandis que la recherche par champ de formulaire est disponible pour les documents PDF.

      # more_feature_loop
      - title: "Configurer les propriétés de signature électronique"
        content: |
          Pour améliorer l'expérience utilisateur des utilisateurs finaux, l'API GroupDocs.Signature pour Java fournit de nombreuses propriétés qui peuvent être configurées assez facilement. Vous pouvez définir les options de police et de couleur (couleur d'arrière-plan, couleur de premier plan, gras, italique, souligné, famille de police, taille de police, etc.), les options d'arrière-plan et de bordure (couleur d'arrière-plan, transparence d'arrière-plan, couleur de bordure, style de tiret de bordure, épaisseur de bordure, Transparence des bordures, etc.), marges de signature (gauche, haut, largeur, hauteur, remplissage, etc.) et configuration de la zone de signature de l'image et de l'alignement de la signature (alignement horizontal, alignement vertical, etc.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature propose des API de visualisation de documents pour d'autres environnements de développement populaires"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---