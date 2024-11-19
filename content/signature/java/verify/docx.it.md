



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:35
draft: false
lang: it
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Verifica le e-firme DOCX utilizzando Java"
head_description: "GroupDocs.Signature for Java consente la verifica delle firme presenti nei file DOCX. Valida le firme in PDF, documenti Word, fogli Excel, Presentazioni, Immagini o archivi ZIP."

############################# Header ############################
title: "Verifica delle e-firme per DOCX" 
description: "Verifica tutte le e-firme supportate nei file PDF, Word, Excel, Presentazioni, Immagini o ZIP con GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica la versione gratuita"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Applicazioni di GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) supporta operazioni complete di CRUD per la firma dei documenti e altro ancora. Firma oltre 60 formati di documento, inclusi PDF, file MS Office, Immagini e archivi ZIP, utilizzando testo, immagini, codici a barre, certificati digitali, metadati e timbri. Sono disponibili anche operazioni aggiuntive come cercare, verificare, modificare o eliminare firme.

############################# Steps ############################
steps:
    enable: true
    title: "Passaggi per verificare le firme in DOCX utilizzando Java"
    content: |
      [GroupDocs.Signature](/signature/java/) può verificare la presenza di firme specifiche in un documento DOCX. Gli sviluppatori Java possono potenziare le proprie applicazioni aggiungendo le funzionalità fornite dalla nostra soluzione.
      
      1. Carica il file DOCX nell'istanza di Signature.
      2. Instanzia e configura VerifyOptions per ottenere il risultato desiderato.
      3. Avvia il processo di verifica.
      4. Rivedi i risultati della verifica.
   
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
        // Instanzia un Signature con il documento
        Signature signature = new Signature("input.docx");

        // Crea TextVerifyOptions per convalidare le firme contenenti testo specifico
        TextVerifyOptions options = new TextVerifyOptions();
        options.setText("signature");
        options.setMatchType(TextMatchType.Contains);

        // Verifica le firme nel documento
        VerificationResult result = signature.verify(options);

        // Elabora i risultati della verifica
        if (result.isValid())
        {
            System.out.print("\nDocument was verified successfully!");
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Soluzione completa per la firma dei documenti"
  description: "GroupDocs.Signature migliora i formati di documenti d'ufficio più diffusi con 7 tipologie di firme e operazioni complete di CRUD, offrendo protezione robusta per il contenuto del tuo documento."
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "Verifica della firma"
  features:
    # feature loop
    - title: "Firma documenti aziendali"
      content: "Aggiungi firme digitali professionali a qualsiasi documento. La nostra soluzione supporta varie tipologie di firme, tra cui testo, immagini, codici a barre, metadati, timbri e certificati digitali."

    # feature loop
    - title: "Operazioni CRUD delle firme"
      content: "In molti casi, i documenti firmati richiedono ulteriori elaborazioni. Recupera un elenco di tutte le firme in un documento, verifica la loro validità, modifica le loro proprietà o rimuovile quando necessario."

    # feature loop
    - title: "Proteggi il contenuto del documento"
      content: "Proteggi i documenti aziendali con certificati digitali per prevenire modifiche non autorizzate. Inserisci metadati nascosti per proteggere ulteriormente il contenuto del documento."

    # feature loop
    - title: "Firme native"
      content: "Utilizza firme testuali specifiche per il documento, come timbri PDF o filigrane Word, per creare documenti professionali personalizzati per uso aziendale."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Verifica delle firme a codice a barre"
      content: |
        Questo esempio dimostra come verificare le firme a codice a barre in un documento.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Fornisci il documento contenente le firme a codice a barre
          final Signature signature = new Signature("input.docx");

          // Configura le opzioni per verificare i codici a barre rispetto a un testo specifico
          BarcodeVerifyOptions options = new BarcodeVerifyOptions();
          options.setText("12345");
          options.setMatchType(TextMatchType.StartsWith);

          // Verifica le firme applicate al documento
          VerificationResult result = signature.verify(options);

          // Visualizza i risultati della verifica
          if (result.isValid())
          {
              System.out.print("\nDocument was verified successfully!");
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
    title: "Operazioni supportate e tipologie di firme"
    exclude: "verify"
    description: "Esplora l'intera gamma di funzionalità e operazioni di firma supportate da GroupDocs.Signature."
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
          
############################# More Formats #####################
more_formats:
    enable: true
    title: "Verifica delle firme su vari formati di file"
    exclude: "DOCX"
    description: "GroupDocs.Signature for Java semplifica il processo di verifica di tutte le firme in un documento. Imposta parametri di verifica personalizzati per garantire l'integrità dei documenti firmati."
    items: 
          
        # format loop 1
        - name: "Verifica firme PDF"
          format: "PDF"
          link: "/signature/java/verify/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "Verifica firme DOCX"
          format: "DOCX"
          link: "/signature/java/verify/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "Verifica firme PPTX"
          format: "PPTX"
          link: "/signature/java/verify/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 4
        - name: "Valida firme XLSX"
          format: "XLSX"
          link: "/signature/java/verify/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---