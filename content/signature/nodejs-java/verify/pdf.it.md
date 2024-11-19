



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:36
draft: false
lang: it
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Verifica le firme digitali in PDF tramite JavaScript"
head_description: "Con GroupDocs.Signature for Node.js via Java, puoi verificare in modo efficiente l'autenticità delle firme nei documenti PDF. Controlla senza problemi le firme in PDF, Word, Excel, Presentazioni, Immagini, file ZIP e altro."

############################# Header ############################
title: "Verifica le firme digitali in PDF" 
description: "Assicura l'accuratezza e la validità di tutte le e-firme supportate in una vasta gamma di formati di documento, inclusi PDF, Word, Excel, Presentazioni, Immagini e ZIP, utilizzando GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica la versione gratuita"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Applicazioni di GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) offre una gestione completa delle firme sui documenti, incluso il supporto per oltre 60 formati di file. Con supporto per testi, immagini, codici a barre, certificati digitali, metadati, timbri e altro, GroupDocs.Signature for Node.js via Java ti consente di cercare, verificare, aggiornare o rimuovere le firme senza sforzo in formati come PDF, documenti MS Office, Immagini, archivi ZIP e altro.

############################# Steps ############################
steps:
    enable: true
    title: "Come verificare le firme in PDF usando JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) può autenticare la presenza di firme specifiche in un documento PDF. Gli sviluppatori Node.js via Java possono migliorare le loro applicazioni integrando le nostre funzionalità di verifica.
      
      1. Carica il documento PDF nell'istanza Signature.
      2. Crea e configura VerifyOptions per ottenere i risultati di verifica desiderati.
      3. Avvia il processo di verifica.
      4. Esamina e valuta i risultati della verifica.
   
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

        // Instanzia un oggetto Signature con il documento
        const signature = new signatureLib.Signature('input.pdf');

        // Stabilisci TextVerifyOptions per convalidare le firme che includono testo specificato
        const options = new signatureLib.TextVerifyOptions();
        options.setText('signature');
        options.setMatchType(signatureLib.TextMatchType.Contains);

        // Esegui il processo di verifica per le firme del documento
        const result = signature.verify(options);

        // Interpreta e valuta i risultati della verifica
        if (result.isValid()) {
            console.log('\nDocument was verified successfully!');
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tecnologia di firma dei documenti all'avanguardia"
  description: "GroupDocs.Signature fornisce una soluzione completa per la verifica e la gestione delle firme in vari formati di ufficio. Offrendo sette tipi di firme e operazioni CRUD complete, consente una gestione dei documenti e una sicurezza dei contenuti senza soluzione di continuità."
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "Caratteristiche di verifica delle firme"
  features:
    # feature loop
    - title: "Firma facilmente documenti aziendali"
      content: "Applica firme digitali—sia basate su testo, immagini, codici a barre, metadati, timbri o certificati digitali—ai tuoi documenti in modo sicuro e personalizzato. GroupDocs.Signature for Node.js via Java garantisce una firma professionale e snella dei documenti aziendali."

    # feature loop
    - title: "Operazioni sul ciclo di vita della firma"
      content: "Ottieni il controllo totale sulle firme dei documenti. Elenca tutte le firme in un file, verifica la loro autenticità, aggiornale come richiesto o rimuovile completamente quando necessario, garantendo un corretto elaborazione dei documenti."

    # feature loop
    - title: "Assicura l'integrità dei documenti"
      content: "Sfrutta i certificati digitali per proteggere i tuoi documenti da modifiche non autorizzate. Utilizza i metadati per proteggere e tracciare il contenuto del documento, garantendo che rimanga intatto e riservato."

    # feature loop
    - title: "Firme native personalizzate"
      content: "Aggiungi firme native personalizzate come adesivi nei PDF o filigrane nei documenti Word. Queste opzioni personalizzabili consentono una gestione professionale e sicura dei documenti, perfettamente adatte a contesti aziendali."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Processo di verifica delle firme a barre"
      content: |
        Questo esempio illustra la metodologia per autenticare le firme a barre incorporate in un documento.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Invia il documento contenente le firme a barre
          const signature = new signatureLib.Signature('input.pdf');

          // Configura i parametri per convalidare i codici a barre rispetto al testo designato
          const options = new signatureLib.BarcodeVerifyOptions();
          options.setText('12345');
          options.setMatchType(signatureLib.TextMatchType.StartsWith);

          // Autenticare le firme precedentemente apposte sul documento
          const result = signature.verify(options);

          // Controlla il rapporto di validazione
          if (result.isValid()) {
              console.log('\nDocument was verified successfully!');
          }
          ```
        platform: "nodejs-java"
        copy_title: "Copia"
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
    title: "Funzionalità complete e firme supportate"
    exclude: "verify"
    description: "Esplora le capacità avanzate di GroupDocs.Signature, con un'ampia gamma di strumenti e operazioni di gestione delle firme per flussi di lavoro documentali ottimizzati."
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
    title: "Validazione completa delle firme per vari formati"
    exclude: "PDF"
    description: "GroupDocs.Signature for Node.js via Java semplifica la verifica delle firme attraverso molteplici formati di documento, offrendo controlli robusti per i controlli delle firme. Personalizza il processo di verifica e assicurati che i documenti siano firmati correttamente."
    items: 
          
        # format loop 1
        - name: "Verifica firme PDF"
          format: "PDF"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "Verifica firme DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/verify/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "Verifica firme PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/verify/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 4
        - name: "Valida firme XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---