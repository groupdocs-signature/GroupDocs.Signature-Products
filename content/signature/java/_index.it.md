---
############################# Static ############################
layout: "landing"
date: 2024-09-25T12:45:24
draft: false

lang: it
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java" 
    # supported_platforms loop
    - title: "Python"
      tag: "python-net" 

############################# Head ############################
head_title: "Libreria di firme digitali Java - GroupDocs.Signature"
head_description: "Potenzia le app Java tramite firme elettroniche con GroupDocs.Signature. Firma documenti aziendali in modo rapido e semplice."

############################# Header ############################
title: "Firmare documenti via Java API"
description: "Firma documenti digitali e immagini su qualsiasi piattaforma utilizzando le nostre API flessibili e soluzioni basate su app per programmatori e utenti finali."
words:
  for: "per"

actions:
  main: "Scarica gratis Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Licenza"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Pronti per iniziare?"
  description: "Prova gratuitamente le funzionalità di GroupDocs.Signature o richiedi una licenza"

release:
  title: "Rilasciata la versione {0}"
  notes: "Scopri le novità"
  downloads: "Download"

code:
  title: "Firma file PDF in Java"
  more: "Altri esempi"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Seleziona il documento PDF
    Signature signature = new Signature("sample.pdf");
    
    // Fornire testo
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Firma il documento e salvalo su file
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Panoramica di GroupDocs.Signature"
  description: "API per eseguire la firma dei documenti e le operazioni correlate nelle applicazioni Java"
  features:
    # feature loop
    - title: "Documenti aziendali migliorati con firme digitali in Java"
      content: "Firma rapida e personalizzabile: GroupDocs.Signature per Java offre un'ampia gamma di opzioni di firma digitale per PDF, immagini e documenti Office. Puoi utilizzare testo, codici a barre, codici QR, certificati digitali, immagini o metadati nascosti. L'elaborazione dei documenti è rapida ed efficiente."

    # feature loop
    - title: "Manipolazione di documenti firmati"
      content: "L'elaborazione avanzata dei documenti prevede operazioni potenti sui documenti firmati utilizzando GroupDocs.Signature per Java. Puoi cercare e convalidare le firme aggiunte ai documenti aziendali utilizzando vari criteri utili. Inoltre, puoi accedere a informazioni dettagliate sul documento o ottenere immagini di anteprima delle sue pagine."

    # feature loop
    - title: "Varietà di scelte di output"
      content: "Le robuste opzioni di firma ti consentono di personalizzare l'output per i documenti firmati con GroupDocs.Signature per Java. Puoi posizionare con precisione qualsiasi firma su qualsiasi pagina del documento e configurarne l'aspetto in vari modi. L'API Java supporta il salvataggio di documenti aziendali firmati in numerosi formati supportati e fornisce opzioni per proteggerli con password."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Signature per Java supporta i seguenti sistemi operativi, framework e gestori di pacchetti"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formati di file supportati"
  description: |
    GroupDocs.Signature per Java supporta operazioni con i seguenti [formati di file](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formati Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Immagini e altri formati
        * **Portatile:** PDF
        * **immagini:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Altri formati di ufficio:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Altri formati
        * **ragnatela:** HTML, MHTML
        * **Archivi:** ZIP, TAR, 7Z
        * **Certificati:** PFX

############################# Features ############################
features:
  enable: true
  title: "Funzionalità di GroupDocs.Signature"
  description: "Firma di PDF, documenti Office e immagini con firme digitali"

  items:
    # feature loop
    - icon: "sign"
      title: "Aggiunta di firme"
      content: "Firma un documento utilizzando vari tipi di firma supportati inserendo una firma digitale esattamente in qualsiasi posizione su qualsiasi pagina."

    # feature loop
    - icon: "custom"
      title: "Personalizzazione dei risultati"
      content: "Personalizza l'aspetto della firma regolando colore, carattere, bordo, rotazione e altre funzionalità per ottenere il risultato desiderato."

    # feature loop
    - icon: "password"
      title: "Protezione dei documenti con password"
      content: "Per molti tipi di documenti supportati, puoi proteggere il documento firmato con una password."

    # feature loop
    - icon: "protect"
      title: "Prevenire modifiche non autorizzate"
      content: "Proteggi importanti documenti aziendali firmati con un certificato digitale da modifiche non autorizzate."

    # feature loop
    - icon: "convert"
      title: "Ottenere risultati nei formati desiderati"
      content: "Ottieni facilmente file di risultati firmati in qualsiasi formato supportato. Puoi anche convertire documenti MS Word in PDF senza sforzo."

    # feature loop
    - icon: "preview"
      title: "Anteprima del documento"
      content: "Salva qualsiasi pagina di un documento come immagine per elaborazioni future."

    # feature loop
    - icon: "search"
      title: "Alla ricerca delle firme"
      content: "È possibile ottenere informazioni sulle firme aggiunte in precedenza in documenti specifici."

    # feature loop
    - icon: "validate"
      title: "Convalida dei documenti"
      content: "Convalida la correttezza delle firme su qualsiasi documento firmato."

    # feature loop
    - icon: "update"
      title: "Gestione delle firme"
      content: "Una volta inserita una firma su una pagina del documento, è possibile eliminarla, spostarla o aggiornarla secondo necessità."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Esempi di codici"
  description: "Alcuni casi d'uso tipici di GroupDocs.Signature per operazioni Java"
  items:
    # code sample loop
    - title: "Migliora il documento PDF con il codice QR"
      content: |
        Migliorare i processi aziendali aggiungendo [codici QR](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) a pagine specifiche di documenti PDF può essere prezioso. È disponibile un esempio di come aggiungere un codice QR utilizzando GroupDocs.Signature per Java.
        {{< landing/code title="Migliora il documento PDF con il codice QR">}}
        ```java {style=abap}
        // Carica il documento da firmare
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Crea opzioni di codice QR con testo predefinito
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configura il tipo di codifica del codice QR e la posizione sulla pagina
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Firma il documento e salvalo come file dei risultati
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Utilizza la firma digitale per proteggere un DOCX"
      content: |
        Puoi [Proteggere un documento](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) utilizzando firme personali o aziendali archiviate come certificati digitali. I documenti protetti con certificato non possono essere alterati senza invalidare la firma.
        {{< landing/code title="Utilizza la firma digitale per proteggere un DOCX">}}
        ```java {style=abap}   
        // Caricare il documento da firmare digitalmente
        Signature signature = new Signature("file_to_sign.docx");
        
        // Specificare le opzioni di firma digitale e fornire il percorso del file del certificato
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Imposta la password del certificato
        options.setPassword("1234567890");

        // Firma il documento e salvalo nel percorso desiderato
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---