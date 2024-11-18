



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:48
draft: false
lang: it
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Genera e aggiungi timbri a XLSX tramite JavaScript"
head_description: "Sfrutta la potenza di GroupDocs.Signature e JavaScript per generare e posizionare timbri personalizzati su qualsiasi pagina dei tuoi documenti XLSX."

############################# Header ############################
title: "Inserisci timbri personalizzati nei file XLSX" 
description: "Utilizza GroupDocs.Signature for Node.js via Java per generare timbri su misura e inserirli in qualsiasi posizione dei tuoi documenti. La nostra piattaforma offre ampie opzioni per personalizzare i timbri in base alle tue specifiche esigenze aziendali."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Prova gratuita"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Cos'è GroupDocs.Signature for Node.js via Java?"
    link: "/signature/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) offre una soluzione robusta e versatile per la firma dei documenti. Permette agli utenti di aggiungere timbri e altri tipi di firma in oltre 60 formati diversi, come PDF, Word, Excel, file immagini e ZIP. La piattaforma consente di inserire testo, immagini, codici a barre, codici QR, metadati, certificati digitali e firme timbrate. Oltre alla firma, puoi cercare, verificare, modificare o eliminare qualsiasi firma presente nei tuoi documenti.

############################# Steps ############################
steps:
    enable: true
    title: "Guida all'inserimento di timbri in XLSX utilizzando JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) offre un potente strumento per creare e incorporare timbri, che possono migliorare significativamente le applicazioni Node.js via Java. Utilizza questa funzionalità per creare e applicare timbri personalizzati alle pagine dei tuoi documenti.
      
      1. Inserisci il documento XLSX che richiede timbratura.
      2. Utilizza StampSignOptions per definire tutti i parametri essenziali.
      3. Inserisci tante righe di timbre quante necessarie.
      4. Applica il timbro e salva il documento finale.
   
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

        // Associa il percorso del documento con l'istanza di Signature
        const signature = new signatureLib.Signature('input.xlsx');

        // Crea StampSignOptions con il contenuto della firma necessario
        const options = new signatureLib.StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // Incorpora una o più righe di timbro
        const outerLine = new signatureLib.StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(signatureLib.Color.WHITE);
        outerLine.setBackgroundColor(signatureLib.Color.BLUE);
        options.getOuterLines().add(outerLine);

        // Salva il documento con il timbro applicato
        const result = signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Rafforza la sicurezza dei documenti con firme"
  description: "Con GroupDocs.Signature for Node.js via Java, puoi aggiungere, modificare, convalidare o rimuovere timbri e altri tipi di firma in tutti i formati di documento più comuni. L'API semplifica il processo di gestione delle firme per una maggiore integrità e personalizzazione dei documenti."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Caratteristiche di GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firma personalizzata dei documenti"
      content: "Applica firme come testo, immagini, codici a barre, codici QR e timbri in qualsiasi parte del tuo documento. Questo strumento consente anche l'inclusione di metadati nascosti e certificati digitali per proteggere ulteriormente il contenuto da modifiche non autorizzate."

    # feature loop
    - title: "Ricerca e verifica delle firme"
      content: "Dopo che un documento è stato firmato, utilizza il nostro sistema di verifica per garantire l'integrità delle firme. Inoltre, la nostra piattaforma consente di cercare e recuperare informazioni dettagliate su tutte le firme applicate a un documento."

    # feature loop
    - title: "Modifica le firme secondo necessità"
      content: "Regola e aggiorna facilmente le firme precedentemente applicate. Che si tratti di cambiare il contenuto, il colore, la dimensione o la posizione della firma, GroupDocs.Signature for Node.js via Java offre opzioni di personalizzazione complete."

    # feature loop
    - title: "Rimuovi firme indesiderate"
      content: "Rimuovi senza difficoltà qualsiasi firma non necessaria dai tuoi documenti. La nostra API supporta l'eliminazione di un'ampia gamma di tipi di firma, comprese le timbrature e i certificati digitali, offrendoti completa flessibilità nella gestione dei tuoi documenti."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Integra timbri personalizzati nei documenti"
      content: |
        Scopri come progettare e applicare timbri personalizzati contenenti testo essenziale ai tuoi documenti.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Fornisci il documento per la timbratura
          const signature = new signatureLib.Signature('input.xlsx');

          // Imposta le opzioni di timbro con le configurazioni desiderate
          const options = new signatureLib.StampSignOptions();

          // Specifica le dimensioni e la posizione del timbro sulla pagina
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setAllPages(true);

          // Includi linee circolari esterne con testo personalizzato
          const outerLine1 = new signatureLib.StampLine();
          outerLine1.setText('* The best  choice *');
          outerLine1.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
          const signatureFont1 = new signatureLib.SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName('Arial');
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(signatureLib.Color.WHITE);
          outerLine1.setBackgroundColor(signatureLib.Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // Aggiungi linee quadrate interne secondo necessità
          const innerLine1 = new signatureLib.StampLine();
          innerLine1.setText('Company #1');
          innerLine1.setTextColor(signatureLib.Color.RED);
          const signFont1 = new signatureLib.SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);
          
          // Salva il documento timbrato
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
            link: "/examples/signature/formats/signature_stamp.xlsx"
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
    title: "Esplora le funzionalità chiave"
    exclude: "stamp"
    description: "La nostra soluzione offre una varietà di strumenti per creare, gestire e rimuovere diversi tipi di firme, dando agli utenti il controllo completo sui loro flussi di lavoro documentali."
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
    title: "Applica firme timbrate su più tipi di file"
    exclude: "XLSX"
    description: "L'API di GroupDocs.Signature supporta firme timbrate in oltre 60 formati di file, consentendo agli utenti di posizionare timbri personalizzati su qualsiasi pagina o area, migliorando l'accessibilità e la sicurezza dei documenti."
    items: 
          
        # format loop 1
        - name: "Apponi timbro su PDF"
          format: "PDF"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "Apponi timbro su DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "Apponi timbro su JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "Immagine JPEG"
          
        # format loop 4
        - name: "Apponi timbro su PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/stamp/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 5
        - name: "Apponi timbro su XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---