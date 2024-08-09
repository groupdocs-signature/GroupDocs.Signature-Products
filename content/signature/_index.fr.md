---
############################# Static ############################
layout: "family"
date:  2024-07-25T14:25:12
draft: false

product: "Signature"
product_tag: "signature"

lang: fr

############################# Head ############################
head_title: "Applications de signature numérique C# .NET, Java, Node.js"
head_description: "Intégrez les signatures électroniques dans les applications .NET, Java ou Node.js avec GroupDocs.Signature. Signez les formats de documents commerciaux les plus courants."

############################# Header ############################
title: "Solution de signature électronique de documents"
description:  |
  Signez des documents et des images numériques sur n'importe quelle plate-forme à l'aide de nos API flexibles et de nos solutions basées sur des applications pour les programmeurs et les utilisateurs finaux.

  Recherchez et modifiez les signatures précédemment ajoutées à l'aide de méthodes avancées.

  Protégez les documents des modifications grâce aux certificats numériques et contrôlez les métadonnées cachées.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Choisissez votre plateforme"
  title: "Indépendance de la plateforme"
  description: "La bibliothèque GroupDocs.Signature prend en charge les systèmes d'exploitation et les frameworks suivants :"
  details_link_title: "Apprendre encore plus"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Signature .NET 
      color: "blue"
      tag: "net"
      link: "/signature/net/"
      features_link: "https://docs.groupdocs.com/signature/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.6.2 or higher <br> .NET Core 3.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS <br> Microsoft Azure
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Signature Java
      color: "red"
      tag: "java"
      link: "/signature/java/"
      features_link: "https://docs.groupdocs.com/signature/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 8 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Signature Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/signature/nodejs-java/"
      features_link: "https://docs.groupdocs.com/signature/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Tout autre éditeur de texte
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Signature fonctionnalités clés"
  description: "Notre solution est conçue pour ajouter différents types de signatures aux formats de documents et de fichiers courants. Enrichissez facilement vos processus métier."

  items:
    # items loop
    - icon: "additional"
      title: "Enrichissez vos données avec des signatures"
      content: "Ajoutez du texte, des images, des filigranes, etc. à vos documents professionnels."

    # items loop
    - icon: "protect"
      title: "Protéger le contenu des documents"
      content: "Interdisez les modifications de documents en les scellant avec un certificat numérique."

    # items loop
    - icon: "search"
      title: "Ajouter des données cachées et des codes-barres"
      content: "Utilisez des métadonnées pour stocker des informations invisibles ou insérer des codes-barres personnalisés sur les pages."

    # items loop
    - icon: "manipulate"
      title: "Manipuler les signatures"
      content: "Recherchez, mettez à jour ou supprimez toutes les signatures ajoutées précédemment."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Protégez vos fichiers à l'aide de signatures"
  description: "GroupDocs.Signature exemples de code"
  items:
    # code sample loop
    - title: "Générer et ajouter un code QR"
      content: |
       GroupDocs.Signature nous permet de générer et d'ajouter des codes QR aux documents aux formats pris en charge. Fournissez le chemin d’accès à un document qui doit être signé et configurez le texte souhaité et les options visuelles du code QR. Vous pouvez placer l'image du code QR générée sur n'importe quelle zone de n'importe quelle page de document.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Préciser le document à signer
            using (Signature signature = new Signature("source.docx"))
            {
                // Créer des options de signe de code QR
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // Définir les options du code QR
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150,
                };

                // Signer et enregistrer le fichier traité
                SignResult result = signature.Sign("result.docx", options);
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Préciser le document à signer
            Signature signature = new Signature("source.docx");

            // Créer des options de signe de code QR
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith");

            // Définir les options du code QR
            options.setEncodeType(QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Signer et enregistrer le fichier traité
            signature.sign("result.docx", options);
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            const signatureLib = require('@groupdocs/groupdocs.signature')

            // Préciser le document à signer
            const signature = new signatureLib.Signature('source.docx');

            // Créer des options de signe de code QR
            const options = new signatureLib.QrCodeSignOptions('JohnSmith');

            // Définir les options du code QR
            options.setEncodeType(signatureLib.QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Signer et enregistrer le fichier traité
            signature.sign('result.docx', options);
            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "Plus de 60 formats de fichiers sont pris en charge"
  description: "GroupDocs.Signature prend en charge presque tous les formats de fichiers courants"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Données statistiques de notre bibliothèque"
  description: "Inspectez les indicateurs clés des produits, révélant des informations sur nos réalisations, notre impact et notre croissance"

  items:
    # items loop
    - number: "50+"
      title: "Formats pris en charge"
      content: "Signature de plus de 60 formats de fichiers professionnels parmi les plus populaires."

    # items loop
    - number: "500k"
      title: "Téléchargements NuGet"
      content: "GroupDocs.Signature pour .NET est une bibliothèque populaire avec plus de 550 000 téléchargements sur NuGet."

    # items loop
    - number: "15k"
      title: "Téléchargements Maven"
      content: "Les développeurs Java ont téléchargé GroupDocs.Signature sur Maven plus de 15 000 fois."

    # items loop
    - number: "140+"
      title: "Clients satisfaits"
      content: "Des développeurs individuels et de grandes entreprises du monde entier utilisent nos produits pour créer des solutions innovantes."


############################# Customers ###############################
customers:
  enable: true
  title: "Nos clients satisfaits"
  description: "Les bibliothèques GroupDocs sont utilisées par des marques de renommée mondiale et distinguées à travers le monde"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Prêt à commencer?"
  description: "Essayez les fonctionnalités de GroupDocs.Signature gratuitement sur votre plateforme"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/signature/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/signature/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/signature/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "Questions fréquemment posées"
  description: "Explorez notre foire aux questions"

  items:
    # items loop
    - question: "GroupDocs.Signature a-t-il besoin d'une bibliothèque externe pour la signature de documents ?"
      answer: "Non, GroupDocs.Signature fonctionne de manière indépendante. Il n'y a pas de dépendances tierces comme Adobe Acrobat, Microsoft Office, etc."

    # items loop
    - question: "Est-il possible de tester les fonctionnalités de GroupDocs.Signature avant d'acheter ?"
      answer: "Absolument! GroupDocs.Signature propose un essai gratuit. Installez-le et explorez ses fonctionnalités. Notez que les versions d'essai ajoutent des « badges d'essai » à vos documents et ne traitent que les 3 premières pages. Pour une expérience complète, obtenez une licence temporaire gratuite de 30 jours pour accéder à toutes les fonctionnalités. Voir les détails sous [licence temporaire](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Quels types de licences sont proposés ?"
      answer: "Vous recherchez une licence GroupDocs.Signature ? Nous vous proposons différentes options adaptées à vos besoins. Choisissez en fonction de la taille de l'équipe, des emplacements de déploiement (bureau unique ou lieux de travail distants) et si la distribution au client final nécessite le partage du SDK/API avec les clients. Vous pouvez également opter pour une licence d’utilisation mensuelle avec des forfaits payants : ne payez que pour ce que vous utilisez. Découvrez la solution qui vous convient le mieux sous [pricing](https://purchase.groupdocs.com/pricing/signature/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Signature API low-code"
  description: "Signez des fichiers à l'aide de votre application via notre API REST basée sur le cloud."
  
  items:
    # items loop
    - title: "GroupDocs.Signature Cloud for cURL"
      content: "Utilisez l'API cURL RESTful pour apposer des signatures sur PDF, Word, Excel, PowerPoint, JPEG et de nombreux autres formats de fichiers."
      icon: "groupdocs_signature-for-curl"
      link: "https://products.groupdocs.cloud/signature/curl"

    # items loop
    - title: "GroupDocs.Signature Cloud for .NET"
      content: "Enrichissez vos applications .NET avec la signature de documents via Cloud SDK. Protégez les documents professionnels à votre manière."
      icon: "groupdocs_signature-for-net"
      link: "https://products.groupdocs.cloud/signature/net"

    # items loop
    - title: "GroupDocs.Signature Cloud for Java"
      content: "Le SDK GroupDocs.Signature donne accès à diverses possibilités permettant à vos applications Java de signer n'importe quel fichier."
      icon: "groupdocs_signature-for-java"
      link: "https://products.groupdocs.cloud/signature/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Signature Applications Web"
  description: "GroupDocs.Signature présente une application Web gratuite où vous pouvez signer des documents. Plus de 60 formats de fichiers populaires peuvent être signés GRATUITEMENT via votre navigateur préféré."

  items:
    # items loop
    - title: "GroupDocs.Signature Total"
      content: "Outil en ligne pour apposer des signatures sur des documents depuis n'importe quel appareil."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/signature/total"

    # items loop
    - title: "GroupDocs.Signature DOCX"
      content: "Signez MS Word DOCX en ligne."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/signature/docx"

    # items loop
    - title: "GroupDocs.Signature PDF"
      content: "Protégez les documents PDF en ligne."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/signature/pdf"


      


---