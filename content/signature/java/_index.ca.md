---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API de signatura digital de Java, afegeix una signatura electrònica a la imatge PDF Word Excel"
head_description: "API de signatura digital de Java. Biblioteca de signatura electrònica per signar digitalment PDF, Microsoft Word, fulls de càlcul Excel, presentacions de PowerPoint i formats de documents d'imatge."

############################# Header ############################
title: "API de Java per gestionar signatures digitals"
description: "Gestioneu la signatura electrònica d'imatge, codi QR, codi de barres, metadades, text i tipus de segell en aplicacions Java per signar imatges i formats de fitxers de documents digitals."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Visió general"

            # button loop
            - link: "#features"
              text: "Característiques"

            # button loop
            - link: "#support"
              text: "Suport"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Demostració en directe"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Preus"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      L'API de GroupDocs.Signature per a Java us ajuda a desenvolupar aplicacions Java amb funcionalitat de signatures electròniques per signar documents digitals de formats compatibles sense instal·lar cap programari extern. Admet la manipulació i la gestió de diversos tipus de signatures electrònices com ara imatge, codi de barres, codi QR, segell, text, òptica i metadades. Tots els vostres documents de negoci electrònic com Microsoft Office Word, presentacions de PowerPoint, fulls de càlcul Excel, imatges i fitxers PDF es poden signar digitalment personalitzant les propietats de la signatura, p. ombra, dimensions, alineació i més segons els vostres requisits. La biblioteca de signatura digital és senzilla i lleugera, i consta d'un únic fitxer DLL que es pot integrar fàcilment dins d'una aplicació Java nova o existent.  

      Mitjançant l'API de GroupDocs.Signature per a Java, podeu carregar tots els certificats registrats del sistema o localitzar signatures existents mitjançant una cerca senzilla i avançada. Les opcions per treballar amb documents protegits amb contrasenya, especificant propietats de signatura comunes (mida del text, opacitat, rotació, verificació, propietats de tipus de lletra, opcions de color, número de pàgina, amplada, superior, esquerra, etc.) i el suport per implementar diferents tipus de signatura electrònica fan que sigui fiable. Solució de gestió de signatures electròniques per a documents digitals.  

      GroupDocs.Signature per a Java és compatible amb totes les versions de Java i és compatible amb els sistemes operatius populars (Windows, Linux, MacOS) que són capaços d'executar el temps d'execució de Java
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Aquesta és una visió general de les funcions de GroupDocs.Signature per a Java:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Tipus de signatura"
          content: |
            * Signatura de text
            * Signatura de la imatge
            * Signatures digitals
            * Signatura del codi QR
            * Signatura del codi de barres
            * Signatura del segell
            * Formulari-camp Signatura
      
      ## TAB TWO ##
      tab_two:
        description: |
          L'API de signatura electrònica de Java admet [formats de fitxer de document](https://docs.groupdocs.com/signature/java/supported-document-formats/) tal com s'indica a continuació.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Other Formats"
              content: |
                * **Imatges**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Metafitxers**: EMF, WMF, CMX
                * **Portàtil**: PDF
                * **Gràfics vectorials escalables**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Altres**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature per a Java admet els següents sistemes operatius, marcs i gestors de paquets:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Sistemes operatius"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Marcs suportats"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Entorns de desenvolupament"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Eina d'automatització de creació"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "Funcions de GroupDocs.Signature per a Java"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Creeu, llegiu, modifiqueu, amagueu i suprimiu signatures electròniques dels formats de document admesos"

      # feature loop
      - icon: "fas fa-eye"
        content: "Accés per signar el document des del corrent, camí relatiu o camí absolut"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Apliqueu la signatura de text a documents, fulls de càlcul, presentacions, imatges i fitxers PDF"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Afegiu la signatura de text com a anotació, adhesiu, imatge als fitxers PDF, també configureu l'estil i el color"

      # feature loop
      - icon: "fas fa-code"
        content: "Signeu un document PDF, un fitxer d'imatge i obteniu una sortida en un format de fitxer diferent"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Signa digitalment imatges amb la signatura de text com a marca d'aigua i afegeix transparència, rotació a la signatura electrònica"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Cerqueu certificats i signeu documents de Microsoft Word, Excel i PDF amb certificats digitals"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Signeu formats de document de processament de textos amb filigranes de text nadius"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Utilitzeu el codi QR, el codi de barres per signar fitxers de paraules, diapositives, cel·les, PDF i imatges"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Configureu i apliqueu signatures de segell per protegir els formats de fitxer admesos"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Configura i assigna signatures d'imatge a documents, fulls de càlcul, presentacions, imatges i fitxers PDF"

      # feature loop
      - icon: "fas fa-columns"
        content: "Configura les propietats de la signatura, per exemple, aspecte i sensació, marges, alineació, etc."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Apliqueu la signatura digital al document protegit amb contrasenya"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Realitzeu la verificació de text dels documents PDF mitjançant el gestor de signatures"

      # feature loop
      - icon: "fas fa-print"
        content: "Verificació digital de documents Word, Cell, PDF amb contenidors de certificats .CER i .PFX"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Especifiqueu diferents tipus d'unitats de mesura (per exemple, mil·límetres, píxels, etc.) per a signatures de text PDF"

      # feature loop
      - icon: "fas fa-lock"
        content: "Obteniu informació del document mitjançant fitxer o URL: afegiu signatures de camp de formulari als documents PDF"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Afegiu objecte de dades personalitzat, VCard incrustat, correu electrònic, EPC, MeCard o objecte d'esdeveniment al codi QR"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Apliqueu diferents estils de pinzell a les signatures, per exemple, pinzell degradat, radial, sòlid i de textura"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Signar el document Situat a FTP o Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Estableix l'alineació del text dins de les formes per a documents, diapositives, imatges i fitxers PDF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Cerca, verifica i signa digitalment documents de presentació de PowerPoint"

      # feature loop
      - icon: "fas fa-cube"
        content: "Col·loqueu la signatura amb píxels als documents de la cel·la i el posicionament del text per a les signatures de segell"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Implementeu la signatura de segell rectangular amb cantonades arrodonides"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Amplieu les signatures de codis de barres i codis QR amb contingut de dades d'imatge"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Afegiu signatures de metadades xifrades mentre treballeu amb les opcions de signatura i cerca"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Insereix objectes personalitzats a signatures de metadades dins de Word, Excel i presentacions"

    more_feature:
      # more_feature_loop
      - title: "Configureu i apliqueu signatures electrònices fàcilment"
        content: |
          L'API de GroupDocs.Signature per a Java permet configurar i afegir signatures electrònices als formats de document compatibles. A continuació es mostra un exemple de codi que mostra com de senzill és aplicar una signatura de text a un fitxer PDF:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // establir la posició de la signatura
          options.setLeft(100);
          options.setTop(100);
          
          // establir un rectangle de signatura
          options.setWidth(100);
          options.setHeight(30);

          // establir el color del text i el tipus de lletra
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // signar el document per arxivar
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Tipus de codificació de codi de barres compatibles per a la signatura electrònica"
        content: |
          Mitjançant l'API de GroupDocs.Signature per a Java, podeu aplicar signatures de codi de barres i codi QR als formats de fitxer compatibles. GroupDocs.Signature per a Java admet una gran varietat de tipus de codificació de codis de barres per satisfer la majoria de requisits. Els tipus de codificació de codis de barres admesos inclouen: Codi 11, Codi 128, Codi 16K/32, Codis de barres de dades, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard i Codi39 ampliat.

          De la mateixa manera, l'API de GroupDocs.Signature per a Java us permet utilitzar tipus de codi QR, com ara QR, Aztec i Data Matrix. Els tipus de codificació de codis QR admesos inclouen Aztec, DataMatrix, GS1 DataMatrix i GS1 QR.

      # more_feature_loop
      - title: "Cerca signatures i certificats"
        content: |
          Mitjançant l'API de GroupDocs.Signature per a Java, podeu cercar signatures de codi QR i codi de barres en qualsevol document, presentació, full de càlcul, imatge i fitxer PDF i obtenir el resultat de la cerca. També podeu cercar objectes de dades personalitzats a partir de documents signats amb la signatura de codi QR, així com cercar VCard estàndard i objectes de correu electrònic a partir de documents signats amb codi QR. També s'admet la verificació del text xifrat de les signatures del codi QR, així com la cerca de signatura de metadades en documents PDF. Apliqueu criteris de cerca addicionals per a signatures digitals de documents Words & Cells.  

          L'opció de cerca també està disponible per a la signatura de metadades per a documents de Word, diapositives i fulls de càlcul, mentre que la cerca de camp de formulari està disponible per a documents PDF.

      # more_feature_loop
      - title: "Configura les propietats de la signatura electrònica"
        content: |
          Per millorar la UX dels usuaris finals, l'API de GroupDocs.Signature for Java ofereix moltes propietats que es poden configurar amb força facilitat. Podeu definir les opcions de tipus de lletra i color (Color de fons, Color de primer pla, Negreta, Cursiva, Subratllat, Família de tipus de lletra, Mida de la lletra, etc.), Opcions de fons i vores (Color de fons, Transparència de fons, Color de vora, Estil de guió de vora, Pes de vora, Transparència de la vora, etc.), Marges de signatura (esquerra, superior, amplada, alçada, farciment, etc.) i Configuració de l'àrea de signatura de la imatge i alineació de la signatura (alineació horitzontal, alineació vertical, etc.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature ofereix API de visualització de documents per a altres entorns de desenvolupament populars"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---