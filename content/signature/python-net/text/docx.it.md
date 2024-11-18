



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:56
draft: false
lang: it
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Aggiungi firme testuali a DOCX utilizzando Python"
head_description: "Sfrutta l'API Python per incorporare firme testuali nei file DOCX, supportando formati come PDF, Word, Excel, PowerPoint, immagini e ZIP."

############################# Header ############################
title: "Aggiungi facilmente firme testuali a DOCX" 
description: "Integra senza sforzo firme testuali personalizzate nei tuoi documenti utilizzando GroupDocs.Signature for Python via .NET. Semplifica i tuoi flussi di lavoro con opzioni di personalizzazione flessibili delle firme."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Provalo gratis oggi"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Scopri la potenza di GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) offre una piattaforma completa per incorporare firme testuali personalizzabili, rendendo più fluide le operazioni documentali. Personalizza il contenuto e l'aspetto delle firme nei documenti per aumentare l'efficienza e migliorare la gestione dei documenti.

############################# Steps ############################
steps:
    enable: true
    title: "Come creare firme testuali DOCX con Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) consente una facile integrazione delle firme testuali nei file DOCX all'interno delle applicazioni Python via .NET. Aggiungi rapidamente funzionalità ai tuoi prodotti con questa soluzione.
      
      1. Fornisci il documento DOCX al costruttore Signature.
      2. Crea TextSignOptions con il tuo testo della firma.
      3. Imposta le proprietà visive della firma.
      4. Inserisci la firma sulle pagine desiderate del documento.
   
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

            # Inizializza la Signature con il percorso del documento
            with sg.Signature('input.docx') as signature:

                # Configura TextSignOptions con il testo della firma desiderato
                options = sg.TextSignOptions("Approved")

                # Scegli il colore e il font per la firma
                options.ForeColor = sg.Color.Red
                options.Font = sg.SignatureFont()
                options.Font.Size = 12
                options.Font.FamilyName = "Comic Sans MS"

                # Applica la firma testuale al documento
                result = signature.Sign("output.docx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Gestione completa delle firme testuali"
  description: "GroupDocs.Signature for Python via .NET ti aiuta a gestire i flussi di lavoro documentali aggiungendo firme testuali personalizzate a formati popolari. Controlla facilmente l'aspetto, la posizione e il contenuto delle firme per soddisfare le tue esigenze."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Scopri le funzionalità di GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firme documentali flessibili"
      content: "Aggiungi vari tipi di firme — testuali, immagini, codici a barre, codici QR e timbri — a qualsiasi pagina del documento. Usa i metadati per includere informazioni nascoste e proteggere i tuoi file con certificati digitali."

    # feature loop
    - title: "Verifica e cerca firme"
      content: "Utilizza strumenti avanzati per controllare l'integrità dei tuoi documenti firmati. Cerca e analizza tutte le firme in un file per ulteriori validazioni."

    # feature loop
    - title: "Modifica o rimuovi firme"
      content: "Aggiorna facilmente il contenuto, l'aspetto o la posizione delle firme esistenti. Rimuovi firme obsolete per mantenere i tuoi documenti aggiornati."

    # feature loop
    - title: "Firme testuali specializzate"
      content: "Applica firme testuali specifiche per documento, come filigrane per file Word o timbri per PDF, aggiungendo un ulteriore livello di controllo e personalizzazione."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Aggiungi firme testuali ai documenti"
      content: |
        Scopri come incorporare firme testuali nei documenti per ottimizzare i tuoi processi.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Seleziona il documento da firmare
              with sg.Signature('input.docx') as signature:

                    # Configura le opzioni testuali con il contenuto desiderato
                    options = sg.TextSignOptions("Rescheduled to 03/04/2025")

                    # Definisci le dimensioni e la posizione della firma
                    options.Left = 100
                    options.Top = 180
                    options.Width = 230
                    options.Height = 30

                    # Imposta il padding dai margini della pagina
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Scegli il colore del testo e lo stile del font
                    options.ForeColor = sg.Color.Red
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Aggiungi un bordo attorno alla firma testuale
                    options.Border = sg.Border()
                    options.Border.Color = sg.Color.Red
                    options.Border.DashStyle = sg.DashStyle.DashLongDashDot
                    options.Border.Transparency = 0.5
                    options.Border.Visible = True
                    options.Border.Weight = 2

                    # Personalizza lo sfondo se necessario
                    options.Background = sg.Background()
                    options.Background.Color = sg.Color.Yellow
                    options.Background.Transparency = 0.8

                    # Facoltativamente salva la firma come immagine per compatibilità
                    options.SignatureImplementation = sg.TextSignatureImplementation.Image

                    # Salva il documento con la firma incorporata
                    result = signature.Sign("output.docx", options)
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
            link: "/examples/signature/formats/signature_text.docx"
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
    title: "Funzionalità avanzate delle firme"
    exclude: "text"
    description: "La nostra API supporta la gestione completa del ciclo di vita per sette tipi di firme, permettendoti di creare, gestire, verificare e personalizzare le tue firme con efficienza."
    items: 
          
        # operation loop 1
        - name: "Firme elettroniche"
          operation: "esign"
          link: "/signature/python-net/esign/docx/"
          description: "Aggiungi vari tipi di firme ai formati di file supportati"

        # operation loop 2
        - name: "Aggiungi testo ai documenti"
          operation: "text"
          link: "/signature/python-net/text/docx/"
          description: "Migliora il contenuto del documento con firme testuali personalizzabili"

        # operation loop 3
        - name: "Firme con immagine"
          operation: "image"
          link: "/signature/python-net/image/docx/"
          description: "Posiziona qualsiasi immagine in qualsiasi punto di un documento"

        # operation loop 4
        - name: "Genera codici a barre"
          operation: "barcode"
          link: "/signature/python-net/barcode/docx/"
          description: "Crea e inserisci vari codici a barre nei documenti supportati"

        # operation loop 5
        - name: "Genera QR code"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/docx/"
          description: "Genera e QR code, incluso QR code, per la firma dei documenti"
          
        # operation loop 6
        - name: "Certificati digitali"
          operation: "digital"
          link: "/signature/python-net/digital/docx/"
          description: "Proteggi documenti commerciali e firmali con certificati digitali"

        # operation loop 7
        - name: "Firme a timbro"
          operation: "stamp"
          link: "/signature/python-net/stamp/docx/"
          description: "Utilizza il Costruttore di Timbri per creare timbri personalizzati rotondi o quadrati"
          
        # operation loop 8
        - name: "Cerca firme"
          operation: "search"
          link: "/signature/python-net/search/docx/"
          description: "Trova qualsiasi firma precedentemente aggiunta all'interno di un documento"
          
        # operation loop 9
        - name: "Verifica delle firme"
          operation: "verify"
          link: "/signature/python-net/verify/docx/"
          description: "Verifica l'autenticità delle firme dopo che sono state applicate"
          
        # operation loop 10
        - name: "Modifica firme"
          operation: "modify"
          link: "/signature/python-net/modify/docx/"
          description: "Modifica facilmente una varietà di firme all'interno di un documento"
          
        # operation loop 11
        - name: "Elimina firme"
          operation: "delete"
          link: "/signature/python-net/delete/docx/"
          description: "Rimuovi un'ampia gamma di firme precedentemente applicate"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Incorpora firme testuali in più formati"
    exclude: "DOCX"
    description: "Con l'API Python via .NET, puoi aggiungere firme testuali a vari documenti Office, dandoti il pieno controllo sul ciclo di vita del documento e migliorando la sicurezza."
    items: 
          
        # format loop 1
        - name: "Firme testuali PDF"
          format: "PDF"
          link: "/signature/python-net/text/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "Firme testuali DOCX"
          format: "DOCX"
          link: "/signature/python-net/text/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "Firme testuali JPEG"
          format: "JPEG"
          link: "/signature/python-net/text/jpeg/"
          description: "Immagine JPEG"
          
        # format loop 4
        - name: "Firme testuali PPTX"
          format: "PPTX"
          link: "/signature/python-net/text/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 5
        - name: "Firme testuali XLSX"
          format: "XLSX"
          link: "/signature/python-net/text/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---