---
############################# Static ############################
layout: "landing"
date: 2024-02-29T14:43:07
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: it
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

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

############################# Head ############################
head_title: ".NET, Java, API cloud e app per la firma di documenti online"
head_description: "Ottieni una soluzione completa per la firma elettronica dei documenti per .NET, Java e applicazioni basate su cloud. Firma formati di documenti comuni online utilizzando la semplice funzionalità di trascinamento della selezione"

############################# Header ############################
title: "Firmare documenti<br>tramite l'API .NET"
description: "Firma documenti digitali e immagini su qualsiasi piattaforma utilizzando le nostre API flessibili e soluzioni basate su app per programmatori e utenti finali."
words:
  for: "per"

actions:
  main: "Download gratuito di NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licenza"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Pronti per iniziare?"
  description: "Prova gratuitamente le funzionalità di GroupDocs.Signature o richiedi una licenza"

release:
  title: "Rilasciata la versione {0}"
  notes: "Scopri le novità"
  downloads: "Download"

code:
  title: "Firma file PDF in C#"
  more: "Altri esempi"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Seleziona il documento PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Fornire testo
        var options = new TextSignOptions("John Smith")
        {
            // Imposta il colore
            ForeColor = Color.Red
        };
        // Firma il documento e salvalo su file
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Panoramica di GroupDocs.Signature"
  description: "API per eseguire la firma dei documenti e le operazioni correlate nelle applicazioni .NET"
  features:
    # feature loop
    - title: "Aggiunta di firme ai documenti aziendali in C#"
      content: "Firma dei documenti: con GroupDocs.Signature per .NET, puoi aggiungere vari tipi di firme, come testo, immagini, codici a barre e certificati digitali, ai documenti PDF e Office. Questa API ti consente di firmare i tuoi documenti con quasi tutti i tipi di dati, inclusi i metadati nascosti."

    # feature loop
    - title: "Elaborazione di documenti firmati"
      content: "Elaborazione aggiuntiva: puoi eseguire operazioni potenti sui documenti firmati utilizzando GroupDocs.Signature. Ciò include la ricerca di firme esistenti all'interno di documenti aziendali e la loro verifica utilizzando criteri specifici. Inoltre, puoi recuperare informazioni sui documenti e visualizzare in anteprima le pagine tramite questa API .NET."

    # feature loop
    - title: "Personalizzazione dei risultati"
      content: "GroupDocs.Signature per .NET offre ampie opzioni di personalizzazione. Puoi posizionare con precisione le firme in qualsiasi punto della pagina del documento e regolarne l'aspetto utilizzando una varietà di impostazioni. Inoltre, questa API supporta il salvataggio dei documenti elaborati in un'ampia gamma di formati supportati."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Signature per .NET supporta i seguenti sistemi operativi, framework e gestori di pacchetti"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formati di file supportati"
  description: |
    GroupDocs.Signature per .NET supporta operazioni con i seguenti [formati di file](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  description: "Firma di PDF, documenti Office e immagini in modo rapido e accurato"

  items:
    # feature loop
    - icon: "sign"
      title: "Firma del documento"
      content: "Aggiungi con precisione uno o più tipi di firme supportate in qualsiasi posizione specificata sui documenti aziendali."

    # feature loop
    - icon: "custom"
      title: "Personalizza le firme"
      content: "Utilizza funzionalità come colore, carattere, bordo, rotazione, ecc. per configurare l'aspetto delle firme."

    # feature loop
    - icon: "password"
      title: "Protezione dei documenti tramite password"
      content: "Proteggi determinati tipi di documenti impostando una password dopo la firma."

    # feature loop
    - icon: "protect"
      title: "Protezione dai cambiamenti"
      content: "Impedisci modifiche a documenti aziendali importanti dopo aver aggiunto una firma con un certificato digitale."

    # feature loop
    - icon: "convert"
      title: "Converti file firmati in altri formati"
      content: "Converti file firmati nei formati desiderati, ad esempio salvando un documento Word come PDF."

    # feature loop
    - icon: "preview"
      title: "Estrai le anteprime delle pagine"
      content: "Estrai pagine da documenti firmati come singole immagini per elaborazioni future."

    # feature loop
    - icon: "search"
      title: "Ricerca della firma nei documenti"
      content: "Recupera informazioni sulle firme aggiunte in precedenza in documenti specifici."

    # feature loop
    - icon: "validate"
      title: "Convalidare i documenti firmati"
      content: "Verifica la corretta firma dei documenti utilizzando le funzionalità di convalida."

    # feature loop
    - icon: "update"
      title: "Aggiorna o elimina le firme"
      content: "Riposiziona facilmente firme specifiche su una pagina, modificane il testo o eliminale senza problemi."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Esempi di codici"
  description: "Alcuni casi d'uso tipici di GroupDocs.Signature per operazioni .NET"
  items:
    # code sample loop
    - title: "Aggiungi il codice QR al PDF"
      content: |
        L'aggiunta di [codici QR](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) a pagine specifiche di documenti PDF può migliorare i processi aziendali. Di seguito è riportato un esempio di come aggiungere un codice QR utilizzando GroupDocs.Signature.
        {{< landing/code title="Come inserire il codice QR nel PDF.">}}
        ```csharp {style=abap}
        // Carica il documento da firmare
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Crea opzioni di codice QR con testo predefinito
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Configura il tipo di codifica del codice QR e la posizione sulla pagina
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Firma il documento e salvalo come file dei risultati
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Proteggere un documento DOCX utilizzando un certificato digitale"
      content: |
        Puoi [Proteggere un documento](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) utilizzando firme personali o aziendali archiviate come certificati digitali. Tali documenti protetti non possono essere modificati senza invalidare la firma.
        {{< landing/code title="Ecco come garantire l'integrità del documento.">}}
        ```csharp {style=abap}   
        // Caricare il documento da firmare digitalmente
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Specificare le opzioni di firma digitale e fornire il percorso del file del certificato
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Imposta la password del certificato
                Password = "1234567890"
            };
            // Firma il documento e salvalo nel percorso desiderato
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
