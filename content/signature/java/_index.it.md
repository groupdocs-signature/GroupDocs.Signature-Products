---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API per la firma digitale Java, aggiungi la firma elettronica all'immagine PDF Word Excel"
head_description: "API di firma digitale Java. Libreria di firme elettroniche per firmare digitalmente PDF, Microsoft Word, fogli di calcolo Excel, presentazioni PowerPoint e formati di documenti immagine."

############################# Header ############################
title: "API Java per la gestione delle firme digitali"
description: "Gestisci la firma elettronica di tipi di immagini, codici QR, codici a barre, metadati, testo e timbri nelle applicazioni Java per la firma di immagini e formati di file di documenti digitali."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Panoramica"

            # button loop
            - link: "#features"
              text: "Caratteristiche"

            # button loop
            - link: "#support"
              text: "Supporto"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Dimostrazione dal vivo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Prezzi"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature per Java API ti aiuta a sviluppare applicazioni Java con funzionalità di firma elettronica per firmare documenti digitali di formati supportati senza installare alcun software esterno. Supporta la manipolazione e la gestione di vari tipi di firme elettroniche come immagine, codice a barre, codice QR, timbro, testo, ottica e metadati. Tutti i tuoi documenti commerciali elettronici come Microsoft Office Word, presentazioni PowerPoint, fogli di calcolo Excel, immagini e file PDF possono essere firmati digitalmente personalizzando le proprietà della firma, ad es. ombra, dimensioni, allineamento e altro secondo le tue esigenze. La libreria della firma digitale è semplice e leggera, costituita da un singolo file DLL che può essere facilmente integrato all'interno di un'applicazione Java nuova o esistente.  

      Tramite GroupDocs.Signature per l'API Java è possibile caricare tutti i certificati registrati dal sistema o individuare le firme esistenti utilizzando la ricerca semplice e avanzata. Le opzioni per lavorare con documenti protetti da password, specificando proprietà di firma comuni (dimensioni del testo, opacità, rotazione, verifica, proprietà dei caratteri, opzioni di colore, numero di pagina, larghezza, in alto, a sinistra ecc.) e il supporto per l'implementazione di diversi tipi di firma elettronica lo rendono affidabile Soluzione per la gestione delle firme elettroniche per documenti digitali.  

      GroupDocs.Signature per Java è compatibile con tutte le versioni Java e supporta i sistemi operativi più diffusi (Windows, Linux, MacOS) in grado di eseguire il runtime Java
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Questa è una panoramica delle funzionalità di GroupDocs.Signature per Java:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Tipi di firma"
          content: |
            * Firma del testo
            * Firma dell'immagine
            * Firme digitali
            * Firma del codice QR
            * Firma del codice a barre
            * Timbro Firma
            * Firma del campo modulo
      
      ## TAB TWO ##
      tab_two:
        description: |
          L'API di firma elettronica Java supporta [formati di file di documenti](https://docs.groupdocs.com/signature/java/supported-document-formats/) come elencato di seguito.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Other Formats"
              content: |
                * **immagini**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Metafile**: EMF, WMF, CMX
                * **Portatile**: PDF
                * **Grafica vettoriale scalabile**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Altri**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature per Java supporta i seguenti sistemi operativi, framework e gestori di pacchetti:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Sistemi operativi"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Framework supportati"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Ambienti di sviluppo"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Costruisci lo strumento di automazione"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "Funzionalità di GroupDocs.Signature per Java"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Crea, leggi, modifica, nascondi ed elimina firme elettroniche dai formati di documenti supportati"

      # feature loop
      - icon: "fas fa-eye"
        content: "Accesso al documento firmato da flusso, percorso relativo o percorso assoluto"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Applica la firma del testo a documenti, fogli di calcolo, presentazioni, immagini e file PDF"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Aggiungi la firma del testo come annotazione, adesivo, immagine ai file PDF e configura anche lo stile e il colore"

      # feature loop
      - icon: "fas fa-code"
        content: "Firma documento PDF, file immagine e ottieni l'output in diversi formati di file"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Firma digitalmente le immagini con la firma del testo come filigrana e aggiungi trasparenza, rotazione alla firma elettronica"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Cerca certificati e firma documenti Microsoft Word, Excel e PDF con certificati digitali"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Firma formati di documenti di elaborazione testi con filigrane di testo nativo"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Usa QR-Code, Barcode per firmare file Word, Slide, Cell, PDF e immagini"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Configura e applica le firme dei timbri per proteggere i formati di file supportati"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Imposta e assegna firme di immagini a documenti, fogli di calcolo, presentazioni, immagini e file PDF"

      # feature loop
      - icon: "fas fa-columns"
        content: "Configura le proprietà della firma, ad es. Look and Feel, Margini, Allineamento, ecc."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Applicare la firma digitale al documento protetto da password"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Esegui la verifica del testo dei documenti PDF utilizzando il gestore della firma"

      # feature loop
      - icon: "fas fa-print"
        content: "Verifica digitale di documenti Word, Cell, PDF con contenitori di certificati .CER e .PFX"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Specifica diversi tipi di unità di misura (ad es. millimetri, pixel ecc.) per le firme di testo PDF"

      # feature loop
      - icon: "fas fa-lock"
        content: "Ottieni informazioni sul documento tramite file o URL: aggiungi le firme dei campi modulo ai documenti PDF"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Aggiungi oggetto dati personalizzato, VCard incorporata, e-mail, EPC, MeCard o oggetto evento al codice QR"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Applicare diversi stili di pennello alle firme, ad esempio pennello sfumato, radiale, solido e texture"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Firma il documento che si trova su FTP o Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Imposta l'allineamento del testo all'interno delle forme per documenti, diapositive, immagini e file PDF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Cerca, verifica e firma digitalmente documenti di presentazione PowerPoint"

      # feature loop
      - icon: "fas fa-cube"
        content: "Posiziona la firma utilizzando i pixel nei documenti delle celle e il posizionamento del testo per le firme dei timbri"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Implementa la firma del timbro rettangolare con angoli arrotondati"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Estendi le firme di codici a barre e codici QR con contenuti di dati immagine"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Aggiungi firme di metadati crittografati mentre lavori con le opzioni di firma e ricerca"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Incorpora oggetti personalizzati nelle firme dei metadati all'interno di Word, Excel e presentazioni"

    more_feature:
      # more_feature_loop
      - title: "Configura e applica facilmente le firme elettroniche"
        content: |
          L'API GroupDocs.Signature per Java consente di configurare e aggiungere firme elettroniche ai formati di documenti supportati. Di seguito è riportato un esempio di codice che mostra quanto sia semplice applicare una firma di testo a un file PDF:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // impostare la posizione della firma
          options.setLeft(100);
          options.setTop(100);
          
          // imposta il rettangolo della firma
          options.setWidth(100);
          options.setHeight(30);

          // imposta il colore del testo e il carattere
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // firmare il documento da archiviare
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Tipi di codifica di codici a barre supportati per la firma elettronica"
        content: |
          Utilizzando GroupDocs.Signature per l'API Java è possibile applicare codici a barre e codici QR ai formati di file supportati. GroupDocs.Signature per Java supporta una vasta gamma di tipi di codifica di codici a barre per soddisfare la maggior parte delle esigenze. I tipi di codifica di codici a barre supportati includono Code 11, Code 128, Code 16K/32, Databar codes, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard e Codice39 esteso.

          Analogamente, l'API GroupDocs.Signature per Java consente di utilizzare tipi di codice QR, ad esempio QR, Aztec e Data Matrix. I tipi di codifica QR-Code supportati includono Aztec, DataMatrix, GS1 DataMatrix e GS1 QR.

      # more_feature_loop
      - title: "Cerca firme e certificati"
        content: |
          Tramite GroupDocs.Signature per l'API Java, puoi cercare le firme di codici QR e codici a barre in qualsiasi documento, presentazione, foglio di calcolo, immagine e file PDF e recuperare il risultato della ricerca. Puoi anche cercare oggetti di dati personalizzati da documenti firmati con la firma del codice QR, nonché cercare VCard standard e oggetto e-mail da documenti firmati con codice QR. È supportata anche la verifica del testo crittografato delle firme QR-Code e la ricerca della firma dei metadati nei documenti PDF. Applica criteri di ricerca aggiuntivi per le firme digitali dei documenti Words & Cells.  

          L'opzione di ricerca è disponibile anche per la firma dei metadati per documenti word, diapositive e fogli di calcolo, mentre la ricerca nel campo modulo è disponibile per i documenti PDF.

      # more_feature_loop
      - title: "Configurare le proprietà della firma elettronica"
        content: |
          Per migliorare l'esperienza utente degli utenti finali, GroupDocs.Signature for Java API fornisce molte proprietà che possono essere configurate abbastanza facilmente. È possibile impostare le opzioni di carattere e colore (Colore di sfondo, Colore di primo piano, Grassetto, Corsivo, Sottolineato, Famiglia di caratteri, Dimensione carattere ecc.), Opzioni di sfondo e bordo (Colore di sfondo, Trasparenza sfondo, Colore bordo, Stile tratteggio bordo, Spessore bordo, Trasparenza bordo ecc.), Margini firma (sinistro, superiore, larghezza, altezza, riempimento ecc.) e Impostazione area firma immagine e allineamento firma (allineamento orizzontale, allineamento verticale ecc.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature offre API per la visualizzazione di documenti per altri ambienti di sviluppo popolari"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---