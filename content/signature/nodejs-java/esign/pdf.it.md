



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:30
draft: false
lang: it
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Firma PDF con firme elettroniche in JavaScript"
head_description: "Sfrutta le capacità dell'API JavaScript per firmare digitalmente e proteggere i file PDF, inclusi PDF, documenti Word, fogli Excel, presentazioni e formati immagine."

############################# Header ############################
title: "Firma file PDF elettronicamente" 
description: "Utilizza GroupDocs.Signature for Node.js via Java per inserire diverse firme digitali nei tuoi documenti, garantendo l'integrità dei dati e la conformità per file come PDF, Word, Excel, presentazioni e formati immagine."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica ora gratuitamente"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Panoramica dell'API GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) offre un set robusto di strumenti per aggiungere firme elettroniche. Con la sua API intuitiva, puoi firmare, cercare, verificare, modificare e rimuovere firme da vari tipi di file senza necessità di software esterno. Supporta la firma fluida di PDF, documenti Word, fogli Excel, diapositive PowerPoint e numerosi formati immagine.

############################# Steps ############################
steps:
    enable: true
    title: "Passaggi per firmare PDF utilizzando JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) semplifica il processo di aggiunta di firme personalizzate a file PDF. Gli sviluppatori Node.js via Java possono incorporare senza difficoltà la funzionalità di firma nelle loro applicazioni.
      
      1. Carica il documento PDF nell'istanza Signature.
      2. Configura SignOptions per definire gli attributi della firma.
      3. Regola proprietà come dimensioni, colori e contenuto secondo necessità.
      4. Salva il documento firmato nella posizione specificata.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copia"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Firme di esempio"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // Importa il documento in un'istanza di Signature
        const signature = new signatureLib.Signature('input.pdf');

        // Istanziati un oggetto QrCodeSignOptions
        const options = new signatureLib.QrCodeSignOptions('QR code text');
        
        // Specifica tutte le opzioni necessarie
        options.setLeft(100);
        options.setTop(100);
        options.setForeColor(new Color(255, 0, 0));

        // Salva il documento firmato sul disco locale
        signature.sign('output.pdf', options);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacità avanzate di firma digitale"
  description: "La nostra API avanzata semplifica le operazioni aziendali facilitando la firma automatizzata, la verifica, la modifica e la gestione delle firme elettroniche per una gamma di documenti."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "Funzionalità della firma digitale"
  features:
    # feature loop
    - title: "Firma digitale per file di ufficio"
      content: "Aggiungi firme digitali facilmente a qualsiasi pagina o posizione all'interno di un documento. Personalizza le tue firme con opzioni come certificati digitali, metadati, codici a barre o elementi visivi per migliorare la sicurezza e l'integrità del documento."

    # feature loop
    - title: "Controllo completo delle firme"
      content: "Una volta firmato un documento, puoi gestire le sue firme senza sforzo. Recupera un elenco completo di tutte le firme, permettendoti di effettuare aggiornamenti o rimuoverle secondo necessità."

    # feature loop
    - title: "Rafforza la sicurezza del documento"
      content: "Utilizza certificati digitali per proteggere i tuoi documenti da manomissioni. Puoi incorporare o estrarre metadati per migliorare la tracciabilità e l'audit, garantendo la conformità e l'autenticità del documento."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Come applicare una firma immagine a un documento"
      content: |
        Questa guida illustra il processo per affiggere una firma immagine a una pagina designata all'interno di un documento.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
        
          // Fornire il documento sorgente come parametro di input
          const signature = new signatureLib.Signature('input.pdf');

          // Specifica il percorso del file dell'immagine nelle opzioni di configurazione della firma
          const options = new signatureLib.ImageSignOptions('image.jpg');

          // Configura le dimensioni e specifica le pagine di destinazione per la firma
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setHeight(150);
          options.setWidth(200);
          options.setMargin(new signatureLib.Padding(50));
          options.setAllPages(true);

          // Attua l'applicazione della firma al documento
          signature.sign('output.pdf', options);

          ```
        platform: "nodejs-java"
        copy_title: "Copia"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "clicca per copiare"
          copy_done: "copiato"
        top_links:
          #  loop
          - title: "Scarica il risultato"
            icon: "download"
            link: "/examples/signature/formats/signature_esign.pdf"
        links:
          #  loop
          - title: "Altri esempi"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "Documentazione"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Prova gratuitamente le funzionalità di GroupDocs.Signature o richiedi una licenza."
  items:
    #  loop
    - title: "Download di NPM"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licenze"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Scopri le nostre ampie capacità"
    exclude: "esign"
    description: "Offriamo una vasta gamma di tipi di firma e operazioni ricche di funzionalità."
    items: 
          
        # operation loop 1
        - name: "Firme elettroniche"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "Aggiungi vari tipi di firme ai formati di file supportati"

        # operation loop 2
        - name: "Aggiungi testo ai documenti"
          operation: "text"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Migliora il contenuto del documento con firme testuali personalizzabili"

        # operation loop 3
        - name: "Firme con immagine"
          operation: "image"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Posiziona qualsiasi immagine in qualsiasi punto di un documento"

        # operation loop 4
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Crea e inserisci vari codici a barre nei documenti supportati"

        # operation loop 5
        - name: "Genera QR code"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Genera e QR code, incluso QR code, per la firma dei documenti"
          
        # operation loop 6
        - name: "Certificati digitali"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Proteggi documenti commerciali e firmali con certificati digitali"

        # operation loop 7
        - name: "Firme a timbro"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "Utilizza il Costruttore di Timbri per creare timbri personalizzati rotondi o quadrati"
          
        # operation loop 8
        - name: "Cerca firme"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Trova qualsiasi firma precedentemente aggiunta all'interno di un documento"
          
        # operation loop 9
        - name: "Verifica delle firme"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Verifica l'autenticità delle firme dopo che sono state applicate"
          
        # operation loop 10
        - name: "Modifica firme"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "Modifica facilmente una varietà di firme all'interno di un documento"
          
        # operation loop 11
        - name: "Elimina firme"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "Rimuovi un'ampia gamma di firme precedentemente applicate"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Firma digitalmente più tipi di file"
    exclude: "PDF"
    description: "L'API Node.js via Java ti consente di applicare firme digitali a oltre 60 formati di file, offrendoti grande flessibilità nel garantire documenti aziendali critici."
    items: 
          
        # format loop 1
        - name: "e-Firma PDF"
          format: "PDF"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "e-Firma DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/esign/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "e-Firma JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "Immagine JPEG"
          
        # format loop 4
        - name: "e-Firma PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/esign/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 5
        - name: "e-Firma XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---