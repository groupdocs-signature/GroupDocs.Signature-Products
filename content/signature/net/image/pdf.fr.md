



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:51
draft: false
lang: fr
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Ajouter des signatures d'image à un fichier PDF avec C#"
head_description: "Ajoutez une signature d'image dans un fichier PDF pour .NET en utilisant quelques lignes de code. Utilisez l'API GroupDocs.Signature for .NET pour ajouter des images."

############################# Header ############################
title: "Ajoutez une signature d'image aux fichiers PDF" 
description: "Utilisez GroupDocs.Signature for .NET pour intégrer sans effort des images dans une variété de formats de documents bureautiques, y compris PDF, Word, Excel et fichiers images. Incorporer l'image de la signature de votre patron peut créer une impression professionnelle marquante, élevant l'attrait visuel et l'authenticité de vos documents."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger gratuitement"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Découvrez GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "En savoir plus"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) offre des capacités complètes pour intégrer des signatures d'image à tout emplacement sur n'importe quelle page de vos documents professionnels. Améliorez vos flux de travail opérationnels en intégrant des images dans des fichiers PDF, des documents Word, des feuilles de calcul Excel, des présentations PowerPoint et une variété de formats d'image populaires grâce à notre bibliothèque robuste.

############################# Steps ############################
steps:
    enable: true
    title: "Comment ajouter une image à n'importe quel endroit d'un PDF avec C#"
    content: |
      Exploitez [GroupDocs.Signature](/signature/net/) pour doter les applications .NET de la capacité d'incorporer précisément des signatures dans n'importe quelle page de documents PDF. Améliorez les capacités de votre produit sans effort en intégrant notre solution.
      
      1. Instanciez la classe Signature avec le document PDF.
      2. Utilisez ImageSignOptions pour spécifier l'image de signature.
      3. Positionnez l'image précisément à l'emplacement souhaité sur n'importe quelle page.
      4. Enregistrez le nouveau document signé à un emplacement spécifique.
   
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
        // Initialisez Signature avec le chemin d'accès au document
        using (Signature signature = new Signature("input.pdf"))
        {
            // Configurez ImageSignOptions en utilisant une image pour la signature
            ImageSignOptions options = new ImageSignOptions("company_logo.jpg")
            {
                // Positionnez l'image dans le coin supérieur gauche de toutes les pages
                AllPages = true,
                Left = 100,
                Top = 200
            };

            // Enregistrez le document signé
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Solutions complètes de signature de documents"
  description: "Nous sommes heureux de présenter une large gamme de fonctionnalités de signature prises en charge par notre API. Ajoutez, modifiez, supprimez, recherchez et vérifiez sans effort divers types de signatures, y compris les signatures basées sur des images."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Signature d'image"
  features:
    # feature loop
    - title: "Intégrez des images dans les documents bureautiques"
      content: "Insérez sans effort des signatures électroniques et des images à n'importe quelle position désignée sur n'importe quelle page d'un document. Améliorez le contenu de votre document avec du texte, des images, des codes-barres, des métadonnées ou des certificats numériques pour renforcer la fonctionnalité et la sécurité."

    # feature loop
    - title: "Recherche et vérification de signatures"
      content: "Gérez les documents signés en vérifiant l'authenticité et l'intégrité des signatures. Récupérez une liste complète de toutes les signatures dans un document et examinez leurs attributs spécifiques."

    # feature loop
    - title: "Modifier les signatures"
      content: "Parfois, les signatures dans les documents peuvent nécessiter des mises à jour. Ajustez facilement le contenu, l'apparence, la taille ou la position des signatures existantes pour répondre aux exigences en évolution."

    # feature loop
    - title: "Supprimer les signatures redondantes"
      content: "Notre API facilite les opérations CRUD complètes pour la majorité des types de signatures. Vous pouvez supprimer efficacement des signatures de presque tous les formats de documents pris en charge lorsque cela est nécessaire."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Sécurisez le contenu du document avec des signatures d'image"
      content: |
        Découvrez comment enrichir les documents professionnels en intégrant des images, fournissant des informations supplémentaires.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Sélectionnez le document à signer
          using (Signature signature = new Signature("input.pdf"))
          {
              // Créez des options d'image avec le chemin d'image spécifié
              ImageSignOptions options = new ImageSignOptions("manager_signature.jpg")
              {
                    // Définissez les dimensions de la signature d'image
                    Width = 100,
                    Height = 100,

                    // Positionnez l'image dans le coin inférieur droit
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,

                    // Appliquez un rembourrage nécessaire à partir des bords de la page
                    Margin = new Padding() { Bottom = 120, Right = 120 },

                    // Facultativement, ajoutez une bordure personnalisée à l'image
                    Border = new Border()
                    {
                        Visible = true,
                        Color = Color.Red,
                        DashStyle = DashStyle.DashDotDot,
                        Weight = 5
                    },

                    // Faites pivoter la signature pour un alignement optimal
                    RotationAngle = 45
              };

              // Enregistrez le document mis à jour à l'emplacement souhaité
              SignResult result = signature.Sign("output.pdf", options);
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
            link: "/examples/signature/formats/signature_image.pdf"
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
    title: "Comprenez nos offres fonctionnelles"
    exclude: "image"
    description: "Explorez un ensemble diversifié de types de signatures et d'opérations robustes fournies par notre plateforme."
    items: 
          
        # operation loop 1
        - name: "Signatures électroniques"
          operation: "esign"
          link: "/signature/net/esign/pdf/"
          description: "Ajoutez différents types de signatures aux formats de fichier pris en charge"

        # operation loop 2
        - name: "Ajouter du texte aux documents"
          operation: "text"
          link: "/signature/net/text/pdf/"
          description: "Améliorez le contenu du document avec des signatures textuelles personnalisables"

        # operation loop 3
        - name: "Signatures d'image"
          operation: "image"
          link: "/signature/net/image/pdf/"
          description: "Placez n'importe quelle image à n'importe quelle position dans un document"

        # operation loop 4
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/signature/net/barcode/pdf/"
          description: "Créez et insérez divers codes-barres dans les documents pris en charge"

        # operation loop 5
        - name: "Générer des QR codes"
          operation: "qrcode"
          link: "/signature/net/qrcode/pdf/"
          description: "Générez des QR Codes, y compris des codes QR, pour la signature de documents"
          
        # operation loop 6
        - name: "Certificats numériques"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "Sécurisez les affaires et signez des documents avec des certificats numériques"

        # operation loop 7
        - name: "Tampons"
          operation: "stamp"
          link: "/signature/net/stamp/pdf/"
          description: "Utilisez le constructeur de tampons pour créer des tampons ronds ou carrés personnalisés"
          
        # operation loop 8
        - name: "Rechercher des signatures"
          operation: "search"
          link: "/signature/net/search/pdf/"
          description: "Trouvez toutes les signatures précédemment ajoutées dans un document"
          
        # operation loop 9
        - name: "Vérification des signatures"
          operation: "verify"
          link: "/signature/net/verify/pdf/"
          description: "Vérifiez l'authenticité des signatures après qu'elles aient été appliquées"
          
        # operation loop 10
        - name: "Modifier les signatures"
          operation: "modify"
          link: "/signature/net/modify/pdf/"
          description: "Modifiez facilement une variété de signatures dans un document"
          
        # operation loop 11
        - name: "Supprimer les signatures"
          operation: "delete"
          link: "/signature/net/delete/pdf/"
          description: "Retirez une large gamme de signatures précédemment appliquées"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Intégrez des images dans divers formats de fichiers"
    exclude: "PDF"
    description: "Exploitez l'API .NET pour ajouter des formats d'image pris en charge à une vaste gamme de documents. Redimensionnez, positionnez, sélectionnez des pages spécifiques et appliquez des signatures basées sur des images à vos documents sans effort."
    items: 
          
        # format loop 1
        - name: "Signer PDF avec une image"
          format: "PDF"
          link: "/signature/net/image/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Signer DOCX avec une image"
          format: "DOCX"
          link: "/signature/net/image/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 3
        - name: "Signer JPEG avec une image"
          format: "JPEG"
          link: "/signature/net/image/jpeg/"
          description: "Image JPEG"
          
        # format loop 4
        - name: "Signer PPTX avec une image"
          format: "PPTX"
          link: "/signature/net/image/pptx/"
          description: "Présentation Open XML de PowerPoint"
          
        # format loop 5
        - name: "Signer XLSX avec une image"
          format: "XLSX"
          link: "/signature/net/image/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"


          

---