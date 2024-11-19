



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:20
draft: false
lang: fr
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Créer un QR code pour XLSX avec Java"
head_description: "L'API GroupDocs.Signature permet la génération de QR codes pour les fichiers XLSX. Créez des QR codes à partir de votre contenu et placez-les sur n'importe quelle page."

############################# Header ############################
title: "Créer des QR codes pour XLSX" 
description: "Créez des codes-barres 2D avec des données textuelles et numériques et placez-les sur n'importe quelle page de divers documents en utilisant GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Essai gratuit"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "En savoir plus sur GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "En savoir plus"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) offre une large gamme de fonctionnalités pour générer et intégrer différents types de signatures dans tous les principaux formats de documents. Il prend en charge les PDF, les documents Word, les feuilles de calcul Excel, les présentations PowerPoint et les images. Améliorez vos documents avec des signatures de type Texte, Image, Code-barres, QR Code, Métadonnées, Numérique et Cachet.

############################# Steps ############################
steps:
    enable: true
    title: "Étapes pour générer et placer un QR code à tout emplacement dans un XLSX"
    content: |
      [GroupDocs.Signature](/signature/java/) peut générer des QR codes dans de nombreux formats populaires et les placer sur les pages XLSX. Plus de 10 types de QR codes sont pris en charge et peuvent être rapidement intégrés dans des applications Java. Utilisez notre produit pour signer des documents avec des QR codes générés.
      
      1. Obtenez le fichier ou le flux XLSX à signer avec un QR code.
      2. Fournissez le texte pour QrCodeSignOptions.
      3. Personnalisez les options visuelles telles que la couleur, la position, la taille, etc.
      4. Enregistrez le fichier avec le QR code.
   
    code:
      platform: "java"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Signatures d'exemple"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // Passez le document à une nouvelle instance de Signature
        Signature signature = new Signature("input.xlsx");

        // Utilisez QrCodeSignOptions pour ajouter un QR code au document
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // Spécifiez le type de signature et sa position sur la page
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // Enregistrez le fichier avec le QR code ajouté
        signature.sign("output.xlsx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Ajoutez des signatures à vos documents"
  description: "L'API GroupDocs.Signature for Java prend en charge la signature de tous les formats de fichiers populaires. Générez, modifiez, recherchez, vérifiez et supprimez différents types de signatures."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Signer des documents"
      content: "GroupDocs.Signature prend en charge la signature avec des signatures de type Texte, Image, Code-barres, QR Code et Cachet. Placez-les sur n'importe quelle page de n'importe quel format de document pris en charge. Gérez les métadonnées du document avec des signatures de métadonnées, et protégez le contenu contre les modifications non autorisées en utilisant des certificats numériques."

    # feature loop
    - title: "Recherche et vérification"
      content: "Assurez-vous que toutes les signatures d'un document sont valides grâce à la procédure de vérification. Récupérez une liste complète des signatures dans un document en utilisant la fonction de recherche intégrée."

    # feature loop
    - title: "Modifier des signatures"
      content: "Modifiez facilement les propriétés des signatures après signature. Ajustez le contenu, la position, la couleur, la taille et d'autres attributs selon vos besoins."

    # feature loop
    - title: "Supprimer des signatures"
      content: "Supprimez les signatures indésirables sans difficulté. Divers types de signatures, y compris les certificats numériques, peuvent être supprimés programmatique de documents."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Comment personnaliser un QR code généré"
      content: |
        Utilisez cet exemple pour apprendre à placer un nouveau QR code sur une page XLSX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Obtenez le document qui doit être signé et passez-le à Signature
          Signature signature = new Signature("input.xlsx");

          // Utilisez les options du code QR pour fournir le texte avec les informations requises
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // Définissez la position relative du QR code sur la page
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // Définissez les marges de la signature
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Spécifiez la couleur du QR code
          signOptions.setForeColor(Color.RED);

          // Définissez les options de police pour le message
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Personnalisez la couleur de fond du QR code et le pinceau
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Ajoutez le QR code au document
          SignResult signResult = signature.sign("output.xlsx", signOptions);
          ```
        platform: "java"
        copy_title: "Copier"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "cliquez pour copier"
          copy_done: "copié"
        top_links:
          #  loop
          - title: "Télécharger le résultat"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.xlsx"
        links:
          #  loop
          - title: "Plus d'exemples"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Prêt à commencer ?"
  description: "Essayez les fonctionnalités de GroupDocs.Signature gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "Téléchargement Maven"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Découvrez nos principales offres"
    exclude: "qrcode"
    description: "Nous proposons une sélection diversifiée de fonctionnalités de signature et d'opérations avancées"
    items: 
          
        # operation loop 1
        - name: "Signatures électroniques"
          operation: "esign"
          link: "/signature/java/esign/xlsx/"
          description: "Ajoutez différents types de signatures aux formats de fichier pris en charge"

        # operation loop 2
        - name: "Ajouter du texte aux documents"
          operation: "text"
          link: "/signature/java/text/xlsx/"
          description: "Améliorez le contenu du document avec des signatures textuelles personnalisables"

        # operation loop 3
        - name: "Signatures d'image"
          operation: "image"
          link: "/signature/java/image/xlsx/"
          description: "Placez n'importe quelle image à n'importe quelle position dans un document"

        # operation loop 4
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/signature/java/barcode/xlsx/"
          description: "Créez et insérez divers codes-barres dans les documents pris en charge"

        # operation loop 5
        - name: "Générer des QR codes"
          operation: "qrcode"
          link: "/signature/java/qrcode/xlsx/"
          description: "Générez des QR Codes, y compris des codes QR, pour la signature de documents"
          
        # operation loop 6
        - name: "Certificats numériques"
          operation: "digital"
          link: "/signature/java/digital/xlsx/"
          description: "Sécurisez les affaires et signez des documents avec des certificats numériques"

        # operation loop 7
        - name: "Tampons"
          operation: "stamp"
          link: "/signature/java/stamp/xlsx/"
          description: "Utilisez le constructeur de tampons pour créer des tampons ronds ou carrés personnalisés"
          
        # operation loop 8
        - name: "Rechercher des signatures"
          operation: "search"
          link: "/signature/java/search/xlsx/"
          description: "Trouvez toutes les signatures précédemment ajoutées dans un document"
          
        # operation loop 9
        - name: "Vérification des signatures"
          operation: "verify"
          link: "/signature/java/verify/xlsx/"
          description: "Vérifiez l'authenticité des signatures après qu'elles aient été appliquées"
          
        # operation loop 10
        - name: "Modifier les signatures"
          operation: "modify"
          link: "/signature/java/modify/xlsx/"
          description: "Modifiez facilement une variété de signatures dans un document"
          
        # operation loop 11
        - name: "Supprimer les signatures"
          operation: "delete"
          link: "/signature/java/delete/xlsx/"
          description: "Retirez une large gamme de signatures précédemment appliquées"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Générez des QR codes pour des formats de fichiers supplémentaires"
    exclude: "XLSX"
    description: "Améliorez tous les formats de fichiers populaires avec des QR codes générés en utilisant l'API Java. Ajoutez des données de code-barres 2D pour un scan et un traitement aisés."
    items: 
          
        # format loop 1
        - name: "QRCode pour PDF"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "QRCode pour DOCX"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 3
        - name: "QRCode pour JPEG"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "Image JPEG"
          
        # format loop 4
        - name: "QRCode pour PPTX"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "Présentation Open XML de PowerPoint"
          
        # format loop 5
        - name: "QRCode pour XLSX"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"


          

---