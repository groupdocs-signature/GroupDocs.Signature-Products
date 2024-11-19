



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:07
draft: false
lang: it
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Crea timbri rotondi e quadrati in DOCX utilizzando Python"
head_description: "Genera e inserisci timbri personalizzati nei file DOCX con l'API GroupDocs.Signature for Python via .NET."

############################# Header ############################
title: "Crea timbri per DOCX" 
description: "Aggiungi timbri progettati su misura in qualsiasi parte dei tuoi documenti con GroupDocs.Signature for Python via .NET, offrendo grande flessibilità per posizionamento e configurazione per soddisfare le tue esigenze aziendali."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica gratuitamente"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Panoramica di GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Scopri di più"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) è uno strumento completo che consente di inserire vari tipi di firme nei documenti, inclusi timbri personalizzati. Supportando oltre 60 formati file - da PDF e documenti Word a immagini e file ZIP - puoi arricchire i tuoi documenti con testo, immagini, codici a barre, metadati, certificati digitali e timbri. Hai anche il pieno controllo per cercare, verificare, modificare o eliminare tutte le firme applicate.

############################# Steps ############################
steps:
    enable: true
    title: "Come aggiungere un timbro a DOCX utilizzando Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) offre strumenti robusti per la creazione di timbri per migliorare le applicazioni Python via .NET. Usalo per progettare e implementare timbri personalizzati per le tue pagine documentali.
      
      1. Fornisci il documento DOCX che desideri timbrare.
      2. Usa StampSignOptions per configurare tutte le impostazioni necessarie.
      3. Aggiungi più linee di timbro se necessario.
      4. Applica il timbro e salva il documento aggiornato.
   
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

            # Allega il percorso del documento all'istanza di Signature
            with sg.Signature('input.docx') as signature:

                # Configura StampSignOptions con i dettagli del timbro richiesti
                options = sg.StampSignOptions()
                options.Height = 180
                options.Width = 180

                # Aggiungi una o più linee al timbro
                outerLine = sg.StampLine()
                outerLine.Text = "* The Best Company *"
                outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                outerLine.Font = sg.SignatureFont()
                outerLine.Font.Size = 12
                outerLine.Font.FamilyName = "Arial"
                outerLine.Height = 22
                outerLine.TextBottomIntent = 6
                outerLine.TextColor = sg.Color.WhiteSmoke
                outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                options.OuterLines.Add(outerLine)

                # Salva il documento con il timbro applicato
                result = signature.Sign("output.docx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Utilizza le firme per garantire e migliorare l'integrità dei documenti"
  description: "Con la libreria GroupDocs.Signature for Python via .NET, puoi aggiungere facilmente funzionalità di firma ai tuoi documenti. Crea, modifica, verifica o elimina timbri personalizzati e altri tipi di firme, fornendo flessibilità e sicurezza ai tuoi flussi di lavoro documentali."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Firme a timbro alimentate da GroupDocs.Signature"
  features:
    # feature loop
    - title: "Firma completa dei documenti"
      content: "Migliora i tuoi documenti aggiungendo firme come testo, immagini, codici a barre, codici QR e timbri in qualsiasi posizione su qualsiasi pagina. Gestisci i metadati incorporati e applica certificati digitali per proteggerti da modifiche non autorizzate."

    # feature loop
    - title: "Ricerca e verifica delle firme efficienti"
      content: "Dopo la firma, utilizza strumenti di ricerca avanzata per trovare tutte le firme incorporate. Verifica o gestisci facilmente i dati delle firme per garantire l'integrità del documento."

    # feature loop
    - title: "Modifica e personalizza le firme"
      content: "Apporta modifiche alle firme precedentemente aggiunte. Che tu voglia cambiare il contenuto, la posizione, la dimensione o il colore, GroupDocs.Signature for Python via .NET ti offre il pieno controllo per regolare le firme secondo necessità."

    # feature loop
    - title: "Rimuovi facilmente le firme"
      content: "Se hai bisogno di rimuovere firme, GroupDocs.Signature for Python via .NET offre tutti gli strumenti necessari per eliminare qualsiasi tipo, inclusi timbri e certificati digitali, aiutandoti a mantenere i tuoi documenti aggiornati e conformi."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Come aggiungere timbri personalizzati ai documenti"
      content: |
        Questo esempio mostra come creare e inserire timbri personalizzati con dettagli di testo specifici in un documento.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Fornisci il documento che desideri timbrare
              with sg.Signature('input.docx') as signature:

                    # Configura le opzioni del timbro con le impostazioni desiderate
                    options = sg.StampSignOptions()

                    # Definisci la dimensione e il posizionamento del timbro sulla pagina
                    options.Height = 200
                    options.Width = 200
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right
                    options.AllPages = True

                    # Aggiungi linee circolari esterne con testo
                    outerLine = sg.StampLine()
                    outerLine.Text = "* The best  choice *"
                    outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                    outerLine.Font = sg.SignatureFont()
                    outerLine.Font.Size = 12
                    outerLine.Font.FamilyName = "Arial"
                    outerLine.Height = 22
                    outerLine.TextBottomIntent = 6
                    outerLine.TextColor = sg.Color.WhiteSmoke
                    outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                    options.OuterLines.Add(outerLine)

                    # Facoltativamente, aggiungi linee quadrate interne
                    innerLine = sg.StampLine()
                    innerLine.Text = "Company #1"
                    innerLine.TextColor = sg.Color.MediumVioletRed
                    innerLine.Font = sg.SignatureFont()
                    innerLine.Font.Size = 20
                    innerLine.Font.Bold = True
                    innerLine.Height = 40
                    options.InnerLines.Add(innerLine)

                    # Finalizza e salva il documento timbrato
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
            link: "/examples/signature/formats/signature_stamp.docx"
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
    title: "Esplora le funzionalità chiave"
    exclude: "stamp"
    description: "Trova una vasta gamma di opzioni per creare, gestire e rimuovere firme, dandoti pieno controllo sui flussi di lavoro documentali."
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
    title: "Applica timbri a vari formati di documento"
    exclude: "DOCX"
    description: "Con l'API GroupDocs.Signature, puoi inserire timbri personalizzati in oltre 60 tipi di file standard. Applica facilmente timbri ovunque nei tuoi documenti, migliorando la personalizzazione e il tracciamento."
    items: 
          
        # format loop 1
        - name: "Apponi timbro su PDF"
          format: "PDF"
          link: "/signature/python-net/stamp/pdf/"
          description: "Formato di Documento Portabile Adobe"
          
        # format loop 2
        - name: "Apponi timbro su DOCX"
          format: "DOCX"
          link: "/signature/python-net/stamp/docx/"
          description: "Documento Open XML di Microsoft Word"
          
        # format loop 3
        - name: "Apponi timbro su JPEG"
          format: "JPEG"
          link: "/signature/python-net/stamp/jpeg/"
          description: "Immagine JPEG"
          
        # format loop 4
        - name: "Apponi timbro su PPTX"
          format: "PPTX"
          link: "/signature/python-net/stamp/pptx/"
          description: "Presentazione Open XML di PowerPoint"
          
        # format loop 5
        - name: "Apponi timbro su XLSX"
          format: "XLSX"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Foglio di Calcolo Open XML di Microsoft Excel"


          

---