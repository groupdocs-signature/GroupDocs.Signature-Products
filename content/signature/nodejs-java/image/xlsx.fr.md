



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:10
draft: false
lang: fr
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Ajout de signatures d'image au fichier XLSX avec JavaScript"
head_description: "Insérez une signature d'image sur le fichier XLSX pour Node.js en quelques lignes de code. Utilisez l'API GroupDocs.Signature for Node.js via Java pour ajouter des images."

############################# Header ############################
title: "Signer des fichiers XLSX avec des signatures d'image" 
description: "Tirez parti des capacités de GroupDocs.Signature for Node.js via Java pour intégrer des images dans une multitude de formats de documents bureautiques tels que PDF, Word, Excel et divers fichiers image. Ajouter une image de signature peut considérablement améliorer le professionnalisme et la crédibilité de vos documents, créant ainsi une présentation raffinée et soignée."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger gratuitement"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Présentation de GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) permet aux utilisateurs d'incorporer des signatures d'image à n'importe quel endroit de vos documents. Cet outil permet aux entreprises d'optimiser leurs flux de travail en ajoutant des images à des fichiers PDF, Word, Excel, PowerPoint et à des formats d'image populaires, améliorant ainsi l'efficacité de la gestion des documents.

############################# Steps ############################
steps:
    enable: true
    title: "Guide pour ajouter des images dans XLSX avec JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) permet aux applications Node.js via Java d'intégrer parfaitement des signatures d'image dans des documents XLSX. Améliorez les capacités de votre application avec notre bibliothèque complète.
      
      1. Instanciez Signature avec le document XLSX
      2. Utilisez ImageSignOptions pour spécifier l'image de signature
      3. Positionnez précisément l'image sur n'importe quelle page
      4. Enregistrez le document signé à l'emplacement souhaité
   
    code:
      platform: "nodejs-java"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Signatures d'exemple"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // Initialisez Signature avec le chemin du document
        const signature = new signatureLib.Signature('input.xlsx');

        // Configurez ImageSignOptions pour inclure la signature d'image souhaitée
        const options = new signatureLib.ImageSignOptions('company_logo.jpg');

        // Placez l'image en haut à gauche sur toutes les pages
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);
        
        // Enregistrez le document avec la signature d'image appliquée
        const result = signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Fonctionnalités avancées de signature de documents"
  description: "Notre API propose un ensemble de fonctionnalités qui simplifient la signature électronique. Vous pouvez ajouter, modifier, supprimer, rechercher et vérifier plusieurs types de signatures, y compris les signatures d'image, sans difficulté."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Signatures d'image"
  features:
    # feature loop
    - title: "Intégrer des images dans des documents bureautiques"
      content: "Insérez des signatures d'image n'importe où dans votre document, que ce soit dans des fichiers PDF, Word ou Excel. Améliorez vos documents en ajoutant des images, des codes-barres, des métadonnées ou des certificats numériques pour des fonctionnalités supplémentaires."

    # feature loop
    - title: "Rechercher et valider des signatures"
      content: "Assurez l'authenticité de vos documents signés en vérifiant les signatures. Utilisez la fonctionnalité de recherche pour extraire et examiner toutes les signatures intégrées dans votre document."

    # feature loop
    - title: "Modifier les signatures existantes"
      content: "Notre API permet aux utilisateurs de mettre à jour et d'ajuster les signatures selon leurs besoins. Modifiez la taille, la position ou d'autres attributs de toute signature précédemment ajoutée pour plus de flexibilité dans la gestion des documents."

    # feature loop
    - title: "Supprimer les signatures inutiles"
      content: "Gérez efficacement vos documents en supprimant les signatures qui ne sont plus nécessaires. Notre API prend en charge des opérations CRUD complètes pour presque tous les types de signatures."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Améliorez les documents avec des signatures d'image"
      content: |
        Apprenez à intégrer des images dans des documents professionnels pour ajouter des informations complémentaires.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Sélectionnez le document à signer
          const signature = new signatureLib.Signature('input.xlsx');

          // Configurez les options d'image avec le chemin de l'image
          const options = new signatureLib.ImageSignOptions('manager_signature.jpg');

          // Ajustez la taille de la signature d'image
          options.setWidth(100);
          options.setHeight(100);

          // Placez l'image en bas à droite
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Appliquez un espacement des coins de la page si nécessaire
          const padding = new signatureLib.Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // Optionnellement, ajoutez une bordure personnalisée à l'image
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // Faites pivoter la signature d'image pour une apparence optimale
          options.setRotationAngle(45);

          // Enregistrez le document mis à jour à l'emplacement souhaité
          const result = signature.sign('output.xlsx', options);
          ```
        platform: "nodejs-java"
        copy_title: "Copier"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "cliquez pour copier"
          copy_done: "copié"
        top_links:
          #  loop
          - title: "Télécharger le résultat"
            icon: "download"
            link: "/examples/signature/formats/signature_image.xlsx"
        links:
          #  loop
          - title: "Plus d'exemples"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Prêt à commencer ?"
  description: "Essayez les fonctionnalités de GroupDocs.Signature gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "Téléchargement NPM"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Découvrez les fonctions que nous proposons"
    exclude: "image"
    description: "Nous sommes fiers de présenter une large sélection de méthodes et d'opérations de signature"
    items: 
          
        # operation loop 1
        - name: "Signatures électroniques"
          operation: "esign"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "Ajoutez différents types de signatures aux formats de fichier pris en charge"

        # operation loop 2
        - name: "Ajouter du texte aux documents"
          operation: "text"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Améliorez le contenu du document avec des signatures textuelles personnalisables"

        # operation loop 3
        - name: "Signatures d'image"
          operation: "image"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Placez n'importe quelle image à n'importe quelle position dans un document"

        # operation loop 4
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "Créez et insérez divers codes-barres dans les documents pris en charge"

        # operation loop 5
        - name: "Générer des QR codes"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Générez des QR Codes, y compris des codes QR, pour la signature de documents"
          
        # operation loop 6
        - name: "Certificats numériques"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Sécurisez les affaires et signez des documents avec des certificats numériques"

        # operation loop 7
        - name: "Tampons"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "Utilisez le constructeur de tampons pour créer des tampons ronds ou carrés personnalisés"
          
        # operation loop 8
        - name: "Rechercher des signatures"
          operation: "search"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "Trouvez toutes les signatures précédemment ajoutées dans un document"
          
        # operation loop 9
        - name: "Vérification des signatures"
          operation: "verify"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "Vérifiez l'authenticité des signatures après qu'elles aient été appliquées"
          
        # operation loop 10
        - name: "Modifier les signatures"
          operation: "modify"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "Modifiez facilement une variété de signatures dans un document"
          
        # operation loop 11
        - name: "Supprimer les signatures"
          operation: "delete"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "Retirez une large gamme de signatures précédemment appliquées"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Ajouter des images à divers types de fichiers"
    exclude: "XLSX"
    description: "L'API Node.js via Java vous permet d'incorporer des images dans une large gamme de formats de documents. Personnalisez la taille, le placement et la position sur la page pour améliorer votre processus de signature de documents."
    items: 
          
        # format loop 1
        - name: "Signer PDF avec une image"
          format: "PDF"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Signer DOCX avec une image"
          format: "DOCX"
          link: "/signature/nodejs-java/image/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 3
        - name: "Signer JPEG avec une image"
          format: "JPEG"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "Image JPEG"
          
        # format loop 4
        - name: "Signer PPTX avec une image"
          format: "PPTX"
          link: "/signature/nodejs-java/image/pptx/"
          description: "Présentation Open XML de PowerPoint"
          
        # format loop 5
        - name: "Signer XLSX avec une image"
          format: "XLSX"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"


          

---