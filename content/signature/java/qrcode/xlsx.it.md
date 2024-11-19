



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:20
draft: false
lang: it
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Crea codice QR per XLSX con Java"
head_description: "L'API di GroupDocs.Signature consente la generazione di codici QR per file XLSX. Crea codici QR dai tuoi contenuti e posizionali su qualsiasi pagina."

############################# Header ############################
title: "Crea codici QR per XLSX" 
description: "Crea codici a barre 2D con dati testuali e numerici e posizionali su qualsiasi pagina di vari documenti utilizzando GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Prova gratuita"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Scopri di più su GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) offre un'ampia gamma di funzionalità per generare e incorporare vari tipi di firme in tutti i principali formati di documento. Supporta PDF, documenti Word, fogli di calcolo Excel, presentazioni PowerPoint e immagini. Migliora i tuoi documenti con firme Testo, Immagine, Codice a barre, QR Code, Metadati, Digitale e Timbro.

############################# Steps ############################
steps:
    enable: true
    title: "Passaggi per generare e posizionare un codice QR in qualsiasi posizione in un XLSX"
    content: |
      [GroupDocs.Signature](/signature/java/) può generare codici QR in molti formati popolari e posizionarli sulle pagine XLSX. Sono supportati oltre 10 tipi di codici QR che possono essere rapidamente integrati nelle applicazioni Java. Usa il nostro prodotto per firmare documenti con codici QR generati.
      
      1. Ottieni il file o lo stream XLSX da firmare con un codice QR.
      2. Fornisci il testo per QrCodeSignOptions.
      3. Personalizza le opzioni visive come colore, posizione, dimensioni, ecc.
      4. Salva il file con il codice QR.
   
    code:
      platform: "java"
      copy_title: "Copia"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Firme di esempio"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // Passa il documento a una nuova istanza di Signature
        Signature signature = new Signature("input.xlsx");

        // Utilizza QrCodeSignOptions per aggiungere un codice QR al documento
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // Specifica il tipo di firma e la posizione sulla pagina
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // Salva il file con il codice QR aggiunto
        signature.sign("output.xlsx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Aggiungi firme ai tuoi documenti"
  description: "L'API di GroupDocs.Signature for Java supporta la firma di tutti i formati di file popolari. Genera, modifica, cerca, verifica e rimuovi diversi tipi di firme."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firma documenti"
      content: "GroupDocs.Signature supporta la firma con firme Testo, Immagine, Codice a barre, QR Code e Timbro. Posizionali su qualsiasi pagina di qualsiasi formato di documento supportato. Gestisci i metadati del documento con firme di metadati e proteggi il contenuto da modifiche non autorizzate utilizzando certificati digitali."

    # feature loop
    - title: "Ricerca e verifica"
      content: "Assicurati che tutte le firme di un documento siano valide tramite la procedura di verifica. Recupera un elenco completo delle firme contenute in un documento utilizzando la funzione di ricerca integrata."

    # feature loop
    - title: "Modifica firme"
      content: "Modifica facilmente le proprietà delle firme dopo la firma. Regola contenuto, posizione, colore, dimensioni e altri attributi secondo necessità."

    # feature loop
    - title: "Rimuovi firme"
      content: "Elimina firmate indesiderate senza difficoltà. Vari tipi di firme, inclusi i certificati digitali, possono essere rimossi programmaticamente dai documenti."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Come personalizzare un codice QR generato"
      content: |
        Utilizza questo esempio per imparare a posizionare un nuovo codice QR su una pagina XLSX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Ottieni il documento da firmare e passalo a Signature
          Signature signature = new Signature("input.xlsx");

          // Utilizza le opzioni del codice QR per fornire il testo con le informazioni richieste
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // Imposta la posizione relativa del codice QR sulla pagina
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // Imposta il padding della firma
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Specifica il colore del codice QR
          signOptions.setForeColor(Color.RED);

          // Definisci le opzioni di font per il messaggio
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Personalizza il colore di sfondo e del pennello del codice QR
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Aggiungi il codice QR al documento
          SignResult signResult = signature.sign("output.xlsx", signOptions);
          ```
        platform: "java"
        copy_title: "Copia"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "clicca per copiare"
          copy_done: "copiato"
        top_links:
          #  loop
          - title: "Scarica il risultato"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.xlsx"
        links:
          #  loop
          - title: "Altri esempi"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Documentazione"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Prova gratuitamente le funzionalità di GroupDocs.Signature o richiedi una licenza."
  items:
    #  loop
    - title: "Download di Maven"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "Licenze"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Scopri le nostre principali offerte"
    exclude: "qrcode"
    description: "Offriamo una selezione diversificata di funzionalità di firma e operazioni avanzate."
    items: 
          
        # operation loop 1
        - name: "Firme elettroniche"
          operation: "esign"
          link: "/signature/java/esign/xlsx/"
          description: "Aggiungi vari tipi di firme ai formati di file supportati"

        # operation loop 2
        - name: "Aggiungi testo ai documenti"
          operation: "text"
          link: "/signature/java/text/xlsx/"
          description: "Migliora il contenuto del documento con firme testuali personalizzabili"

        # operation loop 3
        - name: "Firme con immagine"
          operation: "image"
          link: "/signature/java/image/xlsx/"
          description: "Posiziona qualsiasi immagine in qualsiasi punto di un documento"

        # operation loop 4
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/signature/java/barcode/xlsx/"
          description: "Crea e inserisci vari codici a barre nei documenti supportati"

        # operation loop 5
        - name: "Genera QR code"
          operation: "qrcode"
          link: "/signature/java/qrcode/xlsx/"
          description: "Genera e QR code, incluso QR code, per la firma dei documenti"
          
        # operation loop 6
        - name: "Certificati digitali"
          operation: "digital"
          link: "/signature/java/digital/xlsx/"
          description: "Proteggi documenti commerciali e firmali con certificati digitali"

        # operation loop 7
        - name: "Firme a timbro"
          operation: "stamp"
          link: "/signature/java/stamp/xlsx/"
          description: "Utilizza il Costruttore di Timbri per creare timbri personalizzati rotondi o quadrati"
          
        # operation loop 8
        - name: "Cerca firme"
          operation: "search"
          link: "/signature/java/search/xlsx/"
          description: "Trova qualsiasi firma precedentemente aggiunta all'interno di un documento"
          
        # operation loop 9
        - name: "Verifica delle firme"
          operation: "verify"
          link: "/signature/java/verify/xlsx/"
          description: "Verifica l'autenticità delle firme dopo che sono state applicate"
          
        # operation loop 10
        - name: "Modifica firme"
          operation: "modify"
          link: "/signature/java/modify/xlsx/"
          description: "Modifica facilmente una varietà di firme all'interno di un documento"
          
        # operation loop 11
        - name: "Elimina firme"
          operation: "delete"
          link: "/signature/java/delete/xlsx/"
          description: "Rimuovi un'ampia gamma di firme precedentemente applicate"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Genera codici QR per formati di file aggiuntivi"
    exclude: "XLSX"
    description: "Migliora tutti i formati di file popolari con codici QR generati utilizzando l'API Java. Aggiungi dati a codici a barre 2D per una facile scansione e elaborazione."
    items: 
          
        # format loop 1
        - name: "QR-Code per PDF"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "QR-Code per DOCX"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "QR-Code per JPEG"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "Immagine JPEG"
          
        # format loop 4
        - name: "QR-Code per PPTX"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 5
        - name: "QR-Code per XLSX"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---