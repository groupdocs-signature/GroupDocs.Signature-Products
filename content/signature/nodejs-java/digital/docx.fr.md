



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:18
draft: false
lang: fr
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Ajouter des signatures électroniques numériques à un fichier DOCX avec JavaScript"
head_description: "Apposez une signature numérique sur un fichier DOCX à l'aide de JavaScript en quelques lignes de code. Utilisez GroupDocs.Signature for Node.js via Java pour signer de nombreux formats de fichiers."

############################# Header ############################
title: "Protégez DOCX avec des certificats numériques" 
description: "Assurez la sécurité de vos documents professionnels en intégrant des certificats numériques grâce aux fonctionnalités avancées de GroupDocs.Signature for Node.js via Java. Nous proposons des options flexibles pour protéger et authentifier vos documents."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger gratuitement"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "À propos de GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) est une solution de signature complète conçue pour répondre à divers besoins de traitement de documents. Elle vous permet d'incorporer du texte, des images, des certificats numériques et des timbres dans plus de 60 formats de fichiers différents, notamment PDF, MS Office, images et fichiers ZIP. De plus, les documents signés peuvent être facilement recherchés, vérifiés, modifiés ou supprimés si nécessaire.

############################# Steps ############################
steps:
    enable: true
    title: "Guide pour sécuriser DOCX avec des certificats numériques en JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) permet aux développeurs Node.js via Java de protéger les documents DOCX contre les modifications en utilisant des signatures numériques. Améliorez vos applications professionnelles avec des fonctionnalités complètes de sécurité des données.
      
      1. Passez le document DOCX au constructeur de la classe Signature.
      2. Appliquez un certificat numérique et son mot de passe correspondant pour sécuriser le document.
      3. Optionnellement, ajoutez une représentation visuelle de la signature numérique sur les pages du document.
      4. Signez le document pour empêcher toute modification future.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Signatures d'exemple"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // Utilisez Signature pour appliquer une signature numérique au document
        const signature = new signatureLib.Signature('input.docx');

        // Fournissez le certificat numérique requis et le mot de passe
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // Configurez les paramètres de signature visuelle si nécessaire
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);
        
        // Chiffrez le document à l'aide du certificat numérique
        const result = signature.sign('output.docx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Optimisez ou sécurisez le contenu de vos documents avec des signatures"
  description: "GroupDocs.Signature for Node.js via Java est conçu pour signer tous les principaux formats de fichiers, vous offrant la possibilité d'ajouter, d'ajuster, de vérifier ou de supprimer divers types de signatures."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Signature"
  features:
    # feature loop
    - title: "Ajoutez des signatures à vos documents"
      content: "Placez facilement des signatures de type Texte, Image, Code-Barres, QR-Code ou Timbre sur n'importe quelle page de documents pris en charge. Vous pouvez également insérer ou modifier des métadonnées cachées, telles que les EXIF sur les images. Protégez le contenu de votre document contre des modifications non autorisées avec des certificats numériques."

    # feature loop
    - title: "Localisez et vérifiez les signatures"
      content: "Après la signature, votre document peut être soumis à plusieurs vérifications. Confirmez l'intégrité du contenu signé ou effectuez une recherche détaillée pour lister toutes les signatures existantes."

    # feature loop
    - title: "Révisez les signatures existantes"
      content: "La plupart des types de signatures permettent des modifications après leur création. Vous pouvez facilement modifier le texte, repositionner des éléments, ajuster les couleurs, redimensionner et apporter d'autres modifications nécessaires."

    # feature loop
    - title: "Éliminez les signatures inutiles"
      content: "Notre solution permet d'effectuer des opérations complètes CRUD pour les signatures. Si nécessaire, vous pouvez retirer différents types de signatures, y compris les certificats numériques, de votre document."
      
  code_samples:
    # code sample loop
    - title: "Protégez des documents avec des signatures numériques"
      content: |
        Découvrez comment verrouiller un document contre les modifications à l'aide de signatures numériques.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Fournissez le document qui nécessite une signature
        const signature = new signatureLib.Signature('input.docx');

        // Utilisez un certificat numérique approprié et son mot de passe
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // Incluez toute information textuelle supplémentaire
        options.setReason('Security issue');
        options.setContact('John Smith');
        options.setLocation('Office D.W.');

        // Ajoutez des éléments visuels comme des images pour la représentation de la signature
        options.setImageFilePath('image.png');
        options.setAllPages(true);
        options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
        options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        const padding = new signatureLib.Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);
        
        // Enregistrez le document numériquement sécurisé à un emplacement spécifié
        const result = signature.sign('output.docx', options);
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Prêt à commencer ?"
  description: "Essayez les fonctionnalités de GroupDocs.Signature gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "Téléchargement NPM"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Découvrez nos principales fonctions"
    exclude: "digital"
    description: "Nous supportons fièrement un ensemble complet d'options et de fonctionnalités de signature."
    items: 
          
        # operation loop 1
        - name: "Signatures électroniques"
          operation: "esign"
          link: "/signature/nodejs-java/esign/docx/"
          description: "Ajoutez différents types de signatures aux formats de fichier pris en charge"

        # operation loop 2
        - name: "Ajouter du texte aux documents"
          operation: "text"
          link: "/signature/nodejs-java/text/docx/"
          description: "Améliorez le contenu du document avec des signatures textuelles personnalisables"

        # operation loop 3
        - name: "Signatures d'image"
          operation: "image"
          link: "/signature/nodejs-java/image/docx/"
          description: "Placez n'importe quelle image à n'importe quelle position dans un document"

        # operation loop 4
        - name: "Générer des codes-barres"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "Créez et insérez divers codes-barres dans les documents pris en charge"

        # operation loop 5
        - name: "Générer des QR codes"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Générez des QR Codes, y compris des codes QR, pour la signature de documents"
          
        # operation loop 6
        - name: "Certificats numériques"
          operation: "digital"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Sécurisez les affaires et signez des documents avec des certificats numériques"

        # operation loop 7
        - name: "Tampons"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "Utilisez le constructeur de tampons pour créer des tampons ronds ou carrés personnalisés"
          
        # operation loop 8
        - name: "Rechercher des signatures"
          operation: "search"
          link: "/signature/nodejs-java/search/docx/"
          description: "Trouvez toutes les signatures précédemment ajoutées dans un document"
          
        # operation loop 9
        - name: "Vérification des signatures"
          operation: "verify"
          link: "/signature/nodejs-java/verify/docx/"
          description: "Vérifiez l'authenticité des signatures après qu'elles aient été appliquées"
          
        # operation loop 10
        - name: "Modifier les signatures"
          operation: "modify"
          link: "/signature/nodejs-java/modify/docx/"
          description: "Modifiez facilement une variété de signatures dans un document"
          
        # operation loop 11
        - name: "Supprimer les signatures"
          operation: "delete"
          link: "/signature/nodejs-java/delete/docx/"
          description: "Retirez une large gamme de signatures précédemment appliquées"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Signez des documents dans plusieurs formats"
    exclude: "DOCX"
    description: "L'API Node.js via Java prend en charge plus de 60 formats, vous permettant d'appliquer une gamme de signatures sur n'importe quelle page, d'assurer la sécurité du contenu avec des certificats numériques et de gérer efficacement les signatures dans le document."
    items: 
          
        # format loop 1
        - name: "Protéger le PDF"
          format: "PDF"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 2
        - name: "Protéger le DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 3
        - name: "Protéger le PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "Présentation Open XML de PowerPoint"
          
        # format loop 4
        - name: "Protéger le XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"


          

---