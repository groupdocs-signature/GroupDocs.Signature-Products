



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:21
draft: false
lang: fr
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Générez un code QR pour les fichiers JPEG en utilisant C#"
head_description: "Exploitez l'API GroupDocs.Signature pour générer un code QR pour les fichiers JPEG. Intégrez facilement des codes QR sur n'importe quelle page pour améliorer la fonctionnalité."

############################# Header ############################
title: "Générez des codes QR pour JPEG" 
description: "Générez des codes-barres 2D à partir de données textuelles ou numériques et appliquez-les sur plusieurs pages et formats, y compris des PDF, Word, Excel, et plus, via GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Commencez votre essai gratuit"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Découvrez les capacités de GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "En savoir plus"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) propose une vaste gamme de fonctionnalités, permettant aux utilisateurs de générer et d'incorporer différents types de signatures dans les principaux formats de documents. Que ce soit pour des PDF, des documents Word, des feuilles Excel, des présentations PowerPoint ou des fichiers image, vous pouvez rehausser vos documents avec des signatures Textuelles, d'Image, de Code-Barres, QR Code, de Métadonnées, Numériques, et de Tampons.

############################# Steps ############################
steps:
    enable: true
    title: "Comment générer et insérer un code QR à n'importe quel endroit d'un JPEG"
    content: |
      [GroupDocs.Signature](/signature/net/) facilite la génération de codes QR dans divers formats populaires et leur placement sur les pages JPEG. Supportant plus de 10 types de codes QR, notre bibliothèque peut être intégrée de manière fluide dans les applications .NET. Améliorez vos documents avec des signatures QR codes utilisant notre produit.
      
      1. Acquérez le fichier ou le flux JPEG à signer avec un code QR.
      2. Fournissez le texte requis à QrCodeSignOptions.
      3. Personnalisez les paramètres visuels tels que la couleur, la position, la taille, etc.
      4. Enregistrez le document avec le code QR intégré.
   
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
        // Initialisez une nouvelle instance de Signature avec le document
        using (Signature signature = new Signature("input.jpeg"))
        {
            // Utilisez QrCodeSignOptions pour intégrer un code QR dans le document
            QrCodeSignOptions options = new QrCodeSignOptions("Text Content")
                {
                    // Spécifiez le type de signature et désignez sa position sur la page
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150
                };

            // Enregistrez le document avec le code QR intégré
            SignResult result = signature.Sign("output.jpeg", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Intégration complète de signatures pour documents"
  description: "Avec l'API GroupDocs.Signature for .NET, les utilisateurs peuvent générer, modifier, rechercher, valider et supprimer aisément une variété de types de signatures, rationalisant ainsi les flux de travail documentaires avec une précision inégalée."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Signature de documents avec plusieurs types de signatures"
      content: "GroupDocs.Signature permet l'application de signatures Textuelles, d'Image, de Code-Barres, de QR Code et de Tampons à tout format de document. Les signatures peuvent être positionnées avec précision sur n'importe quelle page, et les métadonnées peuvent être gérées de manière fluide via des signatures de métadonnées. Protégez l'intégrité de vos documents en intégrant des certificats numériques qui empêchent les modifications non autorisées."

    # feature loop
    - title: "Recherche et validation des signatures"
      content: "Vérifiez l'authenticité et la précision des signatures de documents grâce à un processus de validation avancé. Récupérez facilement une liste détaillée de toutes les signatures intégrées dans un document pour un contrôle exhaustif."

    # feature loop
    - title: "Modification personnalisable des signatures"
      content: "Mettez à jour et affinez les signatures précédemment appliquées en ajustant le contenu, la position, la couleur, la taille et d'autres attributs pour répondre à vos besoins spécifiques."

    # feature loop
    - title: "Suppression efficace des signatures"
      content: "Rationalisez la gestion de vos documents en supprimant de manière programmatique les signatures indésirables. Que vous traitiez des certificats numériques ou d'autres types de signatures, la suppression peut être effectuée rapidement et efficacement."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Comment générer un code QR avec diverses options ?"
      content: |
        Cet exemple démontre comment placer un code QR personnalisé sur une page JPEG.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Récupérez le document à signer et transmettez-le à Signature
          using (Signature signature = new Signature("input.jpeg"))
          {
              // Configurez les options de code QR avec le texte nécessaire
              QrCodeSignOptions options = new QrCodeSignOptions("Archived on July 11, 2019")
              {
                    // Désignez la position relative du code QR sur la page
                    VerticalAlignment = Domain.VerticalAlignment.Top,
                    HorizontalAlignment = Domain.HorizontalAlignment.Right,

                    // Définissez le rembourrage de la signature
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // Spécifiez la couleur du code QR
                    ForeColor = Color.Red,

                    // Définissez les options de police pour le message
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // Personnalisez la couleur de fond et le pinceau du code QR
                    Background = new Background()
                    {
                        Color = Color.LimeGreen,
                        Transparency = 0.5,
                        Brush = new Domain.Extensions.LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                    }
              };

              // Intégrez le code QR dans le document
              SignResult result = signature.Sign("output.jpeg", options);
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
            link: "/examples/signature/formats/signature_qrcode.jpeg"
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
    title: "Découvrez nos solutions de signature"
    exclude: "qrcode"
    description: "Nous présentons fièrement une large gamme de types de signatures et de fonctionnalités opérationnelles."
    items: 
          
        # operation loop 1
        - name: "Signatures électroniques"
          operation: "esign"
          link: "/signature/net/esign/jpeg/"
          description: "Ajoutez différents types de signatures aux formats de fichier pris en charge"

        # operation loop 2
        - name: "Ajouter du texte aux documents"
          operation: "text"
          link: "/signature/net/text/jpeg/"
          description: "Améliorez le contenu du document avec des signatures textuelles personnalisables"

        # operation loop 3
        - name: "Signatures d'image"
          operation: "image"
          link: "/signature/net/image/jpeg/"
          description: "Placez n'importe quelle image à n'importe quelle position dans un document"

        # operation loop 4
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/signature/net/barcode/jpeg/"
          description: "Créez et insérez divers codes-barres dans les documents pris en charge"

        # operation loop 5
        - name: "Générer des QR codes"
          operation: "qrcode"
          link: "/signature/net/qrcode/jpeg/"
          description: "Générez des QR Codes, y compris des codes QR, pour la signature de documents"
          
        # operation loop 6
        - name: "Certificats numériques"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "Sécurisez les affaires et signez des documents avec des certificats numériques"

        # operation loop 7
        - name: "Tampons"
          operation: "stamp"
          link: "/signature/net/stamp/jpeg/"
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
    title: "Générez des codes QR pour d'autres formats de documents"
    exclude: "JPEG"
    description: "Améliorez tous les formats de fichiers standard de l'industrie avec la capacité d'incorporer des codes QR via l'API .NET. Stockez et encodez des informations critiques dans des codes-barres 2D pour un scan et une récupération de données sans faille."
    items: 
          
        # format loop 1
        - name: "QRCode pour PDF"
          format: "PDF"
          link: "/signature/net/qrcode/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "QRCode pour DOCX"
          format: "DOCX"
          link: "/signature/net/qrcode/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 3
        - name: "QRCode pour JPEG"
          format: "JPEG"
          link: "/signature/net/qrcode/jpeg/"
          description: "Image JPEG"
          
        # format loop 4
        - name: "QRCode pour PPTX"
          format: "PPTX"
          link: "/signature/net/qrcode/pptx/"
          description: "Présentation Open XML de PowerPoint"
          
        # format loop 5
        - name: "QRCode pour XLSX"
          format: "XLSX"
          link: "/signature/net/qrcode/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"


          

---