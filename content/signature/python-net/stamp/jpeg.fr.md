



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:49
draft: false
lang: fr
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Créer des timbres ronds et carrés en JPEG utilisant Python"
head_description: "Générez et insérez des timbres personnalisés dans des fichiers JPEG avec l'API GroupDocs.Signature for Python via .NET."

############################# Header ############################
title: "Créer des timbres pour JPEG" 
description: "Ajoutez des timbres conçus sur mesure à n'importe quelle partie de vos documents avec GroupDocs.Signature for Python via .NET, offrant une grande flexibilité pour le placement et la configuration selon vos besoins professionnels."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger gratuitement"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Aperçu de GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "En savoir plus"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) est un outil complet qui vous permet d'insérer divers types de signatures dans des documents, y compris des timbres personnalisés. Prisant en charge plus de 60 formats de fichiers, allant des PDF et documents Word aux images et fichiers ZIP, vous pouvez améliorer vos documents avec du texte, des images, des codes-barres, des métadonnées, des certificats numériques et des timbres. Vous disposez également d'un contrôle total pour rechercher, vérifier, modifier ou supprimer toute signature appliquée.

############################# Steps ############################
steps:
    enable: true
    title: "Comment ajouter un timbre à JPEG en utilisant Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) fournit des outils robustes de création de timbres pour améliorer les applications Python via .NET. Utilisez-le pour concevoir et mettre en œuvre des timbres personnalisés pour les pages de votre document.
      
      1. Fournissez le document JPEG que vous souhaitez timbrer.
      2. Utilisez StampSignOptions pour configurer tous les paramètres nécessaires.
      3. Ajoutez plusieurs lignes de timbre si nécessaire.
      4. Appliquez le timbre et enregistrez le document mis à jour.
   
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

            # Attachez le chemin du document à l'instance Signature
            with sg.Signature('input.jpeg') as signature:

                # Configurez StampSignOptions avec les détails du timbre requis
                options = sg.StampSignOptions()
                options.Height = 180
                options.Width = 180

                # Ajoutez une ou plusieurs lignes au timbre
                outerLine = sg.StampLine()
                outerLine.Text = "* The Best Company *"
                outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                outerLine.Font = sg.SignatureFont()
                outerLine.Font.Size = 12
                outerLine.Font.FamilyName = "Arial"
                outerLine.Height = 22
                outerLine.TextBottomIntent = 6
                outerLine.TextColor = sg.Color.WhiteSmoke
                outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                options.OuterLines.Add(outerLine)

                # Enregistrez le document avec le timbre appliqué
                result = signature.Sign("output.jpeg", options)
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "Utilisez les signatures pour sécuriser et améliorer l'intégrité des documents"
  description: "Avec la bibliothèque GroupDocs.Signature for Python via .NET, vous pouvez ajouter sans effort des fonctionnalités de signature à vos documents. Créez, modifiez, vérifiez ou supprimez facilement des timbres personnalisés et d'autres types de signatures, offrant flexibilité et sécurité pour vos flux de travail documentaires."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Signatures de timbre alimentées par GroupDocs.Signature"
  features:
    # feature loop
    - title: "Signature complète des documents"
      content: "Élevez vos documents en ajoutant des signatures telles que texte, images, codes-barres, QR codes et timbres à n'importe quelle position sur n'importe quelle page. Gérez les métadonnées intégrées et appliquez des certificats numériques pour vous protéger contre les modifications non autorisées."

    # feature loop
    - title: "Recherche et vérification de signatures efficaces"
      content: "Après la signature, utilisez des outils de recherche avancés pour trouver toutes les signatures intégrées. Vérifiez facilement ou gérez les données de signature pour garantir l'intégrité des documents."

    # feature loop
    - title: "Modifier et personnaliser les signatures"
      content: "Apportez des modifications aux signatures ajoutées précédemment sans difficulté. Que vous souhaitiez changer le contenu, la position, la taille ou la couleur, GroupDocs.Signature for Python via .NET vous donne un contrôle total pour ajuster les signatures selon vos besoins."

    # feature loop
    - title: "Supprimer les signatures facilement"
      content: "Si vous devez supprimer des signatures, GroupDocs.Signature for Python via .NET offre tous les outils nécessaires pour supprimer tout type, y compris les timbres et certificats numériques, vous aidant à garder vos documents à jour et conformes."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Comment ajouter des timbres personnalisés aux documents"
      content: |
        Cet exemple montre comment créer et insérer des timbres personnalisés avec des détails de texte spécifiques dans un document.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Fournissez le document que vous souhaitez timbrer
              with sg.Signature('input.jpeg') as signature:

                    # Configurez les options de timbre avec vos paramètres souhaités
                    options = sg.StampSignOptions()

                    # Définissez la taille et le placement du timbre sur la page
                    options.Height = 200
                    options.Width = 200
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right
                    options.AllPages = True

                    # Ajoutez des lignes circulaires extérieures avec le texte
                    outerLine = sg.StampLine()
                    outerLine.Text = "* The best  choice *"
                    outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                    outerLine.Font = sg.SignatureFont()
                    outerLine.Font.Size = 12
                    outerLine.Font.FamilyName = "Arial"
                    outerLine.Height = 22
                    outerLine.TextBottomIntent = 6
                    outerLine.TextColor = sg.Color.WhiteSmoke
                    outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                    options.OuterLines.Add(outerLine)

                    # Ajoutez, si vous le souhaitez, des lignes carrées intérieures
                    innerLine = sg.StampLine()
                    innerLine.Text = "Company #1"
                    innerLine.TextColor = sg.Color.MediumVioletRed
                    innerLine.Font = sg.SignatureFont()
                    innerLine.Font.Size = 20
                    innerLine.Font.Bold = True
                    innerLine.Height = 40
                    options.InnerLines.Add(innerLine)

                    # Finalisez et enregistrez le document timbré
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
            link: "/examples/signature/formats/signature_stamp.jpeg"
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
    title: "Découvrez les fonctionnalités clés"
    exclude: "stamp"
    description: "Trouvez une large gamme d'options pour créer, gérer et supprimer des signatures, vous donnant un contrôle total sur les flux de travail documentaires."
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
    title: "Appliquez des timbres à divers formats de documents"
    exclude: "JPEG"
    description: "Avec l'API GroupDocs.Signature, vous pouvez insérer des timbres personnalisés dans plus de 60 types de fichiers standard. Appliquez facilement des timbres n'importe où dans vos documents, améliorant la personnalisation et le suivi."
    items: 
          
        # format loop 1
        - name: "Tamponner PDF"
          format: "PDF"
          link: "/signature/python-net/stamp/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Tamponner DOCX"
          format: "DOCX"
          link: "/signature/python-net/stamp/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 3
        - name: "Tamponner JPEG"
          format: "JPEG"
          link: "/signature/python-net/stamp/jpeg/"
          description: "Image JPEG"
          
        # format loop 4
        - name: "Tamponner PPTX"
          format: "PPTX"
          link: "/signature/python-net/stamp/pptx/"
          description: "Présentation Open XML de PowerPoint"
          
        # format loop 5
        - name: "Tamponner XLSX"
          format: "XLSX"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"


          

---