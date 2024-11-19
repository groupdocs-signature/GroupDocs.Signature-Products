



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:38
draft: false
lang: it
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Modifica le firme PDF con applicazioni Java"
head_description: "L'API di elaborazione delle firme Java consente di modificare le firme in file PDF, inclusi PDF, Word, Excel, Presentazioni e Immagini."

############################# Header ############################
title: "Modifica le firme PDF" 
description: "Modifica una vasta gamma di firme elettroniche utilizzando GroupDocs.Signature for Java in formati popolari come PDF, Word, Excel, Presentazioni e Immagini."
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
       [GroupDocs.Signature for Java](/signature/java/) non solo consente di firmare documenti, ma offre anche la possibilità di modificare le firme esistenti. Aggiorna facilmente le firme in formati ampiamente utilizzati come PDF, Word, Excel e Presentazioni.

############################# Steps ############################
steps:
    enable: true
    title: "Passi per modificare le firme di testo in PDF utilizzando Java"
    content: |
      [GroupDocs.Signature](/signature/java/) consente agli sviluppatori Java di aggiornare il contenuto delle firme di testo precedentemente aggiunte a file PDF. Migliora le applicazioni Java con capacità robuste.
      
      1. Aggiungi il file PDF all'istanza Signature.
      2. Recupera un elenco di tutte le firme nel documento.
      3. Aggiorna il contenuto di qualsiasi firma identificata.
      4. Analizza i risultati della modifica.
   
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
        // Crea un oggetto Signature con il percorso del documento
        Signature signature = new Signature("input.pdf");

        // Cerca eventuali firme di testo all'interno del documento
        TextSearchOptions options = new TextSearchOptions();
        List<TextSignature> signatures = signature.search(TextSignature.class, options);

        if (signatures.size() > 0) {
            // Modifica il testo della prima firma rilevata
            TextSignature textSignature = signatures.get(0);
            textSignature.setText("New Text");
            boolean result = signature.update('output.pdf', textSignature);

            // Valida il risultato della modifica
            if (result) {
                System.out.print("\nSignature was updated successfully.");
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Gestione delle firme per documenti"
  description: "GroupDocs.Signature for Java ti consente di aggiungere, modificare, cercare, verificare e eliminare firme in tutti i principali formati di file industriali."
  image: "/img/signature/features_modify.webp" # 500x500 px
  image_description: "Modifica delle firme"
  features:
    # feature loop
    - title: "Firme sui documenti"
      content: "Il nostro prodotto si concentra principalmente sulla firma dei documenti con firme di testo, immagine, codice a barre o timbro. Puoi posizionarle su qualsiasi pagina e posizione. Aggiungi o modifica metadati nascosti, come i dati EXIF nelle immagini, e proteggi il contenuto del documento da modifiche non autorizzate utilizzando certificati digitali."

    # feature loop
    - title: "Ricerca e verifica delle firme"
      content: "Assicurati che le firme soddisfino i tuoi requisiti verificando i documenti firmati. Puoi recuperare un elenco completo delle firme all'interno di un documento tramite la funzionalità di ricerca."

    # feature loop
    - title: "Modifica delle firme esistenti"
      content: "Modificare le firme precedentemente aggiunte è un compito comune. Utilizza il processo di modifica per aggiornare il contenuto, l'aspetto, la posizione e altre proprietà di una firma."

    # feature loop
    - title: "Eliminazione delle firme"
      content: "La nostra soluzione supporta completamente tutte le operazioni relative alle firme. Rimuovere vari tipi di firme da un documento è un processo semplice."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Modifica le firme di codice a barre"
      content: |
        Questo esempio illustra il processo di modifica delle firme di codice a barre all'interno di un documento.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Utilizza un documento che contiene firme di codice a barre
          final Signature signature = new Signature("input.pdf");

          // Cerca firme di codice a barre esistenti
          BarcodeSearchOptions options = new BarcodeSearchOptions();
          List<BarcodeSignature> signatures = signature.search(BarcodeSignature.class, options);

          if (signatures.size() > 0)
          {
              // Regola la posizione della prima firma di codice a barre e salva il documento aggiornato
              BarcodeSignature barcodeSignature = signatures.get(0);
              barcodeSignature.setLeft(100);
              barcodeSignature.setTop(100);
              boolean result = signature.update("output.pdf", barcodeSignature);

              // Conferma il risultato della modifica
              if (result)
              {
                    System.out.print("\nBarcode was updated successfully.");
              }
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
    title: "Esplora il nostro portafoglio di funzionalità"
    exclude: "modify"
    description: "Siamo orgogliosi di supportare una vasta gamma di formati di firma e strumenti operativi."
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
    title: "Modifica le firme in vari formati di file"
    exclude: "PDF"
    description: "I formati di documento firmati utilizzando la nostra API per Java possono essere modificati. Recupera un elenco di firme da un documento e aggiorna qualsiasi proprietà accessibile."
    items: 
          
        # format loop 1
        - name: "Modifica firme PDF"
          format: "PDF"
          link: "/signature/java/modify/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "Modifica firme DOCX"
          format: "DOCX"
          link: "/signature/java/modify/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "Modifica firme PPTX"
          format: "PPTX"
          link: "/signature/java/modify/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 4
        - name: "Modifica firme XLSX"
          format: "XLSX"
          link: "/signature/java/modify/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---