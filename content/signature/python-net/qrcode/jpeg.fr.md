



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:23
draft: false
lang: fr
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Générez des codes QR pour des fichiers JPEG en utilisant Python"
head_description: "Utilisez l'API GroupDocs.Signature pour générer et intégrer des codes QR dans des fichiers JPEG. Placez facilement des codes QR sur n'importe quelle page pour ajouter des fonctionnalités supplémentaires."

############################# Header ############################
title: "Générez des codes QR pour JPEG" 
description: "Créez des codes-barres 2D à partir de données textuelles ou numériques et appliquez-les à diverses pages et formats, y compris les PDF, Word, Excel, et plus encore avec GroupDocs.Signature for Python via .NET."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Essai gratuit"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Découvrez les fonctionnalités de GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "En savoir plus"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) offre un large éventail de capacités, permettant aux utilisateurs de générer et d'intégrer différents types de signatures dans les principaux formats de documents. Que ce soit pour des PDFs, Word, Excel, PowerPoint ou des images, améliorez vos documents avec des signatures Textuelles, Image, Code-barres, QR Code, Métadonnées, Numérique ou Marque.

############################# Steps ############################
steps:
    enable: true
    title: "Étapes pour générer et insérer un code QR dans JPEG"
    content: |
      [GroupDocs.Signature](/signature/python-net/) vous permet de créer des codes QR dans des formats populaires et de les placer sur des pages JPEG. Avec le support de plus de 10 types de codes QR, vous pouvez intégrer cette fonctionnalité de manière transparente dans les applications Python via .NET. Améliorez vos documents avec des signatures de code QR en utilisant notre produit.
      
      1. Obtenez le fichier ou le flux JPEG où le code QR sera ajouté.
      2. Fournissez le texte requis à QrCodeSignOptions.
      3. Personnalisez les paramètres visuels comme la couleur, la position et la taille.
      4. Enregistrez le document avec le code QR intégré.
   
    code:
      platform: "python-net"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Signatures d'exemple"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Initialisez une nouvelle instance de Signature avec le document
            with sg.Signature('input.jpeg') as signature:

                # Utilisez QrCodeSignOptions pour intégrer un code QR dans le document
                options = sg.QrCodeSignOptions("Text Content")

                # Spécifiez le type de signature et définissez sa position sur la page
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # Enregistrez le document avec le code QR intégré
                result = signature.Sign("output.jpeg", options)
        ```                 

############################# More features ############################
more_features:
  enable: true
  title: "Intégration complète des signatures pour les documents"
  description: "Avec l'API GroupDocs.Signature for Python via .NET, les utilisateurs peuvent générer, modifier, rechercher, valider et supprimer différents types de signatures, simplifiant ainsi les flux de travail documentaires avec précision."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Appliquez plusieurs types de signatures"
      content: "GroupDocs.Signature permet l'application de signatures Textuelles, Image, Code-barres, QR Code et Marque à n'importe quel document. Vous pouvez placer précisément les signatures sur n'importe quelle page et gérer facilement les métadonnées. Protégez vos documents contre les modifications non autorisées avec des certificats numériques."

    # feature loop
    - title: "Rechercher et valider les signatures"
      content: "Vérifiez l'authenticité et la précision des signatures des documents en utilisant des outils de validation avancés. Obtenez facilement une liste détaillée de toutes les signatures intégrées dans un document pour un meilleur contrôle."

    # feature loop
    - title: "Modifier les signatures existantes"
      content: "Vous pouvez mettre à jour les signatures appliquées précédemment en ajustant le contenu, la position, la couleur, la taille et d'autres attributs selon vos besoins spécifiques."

    # feature loop
    - title: "Supprimer facilement les signatures"
      content: "Rationalisez la gestion des documents en supprimant rapidement les signatures indésirables. Que ce soit un certificat numérique ou un autre type de signature, la suppression peut se faire efficacement."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Personnalisez un code QR généré"
      content: |
        Cet exemple montre comment placer un code QR personnalisé sur une page JPEG.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Obtenez le document à signer et passez-le à Signature
              with sg.Signature('input.jpeg') as signature:

                    # Configurez les options du code QR avec le texte requis
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # Définissez la position du code QR sur la page
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # Définissez le padding pour la signature
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Choisissez la couleur du code QR
                    options.ForeColor = sg.Color.Red

                    # Définissez les options de police pour le message
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Définissez la couleur de fond et le pinceau pour le code QR
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # Intégrez le code QR dans le document
                    result = signature.Sign("output.jpeg", options)
          ```
        platform: "python-net"
        copy_title: "Copier"
        install:
          command: "pip install groupdocs-signature-net"
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
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Prêt à commencer ?"
  description: "Essayez les fonctionnalités de GroupDocs.Signature gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "Téléchargement PyPi"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Explorez nos solutions de signature"
    exclude: "qrcode"
    description: "Nous proposons une large variété de types et d'opérations de signatures pour répondre à vos besoins documentaires."
    items: 
          
        # operation loop 1
        - name: "Signatures électroniques"
          operation: "esign"
          link: "/signature/python-net/esign/jpeg/"
          description: "Ajoutez différents types de signatures aux formats de fichier pris en charge"

        # operation loop 2
        - name: "Ajouter du texte aux documents"
          operation: "text"
          link: "/signature/python-net/text/jpeg/"
          description: "Améliorez le contenu du document avec des signatures textuelles personnalisables"

        # operation loop 3
        - name: "Signatures d'image"
          operation: "image"
          link: "/signature/python-net/image/jpeg/"
          description: "Placez n'importe quelle image à n'importe quelle position dans un document"

        # operation loop 4
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/signature/python-net/barcode/jpeg/"
          description: "Créez et insérez divers codes-barres dans les documents pris en charge"

        # operation loop 5
        - name: "Générer des QR codes"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "Générez des QR Codes, y compris des codes QR, pour la signature de documents"
          
        # operation loop 6
        - name: "Certificats numériques"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "Sécurisez les affaires et signez des documents avec des certificats numériques"

        # operation loop 7
        - name: "Tampons"
          operation: "stamp"
          link: "/signature/python-net/stamp/jpeg/"
          description: "Utilisez le constructeur de tampons pour créer des tampons ronds ou carrés personnalisés"
          
        # operation loop 8
        - name: "Rechercher des signatures"
          operation: "search"
          link: "/signature/python-net/search/pdf/"
          description: "Trouvez toutes les signatures précédemment ajoutées dans un document"
          
        # operation loop 9
        - name: "Vérification des signatures"
          operation: "verify"
          link: "/signature/python-net/verify/pdf/"
          description: "Vérifiez l'authenticité des signatures après qu'elles aient été appliquées"
          
        # operation loop 10
        - name: "Modifier les signatures"
          operation: "modify"
          link: "/signature/python-net/modify/pdf/"
          description: "Modifiez facilement une variété de signatures dans un document"
          
        # operation loop 11
        - name: "Supprimer les signatures"
          operation: "delete"
          link: "/signature/python-net/delete/pdf/"
          description: "Retirez une large gamme de signatures précédemment appliquées"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Intégrez des codes QR dans divers formats de documents"
    exclude: "JPEG"
    description: "Utilisez l'API Python via .NET pour intégrer des codes QR dans n'importe quel format de document standard de l'industrie. Stockez et encodez des informations importantes dans des codes-barres 2D pour un scan et une récupération des données faciles."
    items: 
          
        # format loop 1
        - name: "QRCode pour PDF"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "QRCode pour DOCX"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 3
        - name: "QRCode pour JPEG"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "Image JPEG"
          
        # format loop 4
        - name: "QRCode pour PPTX"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "Présentation Open XML de PowerPoint"
          
        # format loop 5
        - name: "QRCode pour XLSX"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"


          

---