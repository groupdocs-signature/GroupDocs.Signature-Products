



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:46
draft: false
lang: it
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Aggiungi timbri a DOCX utilizzando Java"
head_description: "Sfrutta GroupDocs.Signature e Java per creare timbri personalizzati e posizionarli su qualsiasi pagina all'interno dei documenti DOCX."

############################# Header ############################
title: "Aggiungi timbri personalizzati a DOCX" 
description: "Progetta e applica timbri rotondi o quadrati a qualsiasi sezione dei tuoi documenti utilizzando GroupDocs.Signature for Java. La nostra soluzione offre ampie opzioni di personalizzazione per soddisfare tutte le tue esigenze aziendali."
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
    title: "Informazioni su GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) è uno strumento robusto che consente di aggiungere diverse firme timbrate ai documenti. Supporta oltre 60 formati di file diversi, inclusi PDF, Word, Excel, immagini e file ZIP. Puoi applicare firme di testo, immagini, codici a barre, metadati, certificati digitali e firme timbrate. Oltre ad aggiungere firme, puoi cercarle, verificarle, modificarle e rimuoverle.

############################# Steps ############################
steps:
    enable: true
    title: "Passaggi per aggiungere timbri a DOCX tramite Java"
    content: |
      [GroupDocs.Signature](/signature/java/) fornisce un costruttore di timbri che può essere estremamente vantaggioso per le applicazioni Java. Sfruttalo per creare timbri ben personalizzati per le pagine del tuo documento.
      
      1. Fornisci il documento DOCX da timbrare.
      2. Utilizza StampSignOptions per configurare tutti i parametri necessari.
      3. Aggiungi il numero di righe necessario.
      4. Applica il timbro e salva il documento.
   
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
        // Utilizza il percorso del documento con l'oggetto Signature
        Signature signature = new Signature("input.docx");

        // Instanzia StampSignOptions con il testo della firma desiderato
        StampSignOptions options = new StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // Aggiungi una o più righe di timbro
        StampLine outerLine = new StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(Color.WHITE);
        outerLine.setBackgroundColor(Color.BLUE);
        options.getOuterLines().add(outerLine);

        // Salva il documento timbrato
        SignResult result = signature.sign("output.docx", options);
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "Proteggi il contenuto dei tuoi documenti con firme"
  description: "La libreria GroupDocs.Signature for Java è progettata per firmare e gestire firme attraverso formati di file popolari. Aggiungi, modifica, verifica o rimuovi timbri e altri tipi di firme senza sforzo."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Firme Timbrate con GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firma i tuoi documenti"
      content: "Applica firme personalizzabili a qualsiasi parte del tuo documento. Scegli tra vari tipi di firma, inclusi testo, immagini, codici a barre, codici QR e timbri. Inoltre, possono essere aggiunti o modificati metadati nascosti per migliorare la sicurezza del documento."

    # feature loop
    - title: "Cerca e convalida le firme"
      content: "Una volta firmato un documento, utilizza i nostri strumenti di verifica per assicurarti che il contenuto della firma sia valido. Cerca e recupera un elenco di tutte le firme per ulteriori elaborazioni."

    # feature loop
    - title: "Aggiorna le firme secondo necessità"
      content: "Modifica facilmente un'ampia gamma di firme applicate a un documento. Aggiorna proprietà come dimensione, colore, posizione, contenuto e altro."

    # feature loop
    - title: "Rimuovi le firme"
      content: "Hai bisogno di rimuovere firme da un documento? La nostra API supporta completamente l'eliminazione delle firme, rendendo facile gestire i tuoi documenti in modo efficace."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Aggiungi timbri personalizzati ai documenti utilizzando firme speciali"
      content: |
        Scopri come generare e aggiungere timbri personalizzati con informazioni testuali importanti ai tuoi documenti.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Fornisci il documento da timbrare
          Signature signature = new Signature("input.docx");

          // Instanzia l'oggetto delle opzioni di timbratura
          StampSignOptions options = new StampSignOptions();

          // Imposta la dimensione e la posizione sulla pagina
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setAllPages(true);

          // Aggiungi una o più righe esterne rotonde con testo
          StampLine outerLine1 = new StampLine();
          outerLine1.setText("* The best  choice *");
          outerLine1.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
          SignatureFont signatureFont1 = new SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName("Arial");
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(Color.WHITE);
          outerLine1.setBackgroundColor(Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // Aggiungi una o più righe interne quadrate
          StampLine innerLine1 = new StampLine();
          innerLine1.setText("Company #1");
          innerLine1.setTextColor(Color.RED);
          SignatureFont signFont1 = new SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);

          // Salva il documento timbrato
          SignResult result = signature.sign("output.docx", options);
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
            link: "/examples/signature/formats/signature_stamp.docx"
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
    title: "Esplora le nostre funzionalità principali"
    exclude: "stamp"
    description: "Utilizza una vasta gamma di opzioni per aggiungere, gestire e eliminare firme."
    items: 
          
        # operation loop 1
        - name: "Firme elettroniche"
          operation: "esign"
          link: "/signature/java/esign/docx/"
          description: "Aggiungi vari tipi di firme ai formati di file supportati"

        # operation loop 2
        - name: "Aggiungi testo ai documenti"
          operation: "text"
          link: "/signature/java/text/docx/"
          description: "Migliora il contenuto del documento con firme testuali personalizzabili"

        # operation loop 3
        - name: "Firme con immagine"
          operation: "image"
          link: "/signature/java/image/docx/"
          description: "Posiziona qualsiasi immagine in qualsiasi punto di un documento"

        # operation loop 4
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/signature/java/barcode/docx/"
          description: "Crea e inserisci vari codici a barre nei documenti supportati"

        # operation loop 5
        - name: "Genera QR code"
          operation: "qrcode"
          link: "/signature/java/qrcode/docx/"
          description: "Genera e QR code, incluso QR code, per la firma dei documenti"
          
        # operation loop 6
        - name: "Certificati digitali"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "Proteggi documenti commerciali e firmali con certificati digitali"

        # operation loop 7
        - name: "Firme a timbro"
          operation: "stamp"
          link: "/signature/java/stamp/docx/"
          description: "Utilizza il Costruttore di Timbri per creare timbri personalizzati rotondi o quadrati"
          
        # operation loop 8
        - name: "Cerca firme"
          operation: "search"
          link: "/signature/java/search/docx/"
          description: "Trova qualsiasi firma precedentemente aggiunta all'interno di un documento"
          
        # operation loop 9
        - name: "Verifica delle firme"
          operation: "verify"
          link: "/signature/java/verify/docx/"
          description: "Verifica l'autenticità delle firme dopo che sono state applicate"
          
        # operation loop 10
        - name: "Modifica firme"
          operation: "modify"
          link: "/signature/java/modify/docx/"
          description: "Modifica facilmente una varietà di firme all'interno di un documento"
          
        # operation loop 11
        - name: "Elimina firme"
          operation: "delete"
          link: "/signature/java/delete/docx/"
          description: "Rimuovi un'ampia gamma di firme precedentemente applicate"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Aggiungi timbri su più formati di file"
    exclude: "DOCX"
    description: "L'API GroupDocs.Signature supporta la timbratura dei documenti in oltre 60 formati. Posiziona timbri su qualsiasi pagina o area per migliorare la gestione e la personalizzazione dei documenti."
    items: 
          
        # format loop 1
        - name: "Apponi timbro su PDF"
          format: "PDF"
          link: "/signature/java/stamp/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "Apponi timbro su DOCX"
          format: "DOCX"
          link: "/signature/java/stamp/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "Apponi timbro su JPEG"
          format: "JPEG"
          link: "/signature/java/stamp/jpeg/"
          description: "Immagine JPEG"
          
        # format loop 4
        - name: "Apponi timbro su PPTX"
          format: "PPTX"
          link: "/signature/java/stamp/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 5
        - name: "Apponi timbro su XLSX"
          format: "XLSX"
          link: "/signature/java/stamp/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---