



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:31
draft: false
lang: it
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Cerca di firma digitale in PDF utilizzando Java"
head_description: "Sfrutta l'API GroupDocs.Signature for Java per cercare firme all'interno di file PDF. Trova firme in PDF, Word, Excel, Presentazioni e Immagini."

############################# Header ############################
title: "Cerca firme digitali in PDF" 
description: "Recupera un elenco completo di e-firme incorporate in file PDF, Word, Excel, Presentazioni o Immagini utilizzando GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download gratuito"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Informazioni su GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) offre potenti funzionalità per la firma dei documenti. Supporta l'aggiunta di testo, immagini, codici a barre, certificati digitali e timbri a file in oltre 60 formati, tra cui PDF, documenti MS Office, Immagini, file ZIP e altri formati aziendali comuni. Inoltre, puoi cercare, verificare, modificare o eliminare le firme in qualsiasi momento.

############################# Steps ############################
steps:
    enable: true
    title: "Passi per cercare le firme PDF utilizzando Java"
    content: |
      [GroupDocs.Signature](/signature/java/) fornisce un motore potente per cercare tutte le firme digitali all'interno di file PDF. Gli sviluppatori Java possono migliorare le loro applicazioni con la nostra soluzione.
      
      1. Fornisci il percorso del file PDF per la ricerca della firma.
      2. Usa SearchOptions per affinare i risultati della ricerca.
      3. Esegui il metodo Search per ottenere i risultati.
      4. Analizza l'elenco delle firme trovate.
   
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

        // Crea un'istanza di Signature con il percorso del documento
        final Signature signature = new Signature("input.pdf");

        // Istanze TextSearchOptions per coprire tutte le pagine
        TextSearchOptions options = new TextSearchOptions();
        options.setAllPages(true);

        // Cerca firme testuali all'interno del documento
        List<TextSignature> signatures = signature.search(TextSignature.class, options);
        System.out.print("\nSource document contains following text signature(s).");

        // Elenca le firme trovate per ulteriori analisi
        for (TextSignature textSignature : signatures) {
            System.out.print("Found Text signature at page " + textSignature.getPageNumber() 
                + " with type [" + textSignature.getSignatureImplementation() + "] and 
                text '" + textSignature.getText() + "'.");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Soluzione completa per la firma dei documenti"
  description: "Siamo orgogliosi di presentare la nostra soluzione di firma dei documenti, compatibile con tutti i principali formati di documento. Aggiungi un'ampia gamma di firme per migliorare i tuoi documenti o proteggere i loro contenuti."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Ricerca firme"
  features:
    # feature loop
    - title: "Firma documenti aziendali"
      content: "Inserisci firme digitali in qualsiasi posizione su qualsiasi pagina di un documento. Usa una varietà di tipi di firma, come testo, immagini, codici a barre, metadata, timbri o certificati digitali."

    # feature loop
    - title: "Gestisci firme"
      content: "Dopo aver firmato, i documenti potrebbero richiedere ulteriori elaborazioni. Cerca tutte le firme disponibili e aggiornale o eliminale quando necessario."

    # feature loop
    - title: "Proteggi il contenuto del documento"
      content: "Gestisci i metadati nascosti incorporati nel documento. Aggiungi nuovi metadati o rimuovi voci esistenti. Utilizza certificati digitali aziendali per proteggere il contenuto del documento da modifiche non autorizzate."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cerca firme immagine"
      content: |
        Questo esempio dimostra come trovare una firma immagine in un documento specifico.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Passa il documento sorgente come parametro al costruttore
          final Signature signature = new Signature("input.pdf");

          // Cerca qualsiasi firma di tipo testo
          List<ImageSignature> signatures = signature.search(ImageSignature.class, SignatureType.Image);
          System.out.print("\nSource document contains following image signature(s).");

          // Visualizza i risultati con le proprietà delle firme trovate
          for (ImageSignature imageSignature : signatures)
          {
              System.out.print("Image signature found at page "+imageSignature.getPageNumber()+
                    " with size "+imageSignature.getSize()+". Created "+imageSignature.getCreatedOn()+
                    ", modified "+imageSignature.getModifiedOn());
          }
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
    title: "Operazioni supportate"
    exclude: "search"
    description: "Il nostro prodotto offre un'API flessibile per la firma dei documenti e la gestione delle firme dopo la firma."
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
    title: "Cerca firme in vari formati di file"
    exclude: "PDF"
    description: "L'API GroupDocs.Signature for Java ti consente di recuperare l'elenco delle firme da qualsiasi file firmato. Estrai firme da formati di file popolari per ulteriori elaborazioni."
    items: 
          
        # format loop 1
        - name: "Cerca firme in PDF"
          format: "PDF"
          link: "/signature/java/search/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "Trova firme in DOCX"
          format: "DOCX"
          link: "/signature/java/search/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "Trova firme in PPTX"
          format: "PPTX"
          link: "/signature/java/search/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 4
        - name: "Cerca firme in XLSX"
          format: "XLSX"
          link: "/signature/java/search/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---