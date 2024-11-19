



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:08
draft: false
lang: it
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Aggiungere firme di immagini a file PDF con Java"
head_description: "Apponi la firma con immagine su file PDF per Java utilizzando poche righe di codice. Utilizza l'API GroupDocs.Signature for Java per aggiungere immagini."

############################# Header ############################
title: "Firma file PDF con firme di immagini" 
description: "Usa GroupDocs.Signature for Java per inserire immagini in vari formati di documenti d'ufficio, inclusi PDF, Word, Excel e file immagine. Un'immagine con la firma del tuo superiore può dare un tocco impressionante!"
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica gratuitamente"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Scopri GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) offre la possibilità di aggiungere firme di immagini a qualsiasi pagina e posizione all'interno dei documenti aziendali. Snellisci i tuoi flussi di lavoro aggiungendo immagini a PDF, documenti Word, fogli di calcolo Excel, presentazioni PowerPoint e formati di immagine popolari.

############################# Steps ############################
steps:
    enable: true
    title: "Passaggi per aggiungere un'immagine in qualsiasi posizione di un PDF tramite Java"
    content: |
      [GroupDocs.Signature](/signature/java/) migliora le applicazioni Java con la capacità di aggiungere firme a qualsiasi pagina di documenti PDF in modo preciso. Potenzia le funzionalità del tuo prodotto integrando la nostra libreria.
      
      1. Crea un'istanza di Signature con il documento PDF.
      2. Usa ImageSignOptions per specificare l'immagine della firma.
      3. Posiziona l'immagine in qualsiasi posizione di qualsiasi pagina.
      4. Salva il documento firmato in una nuova posizione.
   
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
        // Instantiate Signature con il percorso del documento
        Signature signature = new Signature("input.pdf");

        // Crea ImageSignOptions utilizzando un'immagine per la firma
        ImageSignOptions options = new ImageSignOptions("company_logo.jpg");

        // Posiziona l'immagine nell'angolo in alto a sinistra di tutte le pagine
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);

        // Salva il documento firmato
        SignResult result = signature.sign("output.pdf", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Soluzione completa per la firma dei documenti"
  description: "La nostra API supporta una gamma di funzionalità di firma, consentendoti di aggiungere, modificare, eliminare, cercare e verificare più tipi di firme, incluse le firme con immagine."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Firma delle immagini"
  features:
    # feature loop
    - title: "Inserisci immagini nei documenti d'ufficio"
      content: "Posiziona senza sforzo firme di immagine in qualsiasi posizione su qualsiasi pagina di un documento. Arricchisci il tuo contenuto con testo, immagini, codici a barre, metadati e certificati digitali."

    # feature loop
    - title: "Ricerca e verifica delle firme"
      content: "Verifica la validità delle firme nei documenti firmati. Recupera un elenco di tutte le firme all'interno di un documento e controlla le informazioni dettagliate su ciascuna di esse."

    # feature loop
    - title: "Modifica delle firme"
      content: "Aggiorna il contenuto, l'aspetto, la dimensione o la posizione di qualsiasi firma precedentemente aggiunta a un documento. La nostra API rende semplice e veloce la modifica delle firme."

    # feature loop
    - title: "Rimuovi firme non necessarie"
      content: "La nostra API supporta operazioni CRUD complete per la maggior parte dei tipi di firma. Puoi facilmente rimuovere firme da quasi tutti i tipi di documenti supportati quando necessario."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Migliora il contenuto del documento con firme di immagini"
      content: |
        Scopri come aggiungere immagini ai documenti aziendali per fornire informazioni aggiuntive.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Seleziona un documento da firmare
          Signature signature = new Signature("input.pdf");

          // Crea opzioni di immagine con il percorso dell'immagine
          ImageSignOptions options = new ImageSignOptions("manager_signature.jpg");

          // Imposta la dimensione della firma dell'immagine
          options.setWidth(100);
          options.setHeight(100);

          // Posiziona l'immagine nell'angolo in basso a destra
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);

          // Applica padding dagli angoli della pagina se necessario
          Padding padding = new Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // Aggiungi un bordo personalizzato all'immagine se desiderato
          Border border = new Border();
          border.setColor(Color.RED);
          border.setDashStyle(DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // Ruota la firma per un miglior allineamento
          options.setRotationAngle(45);

          // Salva il documento aggiornato in qualsiasi posizione
          SignResult result = signature.sign("output.pdf", options);

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
            link: "/examples/signature/formats/signature_image.pdf"
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
    title: "Scopri le nostre funzionalità principali"
    exclude: "image"
    description: "Siamo lieti di presentare una varietà di strumenti e operazioni per la firma."
    items: 
          
        # operation loop 1
        - name: "Firme elettroniche"
          operation: "esign"
          link: "/signature/java/esign/pdf/"
          description: "Aggiungi vari tipi di firme ai formati di file supportati"

        # operation loop 2
        - name: "Aggiungi testo ai documenti"
          operation: "text"
          link: "/signature/java/text/pdf/"
          description: "Migliora il contenuto del documento con firme testuali personalizzabili"

        # operation loop 3
        - name: "Firme con immagine"
          operation: "image"
          link: "/signature/java/image/pdf/"
          description: "Posiziona qualsiasi immagine in qualsiasi punto di un documento"

        # operation loop 4
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/signature/java/barcode/pdf/"
          description: "Crea e inserisci vari codici a barre nei documenti supportati"

        # operation loop 5
        - name: "Genera QR code"
          operation: "qrcode"
          link: "/signature/java/qrcode/pdf/"
          description: "Genera e QR code, incluso QR code, per la firma dei documenti"
          
        # operation loop 6
        - name: "Certificati digitali"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "Proteggi documenti commerciali e firmali con certificati digitali"

        # operation loop 7
        - name: "Firme a timbro"
          operation: "stamp"
          link: "/signature/java/stamp/pdf/"
          description: "Utilizza il Costruttore di Timbri per creare timbri personalizzati rotondi o quadrati"
          
        # operation loop 8
        - name: "Cerca firme"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "Trova qualsiasi firma precedentemente aggiunta all'interno di un documento"
          
        # operation loop 9
        - name: "Verifica delle firme"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "Verifica l'autenticità delle firme dopo che sono state applicate"
          
        # operation loop 10
        - name: "Modifica firme"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "Modifica facilmente una varietà di firme all'interno di un documento"
          
        # operation loop 11
        - name: "Elimina firme"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "Rimuovi un'ampia gamma di firme precedentemente applicate"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Aggiungi immagini ad altri formati di file"
    exclude: "PDF"
    description: "Con l'API Java, puoi inserire formati di immagine supportati in vari documenti. Ridimensiona, scegli la posizione e aggiungi firme con immagini ai tuoi documenti."
    items: 
          
        # format loop 1
        - name: "Firma PDF con immagine"
          format: "PDF"
          link: "/signature/java/image/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "Firma DOCX con immagine"
          format: "DOCX"
          link: "/signature/java/image/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "Firma JPEG con immagine"
          format: "JPEG"
          link: "/signature/java/image/jpeg/"
          description: "Immagine JPEG"
          
        # format loop 4
        - name: "Firma PPTX con immagine"
          format: "PPTX"
          link: "/signature/java/image/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 5
        - name: "Firma XLSX con immagine"
          format: "XLSX"
          link: "/signature/java/image/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---