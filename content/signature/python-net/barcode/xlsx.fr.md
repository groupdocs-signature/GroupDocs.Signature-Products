



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:07
draft: false
lang: fr
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Intégrez un code-barres dans votre XLSX avec Python"
head_description: "Ajoutez efficacement des signatures de code-barres aux documents XLSX avec quelques lignes en Python. GroupDocs.Signature offre des solutions de signature sans faille pour plusieurs formats de documents."

############################# Header ############################
title: "Générez des codes-barres pour XLSX" 
description: "Avec GroupDocs.Signature for Python via .NET, vous pouvez placer des codes-barres dans vos documents professionnels où cela est nécessaire. Notre solution propose des options flexibles pour la personnalisation des signatures de code-barres."
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
    title: "À propos de GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "En savoir plus"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) est un outil puissant de signature de documents qui prend en charge une large gamme de types de signatures, y compris du texte, des images, des codes-barres, des certificats numériques et des tampons. Compatible avec plus de 60 formats de fichiers, tels que PDF, MS Office, images, ZIP, etc., il vous permet non seulement d'appliquer des signatures, mais aussi de les rechercher, vérifier, modifier ou supprimer selon vos besoins.

############################# Steps ############################
steps:
    enable: true
    title: "Étapes pour générer et insérer un code-barres dans XLSX"
    content: |
      [GroupDocs.Signature](/signature/python-net/) vous permet de générer et d'intégrer rapidement des codes-barres dans des documents XLSX. Prise en charge de plus de 60 formats de codes-barres, les applications Python via .NET peuvent ajouter sans problème la fonctionnalité de signature de code-barres en intégrant notre bibliothèque.
      
      1. Fournissez le fichier ou le flux XLSX pour le traitement.
      2. Assignez le texte du code-barres à l'objet BarcodeSignOptions.
      3. Ajustez les options du code-barres, telles que la position et la taille.
      4. Enregistrez le document avec le code-barres intégré.
   
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

            # Initialisez l'objet Signature avec le chemin du document
            with sg.Signature('input.xlsx') as signature:

                # Utilisez BarcodeSignOptions pour ajouter un code-barres au document
                options = sg.BarcodeSignOptions('Business data')

                # Définissez le type de code-barres et configurez ses propriétés
                options.EncodeType = sg.BarcodeTypes.Code128
                options.Left = 50
                options.Top = 150

                # Enregistrez le document signé
                result = signature.Sign('output.xlsx', options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Améliorez vos documents avec des fonctionnalités avancées de signature"
  description: "La bibliothèque GroupDocs.Signature for Python via .NET fournit des solutions complètes pour signer et traiter des documents dans des formats couramment utilisés. Vous pouvez facilement ajouter, modifier, vérifier ou supprimer différents types de signatures pour répondre à vos besoins."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Signature de documents flexible"
      content: "Signez n'importe quelle page dans des documents pris en charge avec du texte, des images, des codes-barres, des codes QR ou des tampons. Ajoutez des métadonnées cachées comme les données EXIF dans les images et garantissez la protection du contenu avec des certificats numériques pour prévenir les modifications non autorisées."

    # feature loop
    - title: "Recherchez et vérifiez les signatures"
      content: "Notre outil garantit l'intégrité de vos documents en permettant la vérification des signatures. Vous pouvez également récupérer une liste complète de toutes les signatures dans un document pour une gestion facile."

    # feature loop
    - title: "Modifiez les signatures facilement"
      content: "Modifiez les signatures existantes sans effort. Ajustez le texte, repositionnez les éléments ou changez les couleurs pour correspondre aux besoins de votre document."

    # feature loop
    - title: "Supprimez les signatures sans effort"
      content: "Avec une fonctionnalité CRUD complète, GroupDocs.Signature for Python via .NET facilite la suppression de toutes les signatures indésirables ou obsolètes de vos documents."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Créer et placer une signature de code-barres"
      content: |
        Cet exemple montre comment insérer un code-barres personnalisé dans un document XLSX.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Fournissez le document à signer
              with sg.Signature('input.xlsx') as signature:

                  # Définissez le texte du code-barres et les options de signature
                  options = sg.BarcodeSignOptions('Accepted')
                  options.EncodeType = sg.BarcodeTypes.Code39FullASCII

                  # Choisissez la position du code-barres sur la page
                  options.VerticalAlignment = sg.VerticalAlignment.Top
                  options.HorizontalAlignment = sg.HorizontalAlignment.Left

                  # Définissez l'espacement entre le code-barres et le bord de la page
                  options.Margin = sg.Padding()
                  options.Margin.Top = 180
                  options.Margin.Right = 20

                  # Spécifiez la couleur des barres du code-barres
                  options.ForeColor = sg.Color.Red

                  # Choisissez le style de police pour le message du code-barres
                  options.Font = sg.SignatureFont()
                  options.Font.Size = 12
                  options.Font.FamilyName = 'Arial'

                  # Définissez la position du texte du message
                  options.CodeTextAlignment = sg.CodeTextAlignment.Above

                  # Signez et enregistrez le document
                  result = signature.Sign('output.xlsx', options)
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
            link: "/examples/signature/formats/signature_barcode.xlsx"
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
    title: "Découvrez nos fonctionnalités clés"
    exclude: "barcode"
    description: "Nous offrons un large éventail d'options et d'opérations de signature pour vos besoins documentaires."
    items: 
          
        # operation loop 1
        - name: "Signatures électroniques"
          operation: "esign"
          link: "/signature/python-net/esign/xlsx/"
          description: "Ajoutez différents types de signatures aux formats de fichier pris en charge"

        # operation loop 2
        - name: "Ajouter du texte aux documents"
          operation: "text"
          link: "/signature/python-net/text/xlsx/"
          description: "Améliorez le contenu du document avec des signatures textuelles personnalisables"

        # operation loop 3
        - name: "Signatures d'image"
          operation: "image"
          link: "/signature/python-net/image/xlsx/"
          description: "Placez n'importe quelle image à n'importe quelle position dans un document"

        # operation loop 4
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/signature/python-net/barcode/xlsx/"
          description: "Créez et insérez divers codes-barres dans les documents pris en charge"

        # operation loop 5
        - name: "Générer des QR codes"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Générez des QR Codes, y compris des codes QR, pour la signature de documents"
          
        # operation loop 6
        - name: "Certificats numériques"
          operation: "digital"
          link: "/signature/python-net/digital/xlsx/"
          description: "Sécurisez les affaires et signez des documents avec des certificats numériques"

        # operation loop 7
        - name: "Tampons"
          operation: "stamp"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Utilisez le constructeur de tampons pour créer des tampons ronds ou carrés personnalisés"
          
        # operation loop 8
        - name: "Rechercher des signatures"
          operation: "search"
          link: "/signature/python-net/search/xlsx/"
          description: "Trouvez toutes les signatures précédemment ajoutées dans un document"
          
        # operation loop 9
        - name: "Vérification des signatures"
          operation: "verify"
          link: "/signature/python-net/verify/xlsx/"
          description: "Vérifiez l'authenticité des signatures après qu'elles aient été appliquées"
          
        # operation loop 10
        - name: "Modifier les signatures"
          operation: "modify"
          link: "/signature/python-net/modify/xlsx/"
          description: "Modifiez facilement une variété de signatures dans un document"
          
        # operation loop 11
        - name: "Supprimer les signatures"
          operation: "delete"
          link: "/signature/python-net/delete/xlsx/"
          description: "Retirez une large gamme de signatures précédemment appliquées"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Signez des documents dans plusieurs formats"
    exclude: "XLSX"
    description: "L'API Python via .NET prend en charge la signature de plus de 60 formats de fichiers, vous permettant d'ajouter divers types de signatures à n'importe quelle page ou emplacement spécifique dans vos documents."
    items: 
          
        # format loop 1
        - name: "Ajouter un code-barres au PDF"
          format: "PDF"
          link: "/signature/python-net/barcode/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Ajouter un code-barres au DOCX"
          format: "DOCX"
          link: "/signature/python-net/barcode/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 3
        - name: "Ajouter un code-barres au JPEG"
          format: "JPEG"
          link: "/signature/python-net/barcode/jpeg/"
          description: "Image JPEG"
          
        # format loop 4
        - name: "Ajouter un code-barres au PPTX"
          format: "PPTX"
          link: "/signature/python-net/barcode/pptx/"
          description: "Présentation Open XML de PowerPoint"
          
        # format loop 5
        - name: "Ajouter un code-barres au XLSX"
          format: "XLSX"
          link: "/signature/python-net/barcode/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"


          

---