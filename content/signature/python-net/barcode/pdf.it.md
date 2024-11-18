



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:07
draft: false
lang: it
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Incorpora un codice a barre nel tuo PDF con Python"
head_description: "Aggiungi efficientemente firme con codice a barre ai documenti PDF con poche righe in Python. GroupDocs.Signature offre soluzioni di firma senza interruzioni per più formati di documenti."

############################# Header ############################
title: "Genera codici a barre per PDF" 
description: "Con GroupDocs.Signature for Python via .NET, puoi inserire codici a barre nei tuoi documenti aziendali ovunque sia necessario. La nostra soluzione offre opzioni flessibili per la personalizzazione della firma con codice a barre."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Prova gratuita"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Informazioni su GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) è un potente strumento di firma dei documenti che supporta un'ampia gamma di tipi di firma, tra cui testo, immagini, codici a barre, certificati digitali e timbri. Compatibile con oltre 60 formati di file, come PDF, MS Office, immagini, ZIP e altro, permette non solo di applicare firme, ma anche di cercare, verificare, modificare o rimuovere le firme secondo necessità.

############################# Steps ############################
steps:
    enable: true
    title: "Passaggi per generare e inserire un codice a barre in PDF"
    content: |
      [GroupDocs.Signature](/signature/python-net/) ti consente di generare e incorporare rapidamente codici a barre nei documenti PDF. Supportando più di 60 formati di codice a barre, le applicazioni Python via .NET possono integrare senza problemi la funzionalità di firma con codice a barre integrando la nostra libreria.
      
      1. Fornisci il file o lo stream PDF per l'elaborazione.
      2. Assegna il testo del codice a barre all'oggetto BarcodeSignOptions.
      3. Regola le opzioni del codice a barre, come posizione e dimensioni.
      4. Salva il documento con il codice a barre incorporato.
   
    code:
      platform: "python-net"
      copy_title: "Copia"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Firme di esempio"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Inizializza l'oggetto Signature con il percorso del documento
            with sg.Signature('input.pdf') as signature:

                # Usa BarcodeSignOptions per aggiungere un codice a barre al documento
                options = sg.BarcodeSignOptions('Business data')

                # Imposta il tipo di codice a barre e configura le sue proprietà
                options.EncodeType = sg.BarcodeTypes.Code128
                options.Left = 50
                options.Top = 150

                # Salva il documento firmato
                result = signature.Sign('output.pdf', options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Migliora i tuoi documenti con funzionalità avanzate di firma"
  description: "La libreria GroupDocs.Signature for Python via .NET fornisce soluzioni complete per firmare e elaborare documenti nei formati più comunemente usati. Puoi aggiungere, modificare, verificare o rimuovere vari tipi di firma per soddisfare le tue esigenze."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firma documentale flessibile"
      content: "Firma qualsiasi pagina nei documenti supportati con testo, immagini, codici a barre, codici QR o timbri. Aggiungi metadati nascosti come i dati EXIF nelle immagini e garantisci la protezione del contenuto con certificati digitali per impedire modifiche non autorizzate."

    # feature loop
    - title: "Cerca e verifica le firme"
      content: "Il nostro strumento garantisce l'integrità dei tuoi documenti consentendo la verifica delle firme. Puoi anche recuperare un elenco completo di tutte le firme in un documento per una gestione semplice."

    # feature loop
    - title: "Modifica le firme senza sforzo"
      content: "Modifica facilmente le firme esistenti. Regola il testo, riposiziona gli elementi o cambia i colori per adattarli alle esigenze del tuo documento."

    # feature loop
    - title: "Rimuovi le firme senza difficoltà"
      content: "Con funzionalità CRUD complete, GroupDocs.Signature for Python via .NET rende facile rimuovere qualsiasi firma indesiderata o obsoleta dai tuoi documenti."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Crea e posiziona una firma con codice a barre"
      content: |
        Questo esempio dimostra come inserire un codice a barre personalizzato in un documento PDF.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Fornisci il documento da firmare
              with sg.Signature('input.pdf') as signature:

                  # Imposta il testo del codice a barre e le opzioni di firma
                  options = sg.BarcodeSignOptions('Accepted')
                  options.EncodeType = sg.BarcodeTypes.Code39FullASCII

                  # Scegli la posizione per il codice a barre sulla pagina
                  options.VerticalAlignment = sg.VerticalAlignment.Top
                  options.HorizontalAlignment = sg.HorizontalAlignment.Left

                  # Imposta il padding tra il codice a barre e il bordo della pagina
                  options.Margin = sg.Padding()
                  options.Margin.Top = 180
                  options.Margin.Right = 20

                  # Specifica il colore delle barre del codice a barre
                  options.ForeColor = sg.Color.Red

                  # Scegli lo stile del carattere per il messaggio del codice a barre
                  options.Font = sg.SignatureFont()
                  options.Font.Size = 12
                  options.Font.FamilyName = 'Arial'

                  # Imposta la posizione del testo del messaggio
                  options.CodeTextAlignment = sg.CodeTextAlignment.Above

                  # Firma e salva il documento
                  result = signature.Sign('output.pdf', options)
          ```
        platform: "python-net"
        copy_title: "Copia"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "clicca per copiare"
          copy_done: "copiato"
        top_links:
          #  loop
          - title: "Scarica il risultato"
            icon: "download"
            link: "/examples/signature/formats/signature_barcode.pdf"
        links:
          #  loop
          - title: "Altri esempi"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "Documentazione"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Prova gratuitamente le funzionalità di GroupDocs.Signature o richiedi una licenza."
  items:
    #  loop
    - title: "Download di PyPi"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "Licenze"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Esplora le nostre funzionalità principali"
    exclude: "barcode"
    description: "Offriamo una vasta gamma di opzioni e operazioni per le tue esigenze documentali."
    items: 
          
        # operation loop 1
        - name: "Firme elettroniche"
          operation: "esign"
          link: "/signature/python-net/esign/pdf/"
          description: "Aggiungi vari tipi di firme ai formati di file supportati"

        # operation loop 2
        - name: "Aggiungi testo ai documenti"
          operation: "text"
          link: "/signature/python-net/text/pdf/"
          description: "Migliora il contenuto del documento con firme testuali personalizzabili"

        # operation loop 3
        - name: "Firme con immagine"
          operation: "image"
          link: "/signature/python-net/image/pdf/"
          description: "Posiziona qualsiasi immagine in qualsiasi punto di un documento"

        # operation loop 4
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/signature/python-net/barcode/pdf/"
          description: "Crea e inserisci vari codici a barre nei documenti supportati"

        # operation loop 5
        - name: "Genera QR code"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Genera e QR code, incluso QR code, per la firma dei documenti"
          
        # operation loop 6
        - name: "Certificati digitali"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "Proteggi documenti commerciali e firmali con certificati digitali"

        # operation loop 7
        - name: "Firme a timbro"
          operation: "stamp"
          link: "/signature/python-net/stamp/pdf/"
          description: "Utilizza il Costruttore di Timbri per creare timbri personalizzati rotondi o quadrati"
          
        # operation loop 8
        - name: "Cerca firme"
          operation: "search"
          link: "/signature/python-net/search/pdf/"
          description: "Trova qualsiasi firma precedentemente aggiunta all'interno di un documento"
          
        # operation loop 9
        - name: "Verifica delle firme"
          operation: "verify"
          link: "/signature/python-net/verify/pdf/"
          description: "Verifica l'autenticità delle firme dopo che sono state applicate"
          
        # operation loop 10
        - name: "Modifica firme"
          operation: "modify"
          link: "/signature/python-net/modify/pdf/"
          description: "Modifica facilmente una varietà di firme all'interno di un documento"
          
        # operation loop 11
        - name: "Elimina firme"
          operation: "delete"
          link: "/signature/python-net/delete/pdf/"
          description: "Rimuovi un'ampia gamma di firme precedentemente applicate"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Firma documenti in più formati"
    exclude: "PDF"
    description: "L'API Python via .NET supporta la firma di oltre 60 formati di file, consentendoti di aggiungere vari tipi di firme a qualsiasi pagina o posizione specifica all'interno dei tuoi documenti."
    items: 
          
        # format loop 1
        - name: "Aggiungi codice a barre a PDF"
          format: "PDF"
          link: "/signature/python-net/barcode/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "Aggiungi codice a barre a DOCX"
          format: "DOCX"
          link: "/signature/python-net/barcode/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "Aggiungi codice a barre a JPEG"
          format: "JPEG"
          link: "/signature/python-net/barcode/jpeg/"
          description: "Immagine JPEG"
          
        # format loop 4
        - name: "Aggiungi codice a barre a PPTX"
          format: "PPTX"
          link: "/signature/python-net/barcode/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 5
        - name: "Aggiungi codice a barre a XLSX"
          format: "XLSX"
          link: "/signature/python-net/barcode/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---