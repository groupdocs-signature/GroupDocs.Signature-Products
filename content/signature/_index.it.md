---
############################# Static ############################
layout: "family"
date:  2024-07-16T12:27:51
draft: false

product: "Signature"
product_tag: "signature"

lang: it

############################# Head ############################
head_title: "App di firma digitale C# .NET, Java, Node.js"
head_description: "Integra le firme elettroniche nelle applicazioni .NET, Java o Node.js con GroupDocs.Signature. Firma i formati di documenti aziendali più diffusi."

############################# Header ############################
title: "Soluzione per la firma elettronica dei documenti"
description:  |
  Firma documenti e immagini digitali su qualsiasi piattaforma utilizzando le nostre API flessibili e soluzioni basate su app per programmatori e utenti finali.

  Cerca e modifica le firme aggiunte in precedenza utilizzando metodi avanzati.

  Proteggi i documenti dalle modifiche con certificati digitali e controlla i metadati nascosti.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Scegli la tua piattaforma"
  title: "Indipendenza dalla piattaforma"
  description: "La libreria GroupDocs.Signature supporta i seguenti sistemi operativi e framework:"
  details_link_title: "Saperne di più"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Signature .NET 
      color: "blue"
      tag: "net"
      link: "/signature/net/"
      features_link: "https://docs.groupdocs.com/signature/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.6.2 or higher <br> .NET Core 3.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS <br> Microsoft Azure
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Signature Java
      color: "red"
      tag: "java"
      link: "/signature/java/"
      features_link: "https://docs.groupdocs.com/signature/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 8 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Signature Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/signature/nodejs-java/"
      features_link: "https://docs.groupdocs.com/signature/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Qualsiasi altro editor di testo
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

