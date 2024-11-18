



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:56
draft: false
lang: fr
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Ajouter des signatures texte à JPEG via JavaScript"
head_description: "Utilisez l'API JavaScript pour intégrer sans effort des signatures texte dans des documents JPEG. Notre API prend en charge un large éventail de formats, y compris PDF, Word, Excel, Présentations, Images et fichiers ZIP."

############################# Header ############################
title: "Ajouter des signatures texte à JPEG" 
description: "Incorporez des signatures texte personnalisées dans vos fichiers professionnels avec GroupDocs.Signature for Node.js via Java. Prenez le contrôle de vos flux de documents en les améliorant avec des options de signature sécurisées et personnalisables."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Commencer l'essai gratuit"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Présentation de GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) est une solution innovante conçue pour faciliter l'ajout de signatures texte dans les documents. Personnalisez et placez des signatures sur n'importe quelle page, améliorant ainsi l'efficacité de la gestion des documents. Optimisez les flux de travail de votre organisation en intégrant des marques textuelles personnalisées qui améliorent la fonctionnalité et le professionnalisme.

############################# Steps ############################
steps:
    enable: true
    title: "Guide pour créer des signatures texte pour JPEG en utilisant JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) permet l'ajout de signatures texte dans les documents JPEG au sein des applications Node.js via Java. Améliorez rapidement les capacités de votre produit avec nos solutions robustes.
      
      1. Fournissez le document JPEG en tant qu'argument à la classe Signature.
      2. Instanciez TextSignOptions avec le texte requis.
      3. Définissez les propriétés visuelles de la signature texte.
      4. Ajoutez la signature texte aux pages souhaitées du document.
   
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

        // Initialisez la classe Signature avec le chemin du document
        const signature = new signatureLib.Signature('input.jpeg');

        // Créez TextSignOptions avec le texte de signature requis
        const options = new signatureLib.TextSignOptions('Approved');

        // Configurez la couleur et les propriétés de police du texte
        options.setForeColor(new signatureLib.Color(255, 0, 0));
        const signatureFont = new signatureLib.SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName('Comic Sans MS');
        options.setFont(signatureFont);
        
        // Ajoutez la signature texte au document
        const result = signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Contrôle amélioré des signatures texte"
  description: "Avec GroupDocs.Signature for Node.js via Java, vous pouvez considérablement améliorer la gestion des signatures basées sur du texte dans les formats de documents clés. L'outil vous permet de configurer le style, l'emplacement et le contenu des signatures, permettant aux entreprises d'adapter leurs processus documentaires."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Fonctionnalités principales de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Signatures documents dynamiques"
      content: "Insérez divers types de signatures—telles que texte, images, codes-barres, codes QR ou tampons—sur n'importe quelle page des documents pris en charge. Intégrez des métadonnées pour transporter des informations cachées ou appliquez des certificats numériques pour des mesures de sécurité avancées."

    # feature loop
    - title: "Recherche et validation des signatures"
      content: "Vérifiez l'authenticité des signatures intégrées dans vos documents. Effectuez des recherches efficaces pour localiser toutes les instances de signature, garantissant un suivi et une gestion approfondis des documents."

    # feature loop
    - title: "Modifier ou supprimer des signatures"
      content: "Modifiez ou supprimez les signatures ajoutées précédemment selon vos besoins. Vous pouvez ajuster l'apparence, la position ou le contenu de toute signature pour répondre aux exigences évolutives, assurant ainsi une flexibilité dans la gestion des documents."

    # feature loop
    - title: "Personnalisation des signatures natives"
      content: "Pour certains types de fichiers, personnalisez le placement des signatures avec des fonctionnalités documentaires intégrées, telles que l'ajout de filigranes dans des fichiers Word ou de tampons personnalisés dans des fichiers PDF, augmentant l'unicité de vos documents."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Implémenter des signatures texte dans les documents"
      content: |
        Découvrez comment intégrer des signatures texte dans des documents professionnels pour optimiser les processus.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Choisissez le document à signer
          const signature = new signatureLib.Signature('input.jpeg');

          // Définissez les options de texte avec le contenu spécifié
          const options = new signatureLib.TextSignOptions('Rescheduled to 03/04/2025');

          // Définissez la taille et la position de la signature sur la page
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
          options.setHeight(30);

          // Appliquez un rembourrage pour la signature par rapport aux bords de la page
          const padding = new signatureLib.Padding();
          padding.setBottom(20);
          padding.setRight(20);
          options.setMargin(padding);

          // Personnalisez la couleur du texte et le style de police
          options.setForeColor(signatureLib.Color.RED);
          const signatureFont = new signatureLib.SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName('Comic Sans MS');
          options.setFont(signatureFont);

          // Ajoutez une bordure à la signature texte si désiré
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // Configurez l'arrière-plan de la signature
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // Optionnellement, enregistrez le texte en tant qu'image pour la compatibilité
          options.setSignatureImplementation(signatureLib.TextSignatureImplementation.Image);
          
          // Enregistrez le document avec la signature texte ajoutée
          const result = signature.sign('output.jpeg', options);
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
            link: "/examples/signature/formats/signature_text.jpeg"
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
    title: "Fonctionnalités complètes de gestion des signatures"
    exclude: "text"
    description: "Notre plateforme offre des opérations CRUD complètes et des fonctionnalités avancées pour la gestion de sept types de signatures distincts, vous permettant de gérer vos signatures documentaires avec précision et aisance."
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
    title: "Appliquer des signatures texte dans divers formats"
    exclude: "JPEG"
    description: "Exploitez les capacités de l'API Node.js via Java pour intégrer des signatures basées sur du texte dans un large éventail de formats Office. Contrôlez le flux d'informations à chaque étape du cycle de vie de votre document en ajoutant des marques textuelles hautement personnalisables."
    items: 
          
        # format loop 1
        - name: "Signatures textuelles PDF"
          format: "PDF"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Signatures textuelles DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/text/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 3
        - name: "Signatures textuelles JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "Image JPEG"
          
        # format loop 4
        - name: "Signatures textuelles PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/text/pptx/"
          description: "Présentation Open XML de PowerPoint"
          
        # format loop 5
        - name: "Signatures textuelles XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"


          

---