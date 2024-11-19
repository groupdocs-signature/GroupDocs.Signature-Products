



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:21
draft: false
lang: it
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Genera codici QR in documenti DOCX con JavaScript"
head_description: "Utilizza l'API GroupDocs.Signature per creare e integrare codici a barre 2D all'interno dei file DOCX. Posiziona senza difficoltà codici QR su qualsiasi pagina del documento."

############################# Header ############################
title: "Crea codici QR per DOCX" 
description: "Genera e inserisci codici a barre 2D con contenuti personalizzabili, tra cui testi e dati numerici, attraverso vari tipi di documenti come PDF, Word, Excel e Immagini con GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Provalo Gratis"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Esplora le capacità di GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) offre strumenti avanzati per il miglioramento dei documenti, consentendo la generazione e l'inserimento di diversi tipi di firme, compresi i codici QR, nei formati di file più comuni. Firma e proteggi PDF, documenti Word, fogli di calcolo Excel, presentazioni PowerPoint e immagini con firme di tipo Testo, Immagine, Codice a barre, Codice QR, Metadati, Digitale e Timbro.

############################# Steps ############################
steps:
    enable: true
    title: "Guida alla generazione e all'inserimento di un codice QR in qualsiasi posizione all'interno di un DOCX"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) consente la creazione di codici QR in vari formati ampiamente usati e la loro integrazione in pagine DOCX. Supportando oltre 10 diversi tipi di codici QR, la nostra soluzione può essere integrata senza problemi nelle applicazioni Node.js via Java, arricchendole con capacità di firma con codici QR.
      
      1. Fornisci il file o il flusso DOCX per la firma del codice QR.
      2. Inserisci il testo desiderato nell'istanza di QrCodeSignOptions.
      3. Regola le impostazioni visive come colore, posizione, dimensione, ecc.
      4. Salva il documento contenente il codice QR.
   
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

        // Crea un'istanza di Signature e passa il percorso del documento
        const signature = new signatureLib.Signature('input.docx');

        // Utilizza QrCodeSignOptions per inserire un codice QR nel documento
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // Definisci il tipo di firma e la posizione sulla pagina
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // Salva il documento con il codice QR appena aggiunto
        signature.sign('output.docx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Integrazione completa delle firme e dei codici QR"
  description: "Con l'API GroupDocs.Signature for Node.js via Java, puoi gestire un'ampia gamma di firme. Genera, personalizza, verifica, cerca e rimuovi firme senza sforzo su diversi tipi di documenti, offrendo una flessibilità senza pari per i tuoi flussi di lavoro."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Funzionalità di firma e codice QR"
  features:
    # feature loop
    - title: "Firma di documenti multi-formato"
      content: "Aggiungi diversi tipi di firme, tra cui firme di Testo, Immagine, Codice a barre, Codice QR e Timbro, a qualsiasi formato di documento supportato. Posizionali su qualsiasi pagina e gestisci i metadati del documento. Garantire la sicurezza del documento tramite certificati digitali per prevenire modifiche non autorizzate."

    # feature loop
    - title: "Validazione efficiente delle firme"
      content: "Valida tutte le firme all'interno di un documento per assicurarti che soddisfino gli standard richiesti. Recupera e rivedi facilmente le firme tramite la funzionalità di ricerca integrata."

    # feature loop
    - title: "Modifica flessibile delle firme"
      content: "Aggiorna o modifica firme esistenti, regolando aspetti come contenuto, posizione, dimensione e colore, secondo le esigenze del tuo documento dopo la firma iniziale."

    # feature loop
    - title: "Rimozione delle firme semplificata"
      content: "Rimuovi facilmente qualsiasi firma indesiderata o obsoleta, inclusi i certificati digitali. Un completo controllo sulla gestione delle firme assicura un documento pulito e ben organizzato."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Personalizzazione di un codice QR generato"
      content: |
        Questo esempio illustra il processo di aggiunta di un codice QR personalizzato a una pagina DOCX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Ottieni il documento da firmare e passalo a Signature
          const signature = new signatureLib.Signature('input.docx');

          // Imposta le opzioni del codice QR con il testo richiesto
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // Determina la posizione del codice QR sulla pagina
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Specifica il padding della firma
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Scegli il colore del codice QR
          signOptions.setForeColor(signatureLib.Color.RED);

          // Definisci le opzioni di font per il messaggio accompagnatorio
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Personalizza il colore di sfondo e il pennello per il codice QR
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Integra il codice QR nel documento
          signature.sign('output.docx', signOptions);
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
            link: "/examples/signature/formats/signature_qrcode.docx"
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
    title: "Comprendere le nostre principali capacità"
    exclude: "qrcode"
    description: "Offriamo un'ampia selezione di formati di firma e operazioni su misura per le tue esigenze"
    items: 
          
        # operation loop 1
        - name: "Firme elettroniche"
          operation: "esign"
          link: "/signature/nodejs-java/esign/docx/"
          description: "Aggiungi vari tipi di firme ai formati di file supportati"

        # operation loop 2
        - name: "Aggiungi testo ai documenti"
          operation: "text"
          link: "/signature/nodejs-java/text/docx/"
          description: "Migliora il contenuto del documento con firme testuali personalizzabili"

        # operation loop 3
        - name: "Firme con immagine"
          operation: "image"
          link: "/signature/nodejs-java/image/docx/"
          description: "Posiziona qualsiasi immagine in qualsiasi punto di un documento"

        # operation loop 4
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "Crea e inserisci vari codici a barre nei documenti supportati"

        # operation loop 5
        - name: "Genera QR code"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Genera e QR code, incluso QR code, per la firma dei documenti"
          
        # operation loop 6
        - name: "Certificati digitali"
          operation: "digital"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Proteggi documenti commerciali e firmali con certificati digitali"

        # operation loop 7
        - name: "Firme a timbro"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "Utilizza il Costruttore di Timbri per creare timbri personalizzati rotondi o quadrati"
          
        # operation loop 8
        - name: "Cerca firme"
          operation: "search"
          link: "/signature/nodejs-java/search/docx/"
          description: "Trova qualsiasi firma precedentemente aggiunta all'interno di un documento"
          
        # operation loop 9
        - name: "Verifica delle firme"
          operation: "verify"
          link: "/signature/nodejs-java/verify/docx/"
          description: "Verifica l'autenticità delle firme dopo che sono state applicate"
          
        # operation loop 10
        - name: "Modifica firme"
          operation: "modify"
          link: "/signature/nodejs-java/modify/docx/"
          description: "Modifica facilmente una varietà di firme all'interno di un documento"
          
        # operation loop 11
        - name: "Elimina firme"
          operation: "delete"
          link: "/signature/nodejs-java/delete/docx/"
          description: "Rimuovi un'ampia gamma di firme precedentemente applicate"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Integra codici QR con vari formati di file"
    exclude: "DOCX"
    description: "Sfrutta l'API Node.js via Java per generare codici QR e integrarli in una varietà di formati di file ampiamente utilizzati. Incapsula informazioni importanti in questi codici a barre per un'integrazione fluida e un recupero futuro."
    items: 
          
        # format loop 1
        - name: "QR-Code per PDF"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "QR-Code per DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "QR-Code per JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "Immagine JPEG"
          
        # format loop 4
        - name: "QR-Code per PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 5
        - name: "QR-Code per XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---