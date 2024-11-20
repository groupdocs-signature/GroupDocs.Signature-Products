



---
############################# Static ############################
layout: "format"
date:  2024-11-20T08:57:23
draft: false
lang: it
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Aggiungere firme elettroniche digitali a file XLSX con JavaScript"
head_description: "Apponi una firma digitale su un file XLSX utilizzando JavaScript con poche righe di codice. Usa GroupDocs.Signature for Node.js via Java per firmare numerosi formati di file."

############################# Header ############################
title: "Proteggi XLSX con certificati digitali" 
description: "Garantisci la sicurezza dei tuoi documenti aziendali integrando certificati digitali grazie alle avanzate funzionalità di GroupDocs.Signature for Node.js via Java. Offriamo opzioni flessibili per proteggere e autenticare i tuoi documenti."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica gratuitamente"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Informazioni su GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) è una soluzione completa per la firma progettata per gestire una varietà di esigenze di elaborazione dei documenti. Consente di incorporare testi, immagini, certificati digitali e timbri in oltre 60 diversi formati di file, inclusi PDF, MS Office, immagini e file ZIP. Inoltre, i documenti firmati possono essere facilmente cercati, verificati, modificati o eliminati se necessario.

############################# Steps ############################
steps:
    enable: true
    title: "Linee guida per la protezione di XLSX con certificati digitali in JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) consente agli sviluppatori Node.js via Java di proteggere i documenti XLSX dalle modifiche utilizzando firme digitali. Migliora le tue applicazioni aziendali con funzionalità di sicurezza dei dati complete.
      
      1. Passa il documento XLSX al costruttore della classe Signature.
      2. Applica un certificato digitale e la relativa password per proteggere il documento.
      3. Facoltativamente, aggiungi una rappresentazione visiva della firma digitale sulle pagine del documento.
      4. Firma il documento per impedire future alterazioni.
   
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

        // Utilizza Signature per applicare una firma digitale al documento
        const signature = new signatureLib.Signature('input.xlsx');

        // Fornisci il certificato digitale richiesto e la password
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // Configura le impostazioni della firma visiva se necessario
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);
        
        // Cripta il documento utilizzando il certificato digitale
        const result = signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Ottimizza o proteggi il contenuto del documento con firme"
  description: "GroupDocs.Signature for Node.js via Java è progettato per firmare tutti i principali formati di file, offrendoti la possibilità di aggiungere, modificare, verificare o rimuovere vari tipi di firme."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Signature"
  features:
    # feature loop
    - title: "Aggiungi firme ai tuoi documenti"
      content: "Posiziona Text, Image, Barcode, QR-Code o firme Stamp su qualsiasi pagina dei documenti supportati. Puoi anche inserire o modificare metadati nascosti, come EXIF nelle immagini. Proteggi il contenuto del tuo documento da alterazioni non autorizzate con certificati digitali."

    # feature loop
    - title: "Trova e verifica le firme"
      content: "Dopo la firma, il tuo documento può subire più verifiche. Conferma l'integrità del contenuto firmato o esegui una ricerca dettagliata per elencare tutte le firme esistenti."

    # feature loop
    - title: "Rivedi le firme esistenti"
      content: "La maggior parte dei tipi di firma consente modifiche post-creazione. Puoi facilmente modificare il testo, riposizionare gli elementi, regolare i colori, ridimensionare e apportare altre modifiche necessarie."

    # feature loop
    - title: "Elimina firme non necessarie"
      content: "La nostra soluzione consente operazioni CRUD complete per le firme. Se necessario, puoi rimuovere vari tipi di firme, compresi i certificati digitali, dal tuo documento."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Proteggi documenti con firme digitali"
      content: |
        Scopri come bloccare un documento contro le modifiche utilizzando firme digitali.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Fornisci il documento che richiede la firma
          const signature = new signatureLib.Signature('input.xlsx');

          // Utilizza un certificato digitale appropriato e la sua password
          const options = new signatureLib.DigitalSignOptions('certificate.pfx');
          options.setPassword('1234567890');

          // Includi eventuali informazioni testuali aggiuntive
          options.setReason('Security issue');
          options.setContact('John Smith');
          options.setLocation('Office D.W.');

          // Aggiungi elementi visivi come immagini per la rappresentazione della firma
          options.setImageFilePath('image.png');
          options.setAllPages(true);
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setWidth(80);
          options.setHeight(60);

          const padding = new signatureLib.Padding();
          padding.setBottom(10);
          padding.setRight(10);
          options.setMargin(padding);
          
          // Salva il documento digitalmente protetto in una posizione specificata
          const result = signature.sign('output.xlsx', options);
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
            link: "/examples/signature/formats/signature_digital.xlsx"
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
    title: "Scopri le nostre funzioni principali"
    exclude: "digital"
    description: "Siamo orgogliosi di supportare una suite completa di opzioni e funzionalità di firma."
    items: 
          
        # operation loop 1
        - name: "Firme elettroniche"
          operation: "esign"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "Aggiungi vari tipi di firme ai formati di file supportati"

        # operation loop 2
        - name: "Aggiungi testo ai documenti"
          operation: "text"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Migliora il contenuto del documento con firme testuali personalizzabili"

        # operation loop 3
        - name: "Firme con immagine"
          operation: "image"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Posiziona qualsiasi immagine in qualsiasi punto di un documento"

        # operation loop 4
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "Crea e inserisci vari codici a barre nei documenti supportati"

        # operation loop 5
        - name: "Genera QR code"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Genera e QR code, incluso QR code, per la firma dei documenti"
          
        # operation loop 6
        - name: "Certificati digitali"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Proteggi documenti commerciali e firmali con certificati digitali"

        # operation loop 7
        - name: "Firme a timbro"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "Utilizza il Costruttore di Timbri per creare timbri personalizzati rotondi o quadrati"
          
        # operation loop 8
        - name: "Cerca firme"
          operation: "search"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "Trova qualsiasi firma precedentemente aggiunta all'interno di un documento"
          
        # operation loop 9
        - name: "Verifica delle firme"
          operation: "verify"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "Verifica l'autenticità delle firme dopo che sono state applicate"
          
        # operation loop 10
        - name: "Modifica firme"
          operation: "modify"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "Modifica facilmente una varietà di firme all'interno di un documento"
          
        # operation loop 11
        - name: "Elimina firme"
          operation: "delete"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "Rimuovi un'ampia gamma di firme precedentemente applicate"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Firma documenti in diversi formati"
    exclude: "XLSX"
    description: "L'API Node.js via Java supporta oltre 60 formati, consentendoti di applicare una gamma di firme su qualsiasi pagina, rafforzare la sicurezza dei contenuti con certificati digitali e gestire le firme all'interno del documento in modo efficace."
    items: 
          
        # format loop 1
        - name: "Proteggi PDF"
          format: "PDF"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "Proteggi DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "Proteggi PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 4
        - name: "Proteggi XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---