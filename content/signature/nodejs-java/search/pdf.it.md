



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:13
draft: false
lang: it
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Cerca firme elettroniche in file PDF con JavaScript"
head_description: "Sfrutta la potenza dell'API GroupDocs.Signature for Node.js via Java per rilevare e cercare firme elettroniche in PDF, documenti Word, fogli di calcolo Excel, presentazioni e immagini."

############################# Header ############################
title: "Cerca firme elettroniche in PDF" 
description: "Scopri e recupera informazioni dettagliate su tutte le firme incorporate in file PDF, Word, Excel, presentazioni e immagini utilizzando gli strumenti avanzati forniti da GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Inizia subito gratuitamente"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Panoramica di GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) offre un framework robusto per gestire le firme digitali attraverso un'ampia gamma di tipi di file. Supportando oltre 60 formati come PDF, documenti Microsoft Office, immagini e file ZIP, l'API consente agli utenti di applicare, localizzare, verificare, aggiornare o rimuovere una varietà di tipi di firme, tra cui testo, immagini, codici a barre, certificati digitali e altro ancora.

############################# Steps ############################
steps:
    enable: true
    title: "Guida alla ricerca di firme in PDF utilizzando JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) fornisce uno strumento potente per localizzare firme digitali all'interno di file PDF. Gli sviluppatori Node.js via Java possono ampliare facilmente la funzionalità delle loro applicazioni con la nostra soluzione.
      
      1. Specifica il percorso del file PDF per la ricerca delle firme.
      2. Utilizza SearchOptions per filtrare i risultati della ricerca.
      3. Esegui il metodo Search per trovare le firme.
      4. Esamina l'elenco delle firme scoperte.
   
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

        // Instanzia un oggetto Signature utilizzando il percorso del documento
        const signature = new signatureLib.Signature('input.pdf');

        // Configura TextSearchOptions per includere ogni pagina
        const options = new signatureLib.TextSearchOptions();
        options.setAllPages(true);

        // Esegui una ricerca per localizzare tutte le firme testuali all'interno del documento
        const signatures = signature.search(signatureLib.TextSignature.class, options).toArray();
        console.log(`\nSource document contains the following text signature(s).`);

        // Aggrega le firme scoperte per un'analisi completa
        for (const textSignature of signatures) {
            console.log(`Found Text signature at page ${textSignature.getPageNumber()} 
            with type [${textSignature.getSignatureImplementation()}] and text '${textSignature.getText()}'.`);
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Soluzione completa per la gestione delle firme"
  description: "GroupDocs.Signature for Node.js via Java fornisce una soluzione all-in-one per aggiungere, modificare, cercare e verificare firme elettroniche attraverso i formati di documenti più popolari. Potenzia i tuoi flussi di lavoro con funzionalità avanzate di firma dei documenti."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Caratteristiche di rilevamento delle firme"
  features:
    # feature loop
    - title: "Firmare digitalmente file aziendali"
      content: "Aggiungi firme elettroniche come testo, immagini, codici a barre e certificati digitali in qualsiasi posizione all'interno dei tuoi documenti. GroupDocs.Signature supporta la firma in PDF, Word, Excel, immagini e altro, garantendo una gestione flessibile dei documenti."

    # feature loop
    - title: "Gestione delle firme efficiente"
      content: "Dopo la firma, localizza facilmente tutte le firme incorporate all'interno di un documento. L'API consente una ricerca e un recupero completi delle firme, nonché la possibilità di aggiornarle o rimuoverle."

    # feature loop
    - title: "Sicurezza dei documenti e gestione dei metadati"
      content: "Proteggi l'integrità dei tuoi documenti incorporando o rimuovendo metadati nascosti. Proteggi i tuoi file da modifiche non autorizzate utilizzando certificati digitali per sigillare e autenticare il contenuto del documento."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Identificazione delle firme su immagine"
      content: |
        Questo esempio illustra come rilevare una firma su immagine all'interno di un documento specifico.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Fornisci il documento sorgente come parametro al costruttore
          const signature = new signatureLib.Signature('input.pdf');

          // Cerca eventuali firme che siano di tipo testo
          const signatures = signature.search(signatureLib.ImageSignature.class, signatureLib.SignatureType.Image).toArray();
          console.log(`\nSource document contains the following image signature(s).`);

          // Visualizza i risultati con le proprietà complete delle firme individuate
          for (const imageSignature of signatures) {
              console.log(`Found Image signature at page ${imageSignature.getPageNumber()} 
              and size ${imageSignature.getSize()}.`);
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
    title: "Funzionalità chiave"
    exclude: "search"
    description: "La nostra API completa offre una gamma di operazioni progettate per semplificare la gestione delle firme documentali, dalla firma alla post-elaborazione e verifica."
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
    title: "Localizza firme in più tipi di file"
    exclude: "PDF"
    description: "Con l'API GroupDocs.Signature for Node.js via Java, puoi cercare e recuperare efficientemente firme elettroniche da un'ampia gamma di formati di file supportati, facilitando l'integrazione nei tuoi flussi di lavoro documentali."
    items: 
          
        # format loop 1
        - name: "Cerca firme in PDF"
          format: "PDF"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "Trova firme in DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/search/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "Trova firme in PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/search/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 4
        - name: "Cerca firme in XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---