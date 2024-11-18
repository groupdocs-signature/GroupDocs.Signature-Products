



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:46
draft: false
lang: fr
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Ajouter des cachets à XLSX en utilisant Java"
head_description: "Exploitez GroupDocs.Signature et Java pour créer des cachets personnalisés et les placer sur n'importe quelle page de documents XLSX."

############################# Header ############################
title: "Ajouter des cachets personnalisés à XLSX" 
description: "Créez et appliquez des cachets ronds ou carrés à n'importe quelle section de vos documents en utilisant GroupDocs.Signature for Java. Notre solution propose de nombreuses options de personnalisation pour répondre à tous vos besoins professionnels."
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
       [GroupDocs.Signature for Java](/signature/java/) est un outil robuste qui vous permet d'ajouter diverses signatures de cachets à des documents. Il prend en charge plus de 60 formats de fichiers différents, y compris les PDF, Word, Excel, images et fichiers ZIP. Vous pouvez appliquer des signatures par texte, image, code-barres, métadonnées, certificat numérique et cachets. En plus d’ajouter des signatures, vous pouvez les rechercher, les vérifier, les modifier et les supprimer.

############################# Steps ############################
steps:
    enable: true
    title: "Étapes pour ajouter des cachets à XLSX via Java"
    content: |
      [GroupDocs.Signature](/signature/java/) fournit un constructeur de cachets qui peut être très bénéfique pour les applications Java. Utilisez-le pour créer des cachets bien personnalisés pour vos pages de documents.
      
      1. Fournissez le document XLSX à tamponner.
      2. Utilisez StampSignOptions pour configurer tous les paramètres nécessaires.
      3. Ajoutez autant de lignes que nécessaire.
      4. Appliquez le cachet et enregistrez le document.
   
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
        // Utilisez le chemin du document avec l'objet Signature
        Signature signature = new Signature("input.xlsx");

        // Instanciez StampSignOptions avec le texte de signature souhaité
        StampSignOptions options = new StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // Ajoutez une ou plusieurs lignes de cachets
        StampLine outerLine = new StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(Color.WHITE);
        outerLine.setBackgroundColor(Color.BLUE);
        options.getOuterLines().add(outerLine);

        // Enregistrez le document tamponné
        SignResult result = signature.sign("output.xlsx", options);
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "Protégez le contenu de votre document avec des signatures"
  description: "La bibliothèque GroupDocs.Signature for Java est conçue pour signer et gérer des signatures dans des formats de fichiers populaires. Ajoutez, modifiez, vérifiez ou supprimez facilement des cachets et d'autres types de signatures."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Signatures de cachets avec GroupDocs.Signature"
  features:
    # feature loop
    - title: "Signez vos documents"
      content: "Appliquez des signatures personnalisables à n'importe quelle partie de votre document. Choisissez parmi différentes types de signatures, y compris texte, images, codes-barres, QR codes et cachets. De plus, des métadonnées cachées peuvent être ajoutées ou modifiées pour améliorer la sécurité du document."

    # feature loop
    - title: "Recherchez et validez les signatures"
      content: "Une fois qu'un document est signé, utilisez nos outils de vérification pour vous assurer que le contenu de la signature est valide. Recherchez et récupérez une liste de toutes les signatures pour un traitement ultérieur."

    # feature loop
    - title: "Mettez à jour les signatures si nécessaire"
      content: "Modifiez facilement un large éventail de signatures appliquées à un document. Mettez à jour des propriétés telles que la taille, la couleur, la position, le contenu, et plus encore."

    # feature loop
    - title: "Supprimez les signatures"
      content: "Vous devez supprimer des signatures d'un document ? Notre API prend totalement en charge la suppression des signatures, ce qui facilite la gestion de vos documents."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Ajouter des cachets personnalisés aux documents en utilisant des signatures spéciales"
      content: |
        Apprenez à générer et à ajouter des cachets personnalisés avec des informations textuelles importantes à vos documents.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Fournissez le document à tamponner
          Signature signature = new Signature("input.xlsx");

          // Instanciez l'objet options de cachet
          StampSignOptions options = new StampSignOptions();

          // Définissez la taille et la position sur la page
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setAllPages(true);

          // Ajoutez une ou plusieurs lignes rondes extérieures avec du texte
          StampLine outerLine1 = new StampLine();
          outerLine1.setText("* The best  choice *");
          outerLine1.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
          SignatureFont signatureFont1 = new SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName("Arial");
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(Color.WHITE);
          outerLine1.setBackgroundColor(Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // Ajoutez une ou plusieurs lignes carrées intérieures
          StampLine innerLine1 = new StampLine();
          innerLine1.setText("Company #1");
          innerLine1.setTextColor(Color.RED);
          SignatureFont signFont1 = new SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);

          // Enregistrez le document tamponné
          SignResult result = signature.sign("output.xlsx", options);
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
            link: "/examples/signature/formats/signature_stamp.xlsx"
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
    title: "Découvrez nos fonctionnalités principales"
    exclude: "stamp"
    description: "Utilisez un large éventail d'options pour ajouter, gérer et supprimer des signatures."
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
    title: "Ajoutez des cachets dans plusieurs formats de fichiers"
    exclude: "XLSX"
    description: "L'API GroupDocs.Signature prend en charge l'ajout de cachets à des documents dans plus de 60 formats. Placez des cachets sur n'importe quelle page ou zone pour améliorer la gestion et la personnalisation des documents."
    items: 
          
        # format loop 1
        - name: "Tamponner PDF"
          format: "PDF"
          link: "/signature/java/stamp/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Tamponner DOCX"
          format: "DOCX"
          link: "/signature/java/stamp/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 3
        - name: "Tamponner JPEG"
          format: "JPEG"
          link: "/signature/java/stamp/jpeg/"
          description: "Image JPEG"
          
        # format loop 4
        - name: "Tamponner PPTX"
          format: "PPTX"
          link: "/signature/java/stamp/pptx/"
          description: "Présentation Open XML de PowerPoint"
          
        # format loop 5
        - name: "Tamponner XLSX"
          format: "XLSX"
          link: "/signature/java/stamp/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"


          

---