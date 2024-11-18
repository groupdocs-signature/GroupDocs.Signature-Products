



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:47
draft: false
lang: fr
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tampons ronds et carrés XLSX via C#"
head_description: "Utilisez GroupDocs.Signature for .NET pour générer et intégrer des tampons personnalisés dans vos fichiers XLSX."

############################# Header ############################
title: "Générez des tampons pour des fichiers XLSX" 
description: "Intégrez sans effort des tampons conçus sur mesure dans n'importe quelle section de vos documents grâce à GroupDocs.Signature for .NET, offrant une flexibilité considérable pour le placement et la configuration des tampons afin de répondre à vos besoins professionnels."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargez votre version gratuite"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Aperçu de GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "En savoir plus"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) est un outil polyvalent qui permet l'insertion de plusieurs types de signatures dans les documents, y compris les tampons personnalisables. Supportant plus de 60 formats de fichiers, allant des PDF et documents Word aux images et fichiers ZIP, vous pouvez enrichir vos documents avec du texte, des images, des codes-barres, des métadonnées, des certificats numériques et des tampons. De plus, vous avez un contrôle total pour rechercher, valider, modifier ou supprimer toute signature appliquée à vos fichiers.

############################# Steps ############################
steps:
    enable: true
    title: "Comment intégrer un tampon dans XLSX en utilisant C#"
    content: |
      [GroupDocs.Signature](/signature/net/) offre une fonctionnalité robuste de création de tampons, idéale pour améliorer les applications .NET. Profitez de cet outil pour concevoir et mettre en œuvre des tampons hautement personnalisés sur vos pages de documents.
      
      1. Fournissez le document XLSX à tamponner.
      2. Utilisez StampSignOptions pour configurer méticuleusement tous les paramètres requis.
      3. Ajoutez plusieurs lignes de tampon selon vos besoins.
      4. Appliquez le tampon configuré et enregistrez le document modifié.
   
    code:
      platform: "net"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Signatures d'exemple"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // Intégrez le chemin du document avec l'instance Signature
        using (Signature signature = new Signature("input.xlsx"))
        {
            // Initialisez StampSignOptions avec le contenu de signature requis
            StampSignOptions options = new StampSignOptions();
            options.Height = 180;
            options.Width = 180;

            // Incorporez une ou plusieurs lignes de tampon
            options.OuterLines.Add(
                new StampLine()
                {
                    Text = "* The Best Company *",
                    TextRepeatType = StampTextRepeatType.FullTextRepeat,
                    Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                    Height = 22,
                    TextBottomIntent = 6,
                    TextColor = Color.WhiteSmoke,
                    BackgroundColor = Color.DarkSlateBlue
                }
            );

            // Préservez le document avec le tampon appliqué
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Exploitez les signatures pour sécuriser et améliorer l'intégrité des documents"
  description: "Avec la bibliothèque GroupDocs.Signature for .NET, vous pouvez intégrer sans effort la fonctionnalité de signature dans vos documents. Ajoutez, modifiez, vérifiez ou supprimez facilement des tampons personnalisés et d'autres types de signatures, offrant flexibilité et précision pour une gestion sécurisée des documents."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Signatures de Tampon Alimentées par GroupDocs.Signature"
  features:
    # feature loop
    - title: "Signature documentaire complète"
      content: "Améliorez vos documents en plaçant des signatures, incluant texte, images, codes-barres, codes QR et tampons, à n'importe quelle position ou page du fichier. De plus, gérez les métadonnées intégrées et appliquez des certificats numériques pour protéger contre les modifications non autorisées."

    # feature loop
    - title: "Recherche et validation efficaces des signatures"
      content: "Après la signature, vérifiez l'authenticité et l'intégrité des signatures documentaires. Utilisez la fonctionnalité de recherche avancée pour récupérer et gérer toutes les données de signature intégrées dans le document."

    # feature loop
    - title: "Modifier et personnaliser les signatures"
      content: "Ajustez les signatures précédemment insérées sans difficulté. Que vous ayez besoin de changer le contenu, la position, la taille ou la couleur, notre solution offre une flexibilité totale pour la modification des signatures."

    # feature loop
    - title: "Supprimer les signatures sans effort"
      content: "Lorsque les signatures doivent être supprimées, GroupDocs.Signature for .NET fournit un ensemble complet d'outils pour supprimer tout type de signature, y compris les tampons, certificats numériques, et plus, garantissant que vos documents restent à jour et conformes."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Implémentez des tampons personnalisés dans les documents"
      content: |
        Découvrez comment créer et intégrer des tampons personnalisés portant des détails textuels critiques dans vos documents.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Fournissez le document à tamponner
          using (Signature signature = new Signature("input.xlsx"))
          {
              // Initialisez les options de tampon avec les configurations souhaitées
              StampSignOptions options = new StampSignOptions()
              {
                    // Définissez les dimensions et la position du tampon sur la page
                    Height = 200,
                    Width = 200,
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,
                    AllPages = true
              };

              // Incorporez des lignes extérieures circulaires avec du texte
              options.OuterLines.Add(
                    new StampLine()
                    {
                        Text = "* The best  choice *",
                        TextRepeatType = StampTextRepeatType.FullTextRepeat,
                        Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                        Height = 22,
                        TextBottomIntent = 6,
                        TextColor = Color.WhiteSmoke,
                        BackgroundColor = Color.DarkSlateBlue
                    }
              );

              // Intégrez des lignes carrées intérieures si nécessaire
              options.InnerLines.Add(
                    new StampLine()
                    { 
                        Text = "Company #1",
                        TextColor = Color.MediumVioletRed,
                        Font = new SignatureFont() { Size = 20, Bold = true },
                        Height = 40
                    }
              );

              // Finalisez et enregistrez le document tamponné
              SignResult result = signature.Sign("output.xlsx", options);
          }
          ```
        platform: "net"
        copy_title: "Copier"
        install:
          command: "dotnet add package GroupDocs.Signature"
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
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Prêt à commencer ?"
  description: "Essayez les fonctionnalités de GroupDocs.Signature gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "Téléchargement Nuget"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Explorez les fonctionnalités principales"
    exclude: "stamp"
    description: "Découvrez un large éventail d'options pour créer, gérer et supprimer différents types de signatures, garantissant un contrôle complet sur vos flux de travail documentaires."
    items: 
          
        # operation loop 1
        - name: "Signatures électroniques"
          operation: "esign"
          link: "/signature/net/esign/xlsx/"
          description: "Ajoutez différents types de signatures aux formats de fichier pris en charge"

        # operation loop 2
        - name: "Ajouter du texte aux documents"
          operation: "text"
          link: "/signature/net/text/xlsx/"
          description: "Améliorez le contenu du document avec des signatures textuelles personnalisables"

        # operation loop 3
        - name: "Signatures d'image"
          operation: "image"
          link: "/signature/net/image/xlsx/"
          description: "Placez n'importe quelle image à n'importe quelle position dans un document"

        # operation loop 4
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/signature/net/barcode/xlsx/"
          description: "Créez et insérez divers codes-barres dans les documents pris en charge"

        # operation loop 5
        - name: "Générer des QR codes"
          operation: "qrcode"
          link: "/signature/net/qrcode/xlsx/"
          description: "Générez des QR Codes, y compris des codes QR, pour la signature de documents"
          
        # operation loop 6
        - name: "Certificats numériques"
          operation: "digital"
          link: "/signature/net/digital/xlsx/"
          description: "Sécurisez les affaires et signez des documents avec des certificats numériques"

        # operation loop 7
        - name: "Tampons"
          operation: "stamp"
          link: "/signature/net/stamp/xlsx/"
          description: "Utilisez le constructeur de tampons pour créer des tampons ronds ou carrés personnalisés"
          
        # operation loop 8
        - name: "Rechercher des signatures"
          operation: "search"
          link: "/signature/net/search/xlsx/"
          description: "Trouvez toutes les signatures précédemment ajoutées dans un document"
          
        # operation loop 9
        - name: "Vérification des signatures"
          operation: "verify"
          link: "/signature/net/verify/xlsx/"
          description: "Vérifiez l'authenticité des signatures après qu'elles aient été appliquées"
          
        # operation loop 10
        - name: "Modifier les signatures"
          operation: "modify"
          link: "/signature/net/modify/xlsx/"
          description: "Modifiez facilement une variété de signatures dans un document"
          
        # operation loop 11
        - name: "Supprimer les signatures"
          operation: "delete"
          link: "/signature/net/delete/xlsx/"
          description: "Retirez une large gamme de signatures précédemment appliquées"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Appliquez des tampons à divers formats de documents"
    exclude: "XLSX"
    description: "L'API GroupDocs.Signature permet d'incorporer des tampons à plus de 60 types de fichiers standard de l'industrie. Appliquez sans effort des tampons personnalisés à n'importe quel endroit de vos documents, permettant un meilleur suivi et une personnalisation des documents."
    items: 
          
        # format loop 1
        - name: "Tamponner PDF"
          format: "PDF"
          link: "/signature/net/stamp/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Tamponner DOCX"
          format: "DOCX"
          link: "/signature/net/stamp/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 3
        - name: "Tamponner JPEG"
          format: "JPEG"
          link: "/signature/net/stamp/jpeg/"
          description: "Image JPEG"
          
        # format loop 4
        - name: "Tamponner PPTX"
          format: "PPTX"
          link: "/signature/net/stamp/pptx/"
          description: "Présentation Open XML de PowerPoint"
          
        # format loop 5
        - name: "Tamponner XLSX"
          format: "XLSX"
          link: "/signature/net/stamp/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"


          

---