



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:03
draft: false
lang: fr
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Générer des codes QR dans des docs JPEG avec JavaScript"
head_description: "Utilisez l'API GroupDocs.Signature pour créer et intégrer des codes-barres 2D dans des fichiers JPEG. Placez sans effort des codes QR sur n'importe quelle page de document."

############################# Header ############################
title: "Créer des codes QR pour JPEG" 
description: "Créez et intégrez des codes-barres 2D avec un contenu personnalisable, y compris du texte et des données numériques, dans divers types de documents tels que des PDF, Word, Excel et Images avec GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Essayez gratuitement"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Découvrez les capacités de GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) propose des outils avancés d'amélioration de documents, permettant la génération et l'intégration de plusieurs types de signatures, y compris des codes QR, dans des formats de fichiers populaires. Signature et sécurisation de PDF, documents Word, feuilles de calcul Excel, présentations PowerPoint et images avec des signatures de type Texte, Image, Code-barres, Code QR, Métadonnées, Numérique et Cachet.

############################# Steps ############################
steps:
    enable: true
    title: "Guide pour générer et intégrer un code QR à n'importe quel endroit dans un JPEG"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) permet la création de codes QR dans divers formats populaires et leur intégration dans les pages de JPEG. Supportant plus de 10 types distincts de codes QR, notre solution peut être incorporée sans couture dans des applications Node.js via Java, enrichissant celles-ci avec des capacités de signature par code QR.
      
      1. Fournissez le fichier ou le flux JPEG pour la signature du code QR.
      2. Entrez le texte souhaité dans l'instance QrCodeSignOptions.
      3. Ajustez les paramètres visuels tels que la couleur, le positionnement, la taille, etc.
      4. Enregistrez le document contenant le code QR.
   
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

        // Créez une instance Signature et passez le chemin du document
        const signature = new signatureLib.Signature('input.jpeg');

        // Utilisez QrCodeSignOptions pour insérer un code QR dans le document
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // Définissez le type de signature et son emplacement sur la page
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // Enregistrez le document avec le QR code ajouté
        signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Intégration complète des signatures et des codes QR"
  description: "Avec l'API GroupDocs.Signature for Node.js via Java, vous pouvez gérer un large éventail de signatures. Créez, personnalisez, vérifiez, recherchez et supprimez des signatures facilement à travers différents types de documents, offrant une flexibilité inégalée pour vos workflows."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Fonctionnalités de signature et de code QR"
  features:
    # feature loop
    - title: "Signature de documents multi-format"
      content: "Ajoutez plusieurs types de signatures, y compris des signatures de type Texte, Image, Code-barres, Code QR et Cachet, à tout format de document pris en charge. Placez-les sur n'importe quelle page et gérez les métadonnées du document. Assurez la sécurité du document grâce à des certificats numériques pour prévenir les modifications non autorisées."

    # feature loop
    - title: "Validation efficace des signatures"
      content: "Validez toutes les signatures au sein d’un document pour vous assurer qu'elles respectent les normes requises. Récupérez et examinez facilement les signatures grâce à la fonctionnalité de recherche intégrée."

    # feature loop
    - title: "Édition flexible des signatures"
      content: "Mettez à jour ou modifiez les signatures existantes, en ajustant des aspects tels que le contenu, l'emplacement, la taille et la couleur, pour répondre aux besoins de votre document après la signature initiale."

    # feature loop
    - title: "Suppression de signatures simplifiée"
      content: "Supprimez toute signature indésirable ou obsolète, y compris les certificats numériques, facilement. Un contrôle total sur la gestion des signatures garantit un document propre et bien organisé."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Personnalisation d'un code QR généré"
      content: |
        Cet exemple détaille le processus d'ajout d'un code QR personnalisé à une page JPEG.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Obtenez le document à signer et passez-le à Signature.
          const signature = new signatureLib.Signature('input.jpeg');

          // Configurez les options de code QR avec le texte requis.
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // Déterminez la position du code QR sur la page.
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Spécifiez la marge de la signature.
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Choisissez la couleur du code QR.
          signOptions.setForeColor(signatureLib.Color.RED);

          // Définissez les options de police pour le message d'accompagnement.
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Personnalisez la couleur de fond et le pinceau pour le code QR.
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Intégrez le code QR dans le document.
          signature.sign('output.jpeg', signOptions);
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
            link: "/examples/signature/formats/signature_qrcode.jpeg"
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
    title: "Comprendre nos principales capacités"
    exclude: "qrcode"
    description: "Nous offrons une large sélection de formats et opérations de signatures adaptés à vos besoins."
    items: 
          
        # operation loop 1
        - name: "Signatures électroniques"
          operation: "esign"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "Ajoutez différents types de signatures aux formats de fichier pris en charge"

        # operation loop 2
        - name: "Ajouter du texte aux documents"
          operation: "text"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "Améliorez le contenu du document avec des signatures textuelles personnalisables"

        # operation loop 3
        - name: "Signatures d'image"
          operation: "image"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "Placez n'importe quelle image à n'importe quelle position dans un document"

        # operation loop 4
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "Créez et insérez divers codes-barres dans les documents pris en charge"

        # operation loop 5
        - name: "Générer des QR codes"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "Générez des QR Codes, y compris des codes QR, pour la signature de documents"
          
        # operation loop 6
        - name: "Certificats numériques"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Sécurisez les affaires et signez des documents avec des certificats numériques"

        # operation loop 7
        - name: "Tampons"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "Utilisez le constructeur de tampons pour créer des tampons ronds ou carrés personnalisés"
          
        # operation loop 8
        - name: "Rechercher des signatures"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Trouvez toutes les signatures précédemment ajoutées dans un document"
          
        # operation loop 9
        - name: "Vérification des signatures"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Vérifiez l'authenticité des signatures après qu'elles aient été appliquées"
          
        # operation loop 10
        - name: "Modifier les signatures"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "Modifiez facilement une variété de signatures dans un document"
          
        # operation loop 11
        - name: "Supprimer les signatures"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "Retirez une large gamme de signatures précédemment appliquées"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Intégrer des codes QR avec divers formats de fichiers"
    exclude: "JPEG"
    description: "Exploitez l'API Node.js via Java pour générer des codes QR et les intégrer dans une variété de formats de fichiers largement utilisés. Encapsulez des données importantes dans ces codes-barres pour une intégration transparente et une récupération future."
    items: 
          
        # format loop 1
        - name: "QRCode pour PDF"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "QRCode pour DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 3
        - name: "QRCode pour JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "Image JPEG"
          
        # format loop 4
        - name: "QRCode pour PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "Présentation Open XML de PowerPoint"
          
        # format loop 5
        - name: "QRCode pour XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"


          

---