############################# Features ###############################
features:
  enable: true
  title: "Funzionalità principali di GroupDocs.Signature"
  description: "La nostra soluzione è progettata per aggiungere vari tipi di firme ai formati di file e documenti più diffusi. Arricchisci facilmente i tuoi processi aziendali."

  items:
    # items loop
    - icon: "additional"
      title: "Arricchisci i tuoi dati con le firme"
      content: "Aggiungi testo, immagini, filigrane, ecc. ai tuoi documenti aziendali."

    # items loop
    - icon: "protect"
      title: "Proteggi il contenuto dei documenti"
      content: "Vieta modifiche al documento sigillandolo con un certificato digitale."

    # items loop
    - icon: "search"
      title: "Aggiungi dati nascosti e codici a barre"
      content: "Utilizza i metadati per archiviare informazioni invisibili o inserire codici a barre personalizzati nelle pagine."

    # items loop
    - icon: "manipulate"
      title: "Manipolare le firme"
      content: "Cerca, aggiorna o elimina tutte le firme aggiunte in precedenza."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Proteggi i tuoi file utilizzando le firme"
  description: "Esempi di codice GroupDocs.Signature"
  items:
    # code sample loop
    - title: "Genera e aggiungi il codice QR"
      content: |
       GroupDocs.Signature ci consente di generare e aggiungere codici QR a documenti con formati supportati. Fornire il percorso di un documento che deve essere firmato e impostare il testo desiderato e le opzioni visive del codice QR. Puoi inserire l'immagine del codice QR generata in qualsiasi area di qualsiasi pagina del documento.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Specificare il documento da firmare
            using (Signature signature = new Signature("source.docx"))
            {
                // Crea opzioni di segnaletica con codice QR
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // Imposta le opzioni del codice QR
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150,
                };

                // Firma e salva il file elaborato
                SignResult result = signature.Sign("result.docx", options);
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Specificare il documento da firmare
            Signature signature = new Signature("source.docx");

            // Crea opzioni di segnaletica con codice QR
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith");

            // Imposta le opzioni del codice QR
            options.setEncodeType(QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Firma e salva il file elaborato
            signature.sign("result.docx", options);
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            const signatureLib = require('@groupdocs/groupdocs.signature')

            // Specificare il documento da firmare
            const signature = new signatureLib.Signature('source.docx');

            // Crea opzioni di segnaletica con codice QR
            const options = new signatureLib.QrCodeSignOptions('JohnSmith');

            // Imposta le opzioni del codice QR
            options.setEncodeType(signatureLib.QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Firma e salva il file elaborato
            signature.sign('result.docx', options);
            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "Sono supportati oltre 60 formati di file"
  description: "GroupDocs.Signature supporta quasi tutti i formati di file più diffusi"

############################# Metrics ###############################
metrics:
  enable: true
  title: "I dati statistici della nostra biblioteca"
  description: "Ispeziona le metriche chiave del prodotto, rivelando approfondimenti sui nostri risultati, impatto e crescita"

  items:
    # items loop
    - number: "50+"
      title: "Formati supportati"
      content: "Firma di oltre 60 dei formati di file aziendali più diffusi."

    # items loop
    - number: "500k"
      title: "Download di NuGet"
      content: "GroupDocs.Signature per .NET è una libreria popolare con oltre 550.000 download su NuGet."

    # items loop
    - number: "15k"
      title: "Download di Maven"
      content: "Gli sviluppatori Java hanno scaricato GroupDocs.Signature su Maven più di 15.000 volte."

    # items loop
    - number: "140+"
      title: "Clienti felici"
      content: "Singoli sviluppatori e aziende leader in tutto il mondo utilizzano i nostri prodotti per creare soluzioni innovative."


############################# Customers ###############################
customers:
  enable: true
  title: "I nostri clienti felici"
  description: "Le librerie GroupDocs sono utilizzate da marchi distinti e rinomati a livello globale in tutto il mondo"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Pronti per iniziare?"
  description: "Prova gratuitamente le funzionalità di GroupDocs.Signature sulla tua piattaforma"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/signature/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/signature/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/signature/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "Domande frequenti"
  description: "Esplora le nostre domande frequenti"

  items:
    # items loop
    - question: "GroupDocs.Signature necessita di una libreria esterna per la firma dei documenti?"
      answer: "No, GroupDocs.Signature funziona in modo indipendente. Non ci sono dipendenze di terze parti come Adobe Acrobat, Microsoft Office, ecc."

    # items loop
    - question: "È possibile testare le funzionalità di GroupDocs.Signature prima dell'acquisto?"
      answer: "Assolutamente! GroupDocs.Signature offre una prova gratuita. Installalo ed esplora le sue funzionalità. Tieni presente che le versioni di prova aggiungono badge di prova ai tuoi documenti ed elaborano solo le prime 3 pagine. Per un'esperienza completa, ottieni una licenza temporanea gratuita di 30 giorni per accedere a tutte le funzionalità. Vedi i dettagli in [licenza temporanea](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Quali tipi di licenza sono forniti?"
      answer: "Cerchi una licenza GroupDocs.Signature? Offriamo varie opzioni su misura per le vostre esigenze. Scegli in base alle dimensioni del team, alle posizioni di distribuzione (singolo ufficio o luoghi di lavoro remoti) e se la distribuzione al cliente finale richiede la condivisione dell'SDK/API con i clienti. In alternativa, opta per una licenza d'uso mensile con piani a consumo: paga solo per ciò che utilizzi. Scopri la soluzione più adatta a te alla pagina [prezzi](https://purchase.groupdocs.com/pricing/signature/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "API a basso codice GroupDocs.Signature"
  description: "Firma i file utilizzando la tua applicazione tramite la nostra API REST basata su cloud."
  
  items:
    # items loop
    - title: "GroupDocs.Signature Cloud for cURL"
      content: "Utilizza l'API RESTful cURL per inserire firme su PDF, Word, Excel, PowerPoint, JPEG e molti altri formati di file."
      icon: "groupdocs_signature-for-curl"
      link: "https://products.groupdocs.cloud/signature/curl"

    # items loop
    - title: "GroupDocs.Signature Cloud for .NET"
      content: "Arricchisci le tue applicazioni .NET firmando documenti tramite Cloud SDK. Proteggi i documenti aziendali a modo tuo."
      icon: "groupdocs_signature-for-net"
      link: "https://products.groupdocs.cloud/signature/net"

    # items loop
    - title: "GroupDocs.Signature Cloud for Java"
      content: "L'SDK GroupDocs.Signature garantisce l'accesso a varie possibilità per le tue applicazioni Java di firmare qualsiasi file."
      icon: "groupdocs_signature-for-java"
      link: "https://products.groupdocs.cloud/signature/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Signature App web"
  description: "GroupDocs.Signature presenta un'applicazione web gratuita in cui puoi firmare documenti. È possibile firmare GRATUITAMENTE più di 60 formati di file popolari tramite il tuo browser preferito."

  items:
    # items loop
    - title: "GroupDocs.Signature Total"
      content: "Strumento online per apporre firme sui documenti da qualsiasi dispositivo."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/signature/total"

    # items loop
    - title: "GroupDocs.Signature DOCX"
      content: "Firma MS Word DOCX online."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/signature/docx"

    # items loop
    - title: "GroupDocs.Signature PDF"
      content: "Proteggi i documenti PDF online."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/signature/pdf"


      


---