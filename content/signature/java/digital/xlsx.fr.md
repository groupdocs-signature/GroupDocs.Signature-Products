



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:57
draft: false
lang: fr
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Ajout de signatures électroniques numériques à un fichier XLSX avec Java"
head_description: "Apposez une signature numérique sur un fichier XLSX en utilisant Java avec seulement quelques lignes de code. Utilisez GroupDocs.Signature for Java pour signer de nombreux formats de fichiers."

############################# Header ############################
title: "Signer XLSX avec des signatures numériques" 
description: "Protégez le contenu de vos documents professionnels en les scellant avec des certificats numériques grâce aux fonctionnalités de GroupDocs.Signature for Java. Nous proposons plusieurs façons de marquer et de sécuriser vos documents."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger gratuitement"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "À propos de GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "En savoir plus"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) est une solution de signature complète qui prend en charge divers types de traitement de documents. Vous pouvez ajouter du texte, des images, des certificats numériques et des tampons à des fichiers dans plus de 60 formats, y compris PDF, MS Office, images, fichiers ZIP et autres formats commerciaux populaires. De plus, les documents signés peuvent être recherchés, vérifiés, modifiés ou supprimés automatiquement de manière pratique.

############################# Steps ############################
steps:
    enable: true
    title: "Étapes pour protéger XLSX avec des certificats numériques en Java"
    content: |
      [GroupDocs.Signature](/signature/java/) permet aux développeurs Java d'empêcher les modifications dans les documents XLSX en utilisant des signatures numériques. Renforcez vos applications d'entreprise avec la capacité de sécuriser des données importantes.
      
      1. Passez le document XLSX au constructeur de la classe Signature.
      2. Utilisez un certificat numérique et son mot de passe pour protéger le document.
      3. Optionnellement, ajoutez une représentation visuelle de la signature numérique sur les pages du document.
      4. Signez le document pour empêcher toute modification future.
   
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
        // Utilisez Signature avec le document pour la signature numérique
        Signature signature = new Signature("input.xlsx");

        // Fournissez un certificat numérique et un mot de passe
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Configurez une représentation visuelle si nécessaire
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);

        // Protégez le document avec un certificat numérique
        SignResult result = signature.sign("output.xlsx", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Améliorez ou protégez le contenu des documents avec des signatures"
  description: "La bibliothèque GroupDocs.Signature for Java est capable de signer tous les formats de fichiers populaires. Ajoutez, modifiez, vérifiez ou supprimez divers types de signatures automatiquement pour rationaliser vos processus commerciaux."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Fonctionnalités de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Ajouter des signatures aux documents"
      content: "Des signatures Textuelles, d'Image, de Code-Barres, de QR-Code ou de Tampons peuvent être précisément ajoutées à n'importe quelle page de tout document supporté. Des métadonnées cachées comme EXIF peuvent être ajoutées ou modifiées dans les images et la plupart des types de fichiers. Protégez le contenu des documents contre les modifications non autorisées en utilisant des signatures numériques."

    # feature loop
    - title: "Recherche et vérification des signatures"
      content: "Les documents peuvent être traités de différentes manières après leur signature. Vérifiez les documents signés pour vous assurer qu'ils ont été correctement traités. Si vous avez besoin de plus de contrôle, récupérez une liste de toutes les signatures via une recherche."

    # feature loop
    - title: "Modifier les signatures"
      content: "La plupart des types de signatures supportent des modifications ultérieures. Vous êtes libre de corriger le texte, changer la position, la couleur, la taille, et plus encore."

    # feature loop
    - title: "Supprimer les signatures inutiles"
      content: "Notre solution supporte les opérations CRUD complètes pour les signatures. De nombreux types de signatures, y compris les certificats numériques, peuvent être supprimés d'un document si nécessaire."
      
  code_samples:
    # code sample loop
    - title: "Protéger les documents avec des signatures numériques"
      content: |
        Apprenez comment sécuriser un document contre les modifications en utilisant des signatures numériques.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Fournissez un document à signer
        Signature signature = new Signature("input.xlsx");

        // Utilisez un certificat numérique valide avec un mot de passe
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Spécifiez des données textuelles supplémentaires
        options.setReason("Security issue");
        options.setContact("John Smith");
        options.setLocation("Office D.W.");

        // Utilisez une image et d'autres options pour une représentation visuelle
        options.setImageFilePath("image.png");

        options.setAllPages(true);
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        Padding padding = new Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);

        // Enregistrez le document protégé dans un autre emplacement
        SignResult result = signature.sign("output.xlsx", options);
        ```
        {{< /landing/code >}}


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
    title: "Examinez notre ensemble complet de fonctionnalités"
    exclude: "digital"
    description: "Nous sommes fiers de l'étendue des fonctionnalités et du support des signatures que notre plateforme propose."
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
    title: "Signer des documents dans d'autres formats"
    exclude: "XLSX"
    description: "L'API Java vous permet de traiter plus de 60 formats. Créez et ajoutez diverses signatures à n'importe quelle page, scellez le contenu avec des certificats numériques, et gérez et modifiez les signatures existantes dans le document."
    items: 
          
        # format loop 1
        - name: "Protéger le PDF"
          format: "PDF"
          link: "/signature/java/digital/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Protéger le DOCX"
          format: "DOCX"
          link: "/signature/java/digital/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 3
        - name: "Protéger le PPTX"
          format: "PPTX"
          link: "/signature/java/digital/pptx/"
          description: "Présentation Open XML de PowerPoint"
          
        # format loop 4
        - name: "Protéger le XLSX"
          format: "XLSX"
          link: "/signature/java/digital/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"


          

---