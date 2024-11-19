



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:23
draft: false
lang: it
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Genera codici QR per file JPEG utilizzando Python"
head_description: "Utilizza l'API GroupDocs.Signature per generare e incorporare codici QR nei file JPEG. Posiziona facilmente i codici QR su qualsiasi pagina per aggiungere funzionalità extra."

############################# Header ############################
title: "Genera codici QR per JPEG" 
description: "Crea senza sforzo codici a barre 2D utilizzando dati testuali o numerici e applicali a varie pagine e formati, inclusi PDF, Word, Excel e altri con GroupDocs.Signature for Python via .NET."
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
    title: "Scopri le funzionalità di GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) offre una vasta gamma di funzionalità, consentendo agli utenti di generare e incorporare diversi tipi di firma nei principali formati di documento. Che si tratti di PDF, Word, Excel, PowerPoint o immagini, arricchisci i tuoi documenti con firme di Testo, Immagine, Codice a barre, Codice QR, Metadati, Digitale o Timbro.

############################# Steps ############################
steps:
    enable: true
    title: "Passaggi per generare e inserire un codice QR in JPEG"
    content: |
      [GroupDocs.Signature](/signature/python-net/) ti consente di creare codici QR in formati popolari e posizionarli sulle pagine di JPEG. Con supporto per oltre 10 tipi di codici QR, puoi integrare senza soluzione di continuità questa funzionalità nelle applicazioni Python via .NET. Arricchisci i tuoi documenti con firme di codici QR utilizzando il nostro prodotto.
      
      1. Ottieni il file o lo stream JPEG in cui verrà aggiunto il codice QR.
      2. Fornisci il testo richiesto a QrCodeSignOptions.
      3. Personalizza le impostazioni visive come colore, posizione e dimensione.
      4. Salva il documento con il codice QR incorporato.
   
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

            # Inizializza una nuova istanza di Signature con il documento
            with sg.Signature('input.jpeg') as signature:

                # Usa QrCodeSignOptions per incorporare un codice QR nel documento
                options = sg.QrCodeSignOptions("Text Content")

                # Specifica il tipo di firma e imposta la sua posizione sulla pagina
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # Salva il documento con il codice QR incorporato
                result = signature.Sign("output.jpeg", options)
        ```                 

############################# More features ############################
more_features:
  enable: true
  title: "Integrazione completa delle firme per i documenti"
  description: "Con l'API GroupDocs.Signature for Python via .NET, gli utenti possono generare, modificare, cercare, convalidare e rimuovere diversi tipi di firma, semplificando i flussi di lavoro documentali con precisione."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Funzionalità chiave di GroupDocs.Signature"
  features:
    # feature loop
    - title: "Applica più tipi di firma"
      content: "GroupDocs.Signature consente l'applicazione di firme di Testo, Immagine, Codice a barre, Codice QR e Timbro a qualsiasi documento. Puoi posizionare con precisione le firme su qualsiasi pagina e gestire facilmente i metadati. Proteggi i tuoi documenti da modifiche non autorizzate con certificati digitali."

    # feature loop
    - title: "Cerca e convalida firme"
      content: "Verifica l'autenticità e l'accuratezza delle firme dei documenti utilizzando strumenti di convalida avanzati. Ottieni facilmente un elenco dettagliato di tutte le firme incorporate in un documento per una migliore supervisione."

    # feature loop
    - title: "Modifica firme esistenti"
      content: "Puoi aggiornare firme precedentemente applicate modificando contenuto, posizione, colore, dimensione e altri attributi per adattarli alle tue esigenze specifiche."

    # feature loop
    - title: "Rimuovi facilmente firme"
      content: "Semplifica la gestione dei documenti rimuovendo rapidamente le firme indesiderate. Che si tratti di un certificato digitale o di un altro tipo di firma, la rimozione può essere effettuata in modo efficiente."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Personalizza un codice QR generato"
      content: |
        Questo esempio mostra come posizionare un codice QR personalizzato su una pagina JPEG.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Ottieni il documento da firmare e passalo a Signature
              with sg.Signature('input.jpeg') as signature:

                    # Configura le opzioni del codice QR con il testo richiesto
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # Imposta la posizione del codice QR sulla pagina
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # Imposta il margine per la firma
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Scegli il colore del codice QR
                    options.ForeColor = sg.Color.Red

                    # Definisci le opzioni di font per il messaggio
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Imposta il colore di sfondo e il pennello per il codice QR
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # Incorpora il codice QR nel documento
                    result = signature.Sign("output.jpeg", options)
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
            link: "/examples/signature/formats/signature_qrcode.jpeg"
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
    title: "Esplora le nostre soluzioni di firma"
    exclude: "qrcode"
    description: "Offriamo una vasta gamma di tipi di firma e operazioni per soddisfare le tue esigenze documentali."
    items: 
          
        # operation loop 1
        - name: "Firme elettroniche"
          operation: "esign"
          link: "/signature/python-net/esign/jpeg/"
          description: "Aggiungi vari tipi di firme ai formati di file supportati"

        # operation loop 2
        - name: "Aggiungi testo ai documenti"
          operation: "text"
          link: "/signature/python-net/text/jpeg/"
          description: "Migliora il contenuto del documento con firme testuali personalizzabili"

        # operation loop 3
        - name: "Firme con immagine"
          operation: "image"
          link: "/signature/python-net/image/jpeg/"
          description: "Posiziona qualsiasi immagine in qualsiasi punto di un documento"

        # operation loop 4
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/signature/python-net/barcode/jpeg/"
          description: "Crea e inserisci vari codici a barre nei documenti supportati"

        # operation loop 5
        - name: "Genera QR code"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "Genera e QR code, incluso QR code, per la firma dei documenti"
          
        # operation loop 6
        - name: "Certificati digitali"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "Proteggi documenti commerciali e firmali con certificati digitali"

        # operation loop 7
        - name: "Firme a timbro"
          operation: "stamp"
          link: "/signature/python-net/stamp/jpeg/"
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
    title: "Incorpora codici QR in vari formati di documento"
    exclude: "JPEG"
    description: "Utilizza l'API Python via .NET per incorporare codici QR in qualsiasi formato di documento standard del settore. Archivia e codifica informazioni importanti in codici a barre 2D per una facile scansione e recupero dati."
    items: 
          
        # format loop 1
        - name: "QR-Code per PDF"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "QR-Code per DOCX"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "QR-Code per JPEG"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "Immagine JPEG"
          
        # format loop 4
        - name: "QR-Code per PPTX"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 5
        - name: "QR-Code per XLSX"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---