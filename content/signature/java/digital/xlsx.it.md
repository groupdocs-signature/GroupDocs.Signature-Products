



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:16
draft: false
lang: it
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Aggiungere firme elettroniche digitali a file XLSX con Java"
head_description: "Apponi una firma digitale su un file XLSX utilizzando Java con poche righe di codice. Usa GroupDocs.Signature for Java per firmare numerosi formati di file."

############################# Header ############################
title: "Firma XLSX con firme digitali" 
description: "Proteggi il contenuto dei tuoi documenti aziendali sigillandoli con certificati digitali utilizzando le funzionalità di GroupDocs.Signature for Java. Offriamo diversi modi per contrassegnare e garantire i tuoi documenti."
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
       [GroupDocs.Signature for Java](/signature/java/) è una soluzione di firma completa che supporta vari tipi di elaborazione documentale. Puoi aggiungere testo, immagini, certificati digitali e timbri a file in oltre 60 formati, tra cui PDF, MS Office, immagini, file ZIP e altri formati aziendali popolari. Inoltre, i documenti firmati possono essere cercati, verificati, modificati o eliminati automaticamente in modo conveniente.

############################# Steps ############################
steps:
    enable: true
    title: "Passaggi per proteggere XLSX con certificati digitali in Java"
    content: |
      [GroupDocs.Signature](/signature/java/) consente agli sviluppatori Java di prevenire modifiche nei documenti XLSX utilizzando firme digitali. Potenzia le tue applicazioni aziendali con la capacità di proteggere dati importanti.
      
      1. Passa il documento XLSX al costruttore della classe Signature.
      2. Usa un certificato digitale e la sua password per proteggere il documento.
      3. Facoltativamente, aggiungi una rappresentazione visiva della firma digitale sulle pagine del documento.
      4. Firma il documento per prevenire eventuali modifiche future.
   
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
        // Usa Signature con il documento per la firma digitale
        Signature signature = new Signature("input.xlsx");

        // Fornisci un certificato digitale e una password
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Imposta una rappresentazione visiva se necessario
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);

        // Proteggi il documento con un certificato digitale
        SignResult result = signature.sign("output.xlsx", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Migliora o proteggi il contenuto del documento con firme"
  description: "La libreria GroupDocs.Signature for Java è in grado di firmare tutti i formati di file più diffusi. Aggiungi, modifica, verifica o elimina vari tipi di firme automaticamente per semplificare i tuoi processi aziendali."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Caratteristiche di GroupDocs.Signature"
  features:
    # feature loop
    - title: "Aggiungi firme ai documenti"
      content: "Le firme di testo, immagine, codice a barre, QR-Code o timbro possono essere aggiunte con precisione a qualsiasi pagina di qualsiasi documento supportato. Metadata nascosti come EXIF possono essere aggiunti o modificati nelle immagini e nella maggior parte dei tipi di file. Proteggi il contenuto del documento da modifiche non autorizzate utilizzando firme digitali."

    # feature loop
    - title: "Ricerca e verifica delle firme"
      content: "I documenti possono essere elaborati in vari modi dopo la firma. Verifica i documenti firmati per assicurarti che siano stati elaborati correttamente. Se hai bisogno di maggiore controllo, recupera un elenco di tutte le firme tramite ricerca."

    # feature loop
    - title: "Modifica delle firme"
      content: "La maggior parte dei tipi di firme supporta ulteriori modifiche. Sei libero di correggere il testo, cambiare posizione, colore, dimensione e altro."

    # feature loop
    - title: "Rimuovi firme non necessarie"
      content: "La nostra soluzione supporta operazioni CRUD complete per le firme. Molti tipi di firme, inclusi i certificati digitali, possono essere eliminati da un documento quando necessario."
      
  code_samples:
    # code sample loop
    - title: "Proteggi i documenti con firme digitali"
      content: |
        Scopri come proteggere un documento da modifiche utilizzando firme digitali.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // Fornisci un documento per la firma
        Signature signature = new Signature("input.xlsx");

        // Utilizza un certificato digitale valido con una password
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // Specifica dati testuali aggiuntivi
        options.setReason("Security issue");
        options.setContact("John Smith");
        options.setLocation("Office D.W.");

        // Usa un'immagine e altre opzioni per la rappresentazione visiva
        options.setImageFilePath("image.png");

        options.setAllPages(true);
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        Padding padding = new Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);

        // Salva il documento protetto in una posizione diversa
        SignResult result = signature.sign("output.xlsx", options);
        ```
        {{< /landing/code >}}


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
    title: "Esamina il nostro ampio set di funzionalità"
    exclude: "digital"
    description: "Siamo orgogliosi della vasta funzionalità e del supporto per le firme che la nostra piattaforma offre."
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
    title: "Firma documenti in altri formati"
    exclude: "XLSX"
    description: "L'API Java ti consente di elaborare più di 60 formati. Crea e aggiungi varie firme a qualsiasi pagina, sigilla il contenuto con certificati digitali e gestisci e modifica firme esistenti all'interno del documento."
    items: 
          
        # format loop 1
        - name: "Proteggi PDF"
          format: "PDF"
          link: "/signature/java/digital/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "Proteggi DOCX"
          format: "DOCX"
          link: "/signature/java/digital/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "Proteggi PPTX"
          format: "PPTX"
          link: "/signature/java/digital/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 4
        - name: "Proteggi XLSX"
          format: "XLSX"
          link: "/signature/java/digital/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---