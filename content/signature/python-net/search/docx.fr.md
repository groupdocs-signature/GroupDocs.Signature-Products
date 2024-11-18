



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:14
draft: false
lang: fr
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Recherche de signatures électroniques pour DOCX utilisant Python"
head_description: "Exploitez l'API GroupDocs.Signature for Python via .NET pour rechercher des signatures électroniques intégrées dans des formats tels que PDF, Word, Excel, présentations et images."

############################# Header ############################
title: "Recherche de signatures numériques DOCX" 
description: "Extrayez une liste complète de signatures électroniques à partir de plusieurs formats, y compris PDF, Word, Excel, présentations et images, grâce à GroupDocs.Signature for Python via .NET."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargez maintenant"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Déployez le potentiel de GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "En savoir plus"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) offre des capacités avancées pour signer et gérer des documents numériques. Avec le support de plus de 60 formats de fichiers, y compris PDF, documents Office, images et fichiers ZIP, vous pouvez ajouter, rechercher, vérifier, modifier ou supprimer des signatures telles que du texte, des images, des codes-barres, des QR codes, des certificats numériques et des tampons.

############################# Steps ############################
steps:
    enable: true
    title: "Comment rechercher des signatures dans DOCX en utilisant Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) fournit un moteur puissant pour détecter les signatures numériques dans les fichiers DOCX. Les développeurs Python via .NET peuvent facilement enrichir leurs applications avec cette fonctionnalité.
      
      1. Fournissez le chemin du fichier DOCX pour la recherche de signature.
      2. Utilisez SearchOptions pour affiner les critères de recherche.
      3. Appelez la méthode Search pour récupérer les résultats.
      4. Examinez la liste des signatures identifiées.
   
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

            # Initialisez un objet Signature avec le chemin d'accès du fichier du document
            with sg.Signature('input.docx') as signature:

                # Créez une instance de TextSearchOptions pour rechercher sur toutes les pages
                options = sg.TextSearchOptions()
                options.AllPages = True

                # Effectuez une recherche pour localiser toutes les signatures basées sur du texte dans le document
                signatures = signature.Search(options)
                print("\nSource document contains following text signature(s).")

                # Compilez une liste de signatures trouvées pour un examen détaillé
                for textSignature in signatures:
                    print("\nFound Text signature at page ", textSignature.PageNumber)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Une plateforme complète de signature de documents"
  description: "Découvrez une solution de signature puissante et riche en fonctionnalités qui sécurise vos documents avec plusieurs types de signatures, couvrant divers formats de fichiers."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Rechercher et gérer les signatures"
  features:
    # feature loop
    - title: "Signer et sécuriser des documents commerciaux"
      content: "Ajoutez des signatures électroniques n'importe où dans un document. GroupDocs.Signature prend en charge plusieurs types de signatures, y compris du texte, des images, des codes-barres, des métadonnées, des tampons et des certificats numériques, garantissant l'authenticité et la sécurité du document."

    # feature loop
    - title: "Gestion complète des signatures"
      content: "Une fois qu'un document est signé, utilisez la fonction de recherche pour trouver toutes les signatures intégrées. Vous pouvez modifier ou supprimer des signatures selon les besoins, vous donnant un contrôle total sur l'intégrité du document."

    # feature loop
    - title: "Assurez l'intégrité du document"
      content: "Utilisez des outils avancés pour gérer les métadonnées cachées au sein des documents. Ajoutez ou supprimez des métadonnées et appliquez des certificats numériques pour protéger vos documents contre les modifications non autorisées, garantissant leur authenticité."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Rechercher des signatures d'image"
      content: |
        Cet exemple démontre comment trouver une signature d'image dans un document spécifique.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Passez le document source au constructeur
              with sg.Signature('input.docx') as signature:

                    # Recherchez toutes les signatures basées sur du texte
                    signatures = signature.Search(sg.SignatureType.Image)
                    print("\nSource document contains following image signature(s).")

                    # Affichez les propriétés détaillées des signatures identifiées
                    for imageSignature in signatures:
                        print("\nFound image signature at page ", imageSignature.PageNumber)
          ```
        platform: "python-net"
        copy_title: "Copier"
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
    title: "Fonctionnalités principales"
    exclude: "search"
    description: "Notre API offre une flexibilité étendue, permettant aux utilisateurs de signer des documents et d'effectuer des opérations après signature telles que la recherche, la vérification et l'édition des signatures."
    items: 
          
        # operation loop 1
        - name: "Signatures électroniques"
          operation: "esign"
          link: "/signature/python-net/esign/docx/"
          description: "Ajoutez différents types de signatures aux formats de fichier pris en charge"

        # operation loop 2
        - name: "Ajouter du texte aux documents"
          operation: "text"
          link: "/signature/python-net/text/docx/"
          description: "Améliorez le contenu du document avec des signatures textuelles personnalisables"

        # operation loop 3
        - name: "Signatures d'image"
          operation: "image"
          link: "/signature/python-net/image/docx/"
          description: "Placez n'importe quelle image à n'importe quelle position dans un document"

        # operation loop 4
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/signature/python-net/barcode/docx/"
          description: "Créez et insérez divers codes-barres dans les documents pris en charge"

        # operation loop 5
        - name: "Générer des QR codes"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/docx/"
          description: "Générez des QR Codes, y compris des codes QR, pour la signature de documents"
          
        # operation loop 6
        - name: "Certificats numériques"
          operation: "digital"
          link: "/signature/python-net/digital/docx/"
          description: "Sécurisez les affaires et signez des documents avec des certificats numériques"

        # operation loop 7
        - name: "Tampons"
          operation: "stamp"
          link: "/signature/python-net/stamp/docx/"
          description: "Utilisez le constructeur de tampons pour créer des tampons ronds ou carrés personnalisés"
          
        # operation loop 8
        - name: "Rechercher des signatures"
          operation: "search"
          link: "/signature/python-net/search/docx/"
          description: "Trouvez toutes les signatures précédemment ajoutées dans un document"
          
        # operation loop 9
        - name: "Vérification des signatures"
          operation: "verify"
          link: "/signature/python-net/verify/docx/"
          description: "Vérifiez l'authenticité des signatures après qu'elles aient été appliquées"
          
        # operation loop 10
        - name: "Modifier les signatures"
          operation: "modify"
          link: "/signature/python-net/modify/docx/"
          description: "Modifiez facilement une variété de signatures dans un document"
          
        # operation loop 11
        - name: "Supprimer les signatures"
          operation: "delete"
          link: "/signature/python-net/delete/docx/"
          description: "Retirez une large gamme de signatures précédemment appliquées"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Extraire des signatures de plusieurs formats de fichiers"
    exclude: "DOCX"
    description: "L'API GroupDocs.Signature for Python via .NET vous permet d'extraire et de gérer des signatures à partir d'une grande variété de formats de documents. Récupérez facilement les signatures intégrées des principaux types de fichiers pour une analyse ou un traitement ultérieur."
    items: 
          
        # format loop 1
        - name: "Rechercher des signatures dans le PDF"
          format: "PDF"
          link: "/signature/python-net/search/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Rechercher des signatures dans le DOCX"
          format: "DOCX"
          link: "/signature/python-net/search/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 3
        - name: "Rechercher des signatures dans le PPTX"
          format: "PPTX"
          link: "/signature/python-net/search/pptx/"
          description: "Présentation Open XML de PowerPoint"
          
        # format loop 4
        - name: "Rechercher des signatures dans le XLSX"
          format: "XLSX"
          link: "/signature/python-net/search/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"


          

---