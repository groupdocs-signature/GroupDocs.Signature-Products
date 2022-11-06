---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Code39 Extended
fileformat: Tiff
productName: Java
lang: it
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Tiff for Java

############################# Head ############################
head_title: "eSign Tiff documento con codice a barre Code39 Extended in Java"
head_description: "Crea Code39 Extended Firma codice a barre e inseriscilo nel documento Tiff con Java utilizzando un paio di righe di codice. Utilizza l'API per la firma dei documenti di GroupDocs per firmare vari formati di file."

############################# Header ############################
title: "Genera Code39 Extended firma del codice a barre per il documento Tiff in Java"
description: "Firma elettronicamente i tuoi documenti aziendali Tiff con il codice a barre Code39 Extended. Genera la firma del codice a barre in modo rapido e semplice con poche righe di codice per impostare le opzioni di firma."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Informazioni su GroupDocs.Signature for Java API delle firme di codici a barre."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) è un'API semplice e veloce per gestire la firma elettronica dei documenti digitali utilizzando tipi di codici a barre come UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 e molti altri. I clienti possono creare facilmente codici a barre fornendo il testo richiesto e inserirli in PDF, documenti Microsoft Office Words, cartelle di lavoro Microsoft Office Excel, presentazioni MS PowerPoint, file Adobe Photoshop e vari formati di immagine. I codici a barre inseriti nei documenti possono essere aggiornati, ricercati, verificati, eliminati o visualizzati in anteprima. Inoltre, è supportata la personalizzazione dei codici a barre.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Passaggi per firmare Tiff con Barcode in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) offre la possibilità di firmare documenti Tiff con firme Barcode in modo rapido e semplice.
        
        * Crea un'istanza della classe Signature che fornisce il file Tiff che dovrebbe firmare come percorso o flusso di memoria
        * Crea un'istanza della classe SignOptions e imposta tutti i dati richiesti.
        * Richiama il metodo Signature.Sign() passando il file di output Tiff o il flusso di memoria

    title_right: " Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for Java sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Ricevi l'ultimo GroupDocs.Signature for Java da [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Tiff file
        String filePath = "input.tiff";
        // Set up output file
        String outputFilePath = "output.tiff";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Code39 Extended);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Tiff document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma di documenti Tiff con Barcode Demo live"
    content: |
       Firma subito il file Tiff con varie firme visitando il sito web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuita ti aspetta.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Code39 Extended Barcode"
          content: |
            Il codice 39 (noto anche come Alpha39, codice 3 di 9, codice 3/9, tipo 39, codice USS 39 o USD-3) è una simbologia di codici a barre discreti di lunghezza variabile.
          characterset: |
             Set di caratteri: tutti i 128 caratteri ASCII.
          textcapacity: |
             Nessuna restrizione specifica.
          image: |
             iVBORw0KGgoAAAANSUhEUgAABw0AAABGCAYAAAA+TwtQAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAEnVSURBVHhe7dlRiug60zTrd/6T/g4+kCAelC31KtwX/3ZAXARZ8gT8v//7+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4T/P9NPz4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+I/z/TT8+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+PiP8/00/Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4j/P9NPz4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+I/z/TT8+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+PiP8/00/Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4j/PjT8P//e9//78N97SG3fYYWmtorQ33U8v0XtxvW4Mt65vVYMv0XtxvW8Nue2y4v30v7mkNrbXhfmqZ3ot7WsNta8P99l5Daw2nlum9uN+2NtzXN6vBlum9uKc1nFravQZbpvfiftsadttjw/3te3FPazi1tHsNtqxvVkNrDaeW6b2437aG3fbYcH/7XtzTGlprsOVf7zW01nBqmd6L+29bsmvYbY/Blum9uKc1tNaG+6llei/ut63BlvXNarBlei/uaQ2tteF+apnei3taw21rw/3te3FPazi1tHsNtkzvxf22Ney2x4b72/fintbQWhvup5bsGlpruG0NtrR7DbZM78U9reHU0u412DK9F/e0htvWhvvb9+Ke1rDbHoMtp3tbpvfintbQWoMtf30v7retDff1zWqwZXov7mkNrbXhfmpp9xp222OwGz9enD7intaw2x5Daw2tteF+apnei/tta7BlfbMabJnei/tta9htjw33t+/FPa2htTbcTy3Te3FPa7htbbjf3mtoreHUMr0X99vWhvv6ZjXYMr0X97SGU0u712DL9F7cb1vDbntsuL99L+5pDaeWdq/BlvXNamit4dQyvRf329aw2x4b7m/fi3taQ2sNtvzrvYbWGk4t03tx/21Ldg277THYMr0X97SG1tpwP7VM78X9tjXYsr5ZDbZM78U9raG1NtxPLdN7cU9ruG1tuL99L+5pDaeWdq/Blum9uN+2ht322HB/+17c0xpaa8P91JJdQ2sNt63BlnavwZbpvbinNZxa2r0GW6b34p7WcNvacH/7XtzTGnbbY7DldG/L9F7c0xpaa7Dlr+/F/ba14b6+WQ22TO/FPa2htTbcTy3tXsNuewx248eL00fc0xp222NoraG1NtxPLdN7cb9tDbasb1aDLdN7cb9tDbvtseH+9r24pzW01ob7qWV6L+5pDbetDffbew2tNZxapvfiftvacF/frAZbpvfintZwamn3GmyZ3ov7bWvYbY8N97fvxT2t4dTS7jXYsr5ZDa01nFqm9+J+2xp222PD/e17cU9raK3Bln+919Baw6llei/uv23JrmG3PQZbpvfintbQWhvup5bpvbjftgZb1jerwZbpvbinNbTWhvupZXov7mkNt60N97fvxT2t4dTS7jXYMr0X99vWsNseG+5v34t7WkNrbbifWrJraK3htjXY0u412DK9F/e0hlNLu9dgy/Re3NMablsb7m/fi3taw257DLac7m2Z3ot7WkNrDbb89b2437Y23Nc3q8GW6b24pzW01ob7qaXda9htj8Fu/Hhx+oh7WsNuewytNbTWhvupZXov7retwZb1zWqwZXov7retYbc9Ntzfvhf3tIbW2nA/tUzvxT2t4ba14X57r6G1hlPL9F7cb1sb7uub1WDL9F7c0xpOLe1egy3Te3G/bQ277bHh/va9uKc1nFravQZb1jerobWGU8v0XtxvW8Nue2y4v30v7mkNrTXY8q/3GlprOLVM78X9ty3ZNey2x2DL9F7c0xpaa8P91DK9F/fb1mDL+mY12DK9F/e0htbacD+1TO/FPa3htrXh/va9uKc1nFravQZbpvfiftsadttjw/3te3FPa2itDfdTS3YNrTXctgZb2r0GW6b34p7WcGpp9xpsmd6Le1rDbWvD/e17cU9r2G2PwZbTvS3Te3FPa2itwZa/vhf329aG+/pmNdgyvRf3tIbW2nA/tbR7DbvtMdiNHy9OH3FPa9htj6G1htbacD+1TO/F/bY12LK+WQ22TO/F/bY17LbHhvvb9+Ke1tBaG+6nlum9uKc13LY23G/vNbTWcGqZ3ov7bWvDfX2zGmyZ3ot7WsOppd1rsGV6L+63rWG3PTbc374X97SGU0u712DL+mY1tNZwapnei/tta9htjw33t+/FPa2htQZb/vVeQ2sNp5bpvbj/tiW7ht32GGyZ3ot7WkNrbbifWqb34n7bGmxZ36wGW6b34p7W0Fob7qeW6b24pzXctjbc374X97SGU0u712DL9F7cb1vDbntsuL99L+5pDa214X5qya6htYbb1mBLu9dgy/Re3NMaTi3tXoMt03txT2u4bW24v30v7mkNu+0x2HK6t2V6L+5pDa012PLX9+J+29pwX9+sBlum9+Ke1tBaG+6nlnavYbc9Brvx48XpI+5pDbvtMbTW0Fob7qeW6b2437YGW9Y3q8GW6b2437aG3fbYcH/7XtzTGlprw/3UMr0X97SG29aG++29htYaTi3Te3G/bW24r29Wgy3Te3FPazi1tHsNtkzvxf22Ney2x4b72/fintZwamn3GmxZ36yG1hpOLdN7cb9tDbvtseH+9r24pzW01mDLv95raK3h1DK9F/fftmTXsNsegy3Te3FPa2itDfdTy/Re3G9bgy3rm9Vgy/Re3NMaWmvD/dQyvRf3tIbb1ob72/fintZwamn3GmyZ3ov7bWvYbY8N97fvxT2tobU23E8t2TW01nDbGmxp9xpsmd6Le1rDqaXda7Blei/uaQ23rQ33t+/FPa1htz0GW073tkzvxT2tobUGW/76XtxvWxvu65vVYMv0XtzTGlprw/3U0u417LbHYDd+vDh9xD2tYbc9htYaWmvD/dQyvRf329Zgy/pmNdgyvRf329aw2x4b7m/fi3taQ2ttuJ9apvfintZw29pwv73X0FrDqWV6L+63rQ339c1qsGV6L+5pDaeWdq/Blum9uN+2ht322HB/+17c0xpOLe1egy3rm9XQWsOpZXov7retYbc9Ntzfvhf3tIbWGmz513sNrTWcWqb34v7bluwadttjsGV6L+5pDa214X5qmd6L+21rsGV9sxpsmd6Le1pDa224n1qm9+Ke1nDb2nB/+17c0xpOLe1egy3Te3G/bQ277bHh/va9uKc1tNaG+6klu4bWGm5bgy3tXoMt03txT2s4tbR7DbZM78U9reG2teH+9r24pzXstsdgy+nelum9uKc1tNZgy1/fi/tta8N9fbMabJnei3taQ2ttuJ9a2r2G3fYY7MaPF6ePuKc17LbH0FpDa224n1qm9+J+2xpsWd+sBlum9+J+2xp222PD/e17cU9raK0N91PL9F7c0xpuWxvut/caWms4tUzvxf22teG+vlkNtkzvxT2t4dTS7jXYMr0X99vWsNseG+5v34t7WsOppd1rsGV9sxpaazi1TO/F/bY17LbHhvvb9+Ke1tBagy3/eq+htYZTy/Re3H/bkl3DbnsMtkzvxT2tobU23E8t03txv20NtqxvVoMt03txT2torQ33U8v0XtzTGm5bG+5v34t7WsOppd1rsGV6L+63rWG3PTbc374X97SG1tpwP7Vk19Baw21rsKXda7Blei/uaQ2nlnavwZbpvbinNdy2Ntzfvhf3tIbd9hhsOd3bMr0X97SG1hps+et7cb9tbbivb1aDLdN7cU9raK0N91NLu9ew2x6D3fjx4vQR97SG3fYYWmtorQ33U8v0XtxvW4Mt65vVYMv0XtxvW8Nue2y4v30v7mkNrbXhfmqZ3ot7WsNta8P99l5Daw2nlum9uN+2NtzXN6vBlum9uKc1nFravQZbpvfiftsadttjw/3te3FPazi1tHsNtqxvVkNrDaeW6b2437aG3fbYcH/7XtzTGlprsOVf7zW01nBqmd6L+29bsmvYbY/Blum9uKc1tNaG+6llei/ut63BlvXNarBlei/uaQ2tteF+apnei3taw21rw/3te3FPazi1tHsNtkzvxf22Ney2x4b72/fintbQWhvup5bsGlpruG0NtrR7DbZM78U9reHU0u412DK9F/e0htvWhvvb9+Ke1rDbHoMtp3tbpvfintbQWoMtf30v7retDff1zWqwZXov7mkNrbXhfmpp9xp222OwGz9enD7intaw2x5Daw2tteF+apnei/tta7BlfbMabJnei/tta9htjw33t+/FPa2htTbcTy3Te3FPa7htbbjf3mtoreHUMr0X99vWhvv6ZjXYMr0X97SGU0u712DL9F7cb1vDbntsuL99L+5pDaeWdq/BlvXNamit4dQyvRf329aw2x4b7m/fi3taQ2sNtvzrvYbWGk4t03tx/21Ldg277THYMr0X97SG1tpwP7VM78X9tjXYsr5ZDbZM78U9raG1NtxPLdN7cU9ruG1tuL99L+5pDaeWdq/Blum9uN+2ht322HB/+17c0xpaa8P91JJdQ2sNt63BlnavwZbpvbinNZxa2r0GW6b34p7WcNvacH/7XtzTGnbbY7DldG/L9F7c0xpaa7Dlr+/F/ba14b6+WQ22TO/FPa2htTbcTy3tXsNuewx248eL00fc0xp222NoraG1NtxPLdN7cb9tDbasb1aDLdN7cb9tDbvtseH+9r24pzW01ob7qWV6L+5pDbetDffbew2tNZxapvfiftvacF/frAZbpvfintZwamn3GmyZ3ov7bWvYbY8N97fvxT2t4dTS7jXYsr5ZDa01nFqm9+J+2xp222PD/e17cU9raK3Bln+919Baw6llei/uv23JrmG3PQZbpvfintbQWhvup5bpvbjftgZb1jerwZbpvbinNbTWhvupZXov7mkNt60N97fvxT2t4dTS7jXYMr0X99vWsNseG+5v34t7WkNrbbifWrJraK3htjXY0u412DK9F/e0hlNLu9dgy/Re3NMablsb7m/fi3taw257DLac7m2Z3ot7WkNrDbb89b2437Y23Nc3q8GW6b24pzW01ob7qaXda9htj8Fu/Hhx+oh7WsNuewytNbTWhvupZXov7retwZb1zWqwZXov7retYbc9Ntzfvhf3tIbW2nA/tUzvxT2t4ba14X57r6G1hlPL9F7cb1sb7uub1WDL9F7c0xpOLe1egy3Te3G/bQ277bHh/va9uKc1nFravQZb1jerobWGU8v0XtxvW8Nue2y4v30v7mkNrTXY8q/3GlprOLVM78X9ty3ZNey2x2DL9F7c0xpaa8P91DK9F/fb1mDL+mY12DK9F/e0htbacD+1TO/FPa3htrXh/va9uKc1nFravQZbpvfiftsadttjw/3te3FPa2itDfdTS3YNrTXctgZb2r0GW6b34p7WcGpp9xpsmd6Le1rDbWvD/e17cU9r2G2PwZbTvS3Te3FPa2itwZa/vhf329aG+/pmNdgyvRf3tIbW2nA/tbR7DbvtMdiNHy9OH3FPa9htj6G1htbacD+1TO/F/bY12LK+WQ22TO/F/bY17LbHhvvb9+Ke1tBaG+6nlum9uKc13LY23G/vNbTWcGqZ3ov7bWvDfX2zGmyZ3ot7WsOppd1rsGV6L+63rWG3PTbc374X97SGU0u712DL+mY1tNZwapnei/tta9htjw33t+/FPa2htQZb/vVeQ2sNp5bpvbj/tiW7ht32GGyZ3ot7WkNrbbifWqb34n7bGmxZ36wGW6b34p7W0Fob7qeW6b24pzXctjbc374X97SGU0u712DL9F7cb1vDbntsuL99L+5pDa214X5qya6htYbb1mBLu9dgy/Re3NMaTi3tXoMt03txT2u4bW24v30v7mkNu+0x2HK6t2V6L+5pDa012PLX9+J+29pwX9+sBlum9+Ke1tBaG+6nlnavYbc9Brvx48XpI+5pDbvtMbTW0Fob7qeW6b2437YGW9Y3q8GW6b2437aG3fbYcH/7XtzTGlprw/3UMr0X97SG29aG++29htYaTi3Te3G/bW24r29Wgy3Te3FPazi1tHsNtkzvxf22Ney2x4b72/fintZwamn3GmxZ36yG1hpOLdN7cb9tDbvtseH+9r24pzW01mDLv95raK3h1DK9F/fftmTXsNsegy3Te3FPa2itDfdTy/Re3G9bgy3rm9Vgy/Re3NMaWmvD/dQyvRf3tIbb1ob72/fintZwamn3GmyZ3ov7bWvYbY8N97fvxT2tobU23E8t2TW01nDbGmxp9xpsmd6Le1rDqaXda7Blei/uaQ23rQ33t+/FPa1htz0GW073tkzvxT2tobUGW/76XtxvWxvu65vVYMv0XtzTGlprw/3U0u417LbHYDd+vDh9xD2tYbc9htYaWmvD/dQyvRf329Zgy/pmNdgyvRf329aw2x4b7m/fi3taQ2ttuJ9apvfintZw29pwv73X0FrDqWV6L+63rQ339c1qsGV6L+5pDaeWdq/Blum9uN+2ht322HB/+17c0xpOLe1egy3rm9XQWsOpZXov7retYbc9Ntzfvhf3tIbWGmz513sNrTWcWqb34v7bluwadttjsGV6L+5pDa214X5qmd6L+21rsGV9sxpsmd6Le1pDa224n1qm9+Ke1nDb2nB/+17c0xpOLe1egy3Te3G/bQ277bHh/va9uKc1tNaG+6klu4bWGm5bgy3tXoMt03txT2s4tbR7DbZM78U9reG2teH+9r24pzXstsdgy+nelum9uKc1tNZgy1/fi/tta8N9fbMabJnei3taQ2ttuJ9a2r2G3fYY7MaPF6ePuKc17LbH0FpDa224n1qm9+J+2xpsWd+sBlum9+J+2xp222PD/e17cU9raK0N91PL9F7c0xpuWxvut/caWms4tUzvxf22teG+vlkNtkzvxT2t4dTS7jXYMr0X99vWsNseG+5v34t7WsOppd1rsGV9sxpaazi1TO/F/bY17LbHhvvb9+Ke1tBagy3/eq+htYZTy/Re3H/bkl3DbnsMtkzvxT2tobU23E8t03txv20NtqxvVoMt03txT2torQ33U8v0XtzTGm5bG+5v34t7WsOppd1rsGV6L+63rWG3PTbc374X97SG1tpwP7Vk19Baw21rsKXda7Blei/uaQ2nlnavwZbpvbinNdy2Ntzfvhf3tIbd9hhsOd3bMr0X97SG1hps+et7cb9tbbivb1aDLdN7cU9raK0N91NLu9ew2x6D3fjx4vQR97SG3fYYWmtorQ33U8v0XtxvW4Mt65vVYMv0XtxvW8Nue2y4v30v7mkNrbXhfmqZ3ot7WsNta8P99l5Daw2nlum9uN+2NtzXN6vBlum9uKc1nFravQZbpvfiftsadttjw/3te3FPazi1tHsNtqxvVkNrDaeW6b2437aG3fbYcH/7XtzTGlprsOVf7zW01nBqmd6L+29bsmvYbY/Blum9uKc1tNaG+6llei/ut63BlvXNarBlei/uaQ2tteF+apnei3taw21rw/3te3FPazi1tHsNtkzvxf22Ney2x4b72/fintbQWhvup5bsGlpruG0NtrR7DbZM78U9reHU0u412DK9F/e0htvWhvvb9+Ke1rDbHoMtp3tbpvfintbQWoMtf30v7retDff1zWqwZXov7mkNrbXhfmpp9xp222OwGz9enD7intaw2x5Daw2tteF+apnei/tta7BlfbMabJnei/tta9htjw33t+/FPa2htTbcTy3Te3FPa7htbbjf3mtoreHUMr0X99vWhvv6ZjXYMr0X97SGU0u712DL9F7cb1vDbntsuL99L+5pDaeWdq/BlvXNamit4dQyvRf329aw2x4b7m/fi3taQ2sNtvzrvYbWGk4t03tx/21Ldg277THYMr0X97SG1tpwP7VM78X9tjXYsr5ZDbZM78U9raG1NtxPLdN7cU9ruG1tuL99L+5pDaeWdq/Blum9uN+2ht322HB/+17c0xpaa8P91JJdQ2sNt63BlnavwZbpvbinNZxa2r0GW6b34p7WcNvacH/7XtzTGnbbY7DldG/L9F7c0xpaa7Dlr+/F/ba14b6+WQ22TO/FPa2htTbcTy3tXsNuewx248eL00fc0xp222NoraG1NtxPLdN7cb9tDbasb1aDLdN7cb9tDbvtseH+9r24pzW01ob7qWV6L+5pDbetDffbew2tNZxapvfiftvacF/frAZbpvfintZwamn3GmyZ3ov7bWvYbY8N97fvxT2t4dTS7jXYsr5ZDa01nFqm9+J+2xp222PD/e17cU9raK3Bln+919Baw6llei/uv23JrmG3PQZbpvfintbQWhvup5bpvbjftgZb1jerwZbpvbinNbTWhvupZXov7mkNt60N97fvxT2t4dTS7jXYMr0X99vWsNseG+5v34t7WkNrbbifWrJraK3htjXY0u412DK9F/e0hlNLu9dgy/Re3NMablsb7m/fi3taw257DLac7m2Z3ot7WkNrDbb89b2437Y23Nc3q8GW6b24pzW01ob7qaXda9htj8Fu/Hhx+oh7WsNuewytNbTWhvupZXov7retwZb1zWqwZXov7retYbc9Ntzfvhf3tIbW2nA/tUzvxT2t4ba14X57r6G1hlPL9F7cb1sb7uub1WDL9F7c0xpOLe1egy3Te3G/bQ277bHh/va9uKc1nFravQZb1jerobWGU8v0XtxvW8Nue2y4v30v7mkNrTXY8q/3GlprOLVM78X9ty3ZNey2x2DL9F7c0xpaa8P91DK9F/fb1mDL+mY12DK9F/e0htbacD+1TO/FPa3htrXh/va9uKc1nFravQZbpvfiftsadttjw/3te3FPa2itDfdTS3YNrTXctgZb2r0GW6b34p7WcGpp9xpsmd6Le1rDbWvD/e17cU9r2G2PwZbTvS3Te3FPa2itwZa/vhf329aG+/pmNdgyvRf3tIbW2nA/tbR7DbvtMdiNHy9OH3FPa9htj6G1htbacD+1TO/F/bY12LK+WQ22TO/F/bY17LbHhvvb9+Ke1tBaG+6nlum9uKc13LY23G/vNbTWcGqZ3ov7bWvDfX2zGmyZ3ot7WsOppd1rsGV6L+63rWG3PTbc374X97SGU0u712DL+mY1tNZwapnei/tta9htjw33t+/FPa2htQZb/vVeQ2sNp5bpvbj/tiW7ht32GGyZ3ot7WkNrbbifWqb34n7bGmxZ36wGW6b34p7W0Fob7qeW6b24pzXctjbc374X97SGU0u712DL9F7cb1vDbntsuL99L+5pDa214X5qya6htYbb1mBLu9dgy/Re3NMaTi3tXoMt03txT2u4bW24v30v7mkNu+0x2HK6t2V6L+5pDa012PLX9+J+29pwX9+sBlum9+Ke1tBaG+6nlnavYbc9Brvx48XpI+5pDbvtMbTW0Fob7qeW6b2437YGW9Y3q8GW6b2437aG3fbYcH/7XtzTGlprw/3UMr0X97SG29aG++29htYaTi3Te3G/bW24r29Wgy3Te3FPazi1tHsNtkzvxf22Ney2x4b72/fintZwamn3GmxZ36yG1hpOLdN7cb9tDbvtseH+9r24pzW01mDLv95raK3h1DK9F/fftmTXsNsegy3Te3FPa2itDfdTy/Re3G9bgy3rm9Vgy/Re3NMaWmvD/dQyvRf3tIbb1ob72/fintZwamn3GmyZ3ov7bWvYbY8N97fvxT2tobU23E8t2TW01nDbGmxp9xpsmd6Le1rDqaXda7Blei/uaQ23rQ33t+/FPa1htz0GW073tkzvxT2tobUGW/76XtxvWxvu65vVYMv0XtzTGlprw/3U0u417LbHYDd+vDh9xD2tYbc9htYaWmvD/dQyvRf329Zgy/pmNdgyvRf329aw2x4b7m/fi3taQ2ttuJ9apvfintZw29pwv73X0FrDqWV6L+63rQ339c1qsGV6L+5pDaeWdq/Blum9uN+2ht322HB/+17c0xpOLe1egy3rm9XQWsOpZXov7retYbc9Ntzfvhf3tIbWGmz513sNrTWcWqb34v7bluwadttjsGV6L+5pDa214X5qmd6L+21rsGV9sxpsmd6Le1pDa224n1qm9+Ke1nDb2nB/+17c0xpOLe1egy3Te3G/bQ277bHh/va9uKc1tNaG+6klu4bWGm5bgy3tXoMt03txT2s4tbR7DbZM78U9reG2teH+9r24pzXstsdgy+nelum9uKc1tNZgy1/fi/tta8N9fbMabJnei3taQ2ttuJ9a2r2G3fYY7MaPF6ePuKc17LbH0FpDa224n1qm9+J+2xpsWd+sBlum9+J+2xp222PD/e17cU9raK0N91PL9F7c0xpuWxvut/caWms4tUzvxf22teG+vlkNtkzvxT2t4dTS7jXYMr0X99vWsNseG+5v34t7WsOppd1rsGV9sxpaazi1TO/F/bY17LbHhvvb9+Ke1tBagy3/eq+htYZTy/Re3H/bkl3DbnsMtkzvxT2tobU23E8t03txv20NtqxvVoMt03txT2torQ33U8v0XtzTGm5bG+5v34t7WsOppd1rsGV6L+63rWG3PTbc374X97SG1tpwP7Vk19Baw21rsKXda7Blei/uaQ2nlnavwZbpvbinNdy2Ntzfvhf3tIbd9hhsOd3bMr0X97SG1hps+et7cb9tbbivb1aDLdN7cU9raK0N91NLu9ew2x6D3fjx4vQR97SG3fYYWmtorQ33U8v0XtxvW4Mt65vVYMv0XtxvW8Nue2y4v30v7mkNrbXhfmqZ3ot7WsNta8P99l5Daw2nlum9uN+2NtzXN6vBlum9uKc1nFravQZbpvfiftsadttjw/3te3FPazi1tHsNtqxvVkNrDaeW6b2437aG3fbYcH/7XtzTGlprsOVf7zW01nBqmd6L+29bsmvYbY/Blum9uKc1tNaG+6llei/ut63BlvXNarBlei/uaQ2tteF+apnei3taw21rw/3te3FPazi1tHsNtkzvxf22Ney2x4b72/fintbQWhvup5bsGlpruG0NtrR7DbZM78U9reHU0u412DK9F/e0htvWhvvb9+Ke1rDbHoMtp3tbpvfintbQWoMtf30v7retDff1zWqwZXov7mkNrbXhfmpp9xp222OwGz9enD7intaw2x5Daw2tteF+apnei/tta7BlfbMabJnei/tta9htjw33t+/FPa2htTbcTy3Te3FPa7htbbjf3mtoreHUMr0X99vWhvv6ZjXYMr0X97SGU0u712DL9F7cb1vDbntsuL99L+5pDaeWdq/BlvXNamit4dQyvRf329aw2x4b7m/fi3taQ2sNtvzrvYbWGk4t03tx/21Ldg277THYMr0X97SG1tpwP7VM78X9tjXYsr5ZDbZM78U9raG1NtxPLdN7cU9ruG1tuL99L+5pDaeWdq/Blum9uN+2ht322HB/+17c0xpaa8P91JJdQ2sNt63BlnavwZbpvbinNZxa2r0GW6b34p7WcNvacH/7XtzTGnbbY7DldG/L9F7c0xpaa7Dlr+/F/ba14b6+WQ22TO/FPa2htTbcTy3tXsNuewx248eL00fc0xp222NoraG1NtxPLdN7cb9tDbasb1aDLdN7cb9tDbvtseH+9r24pzW01ob7qWV6L+5pDbetDffbew2tNZxapvfiftvacF/frAZbpvfintZwamn3GmyZ3ov7bWvYbY8N97fvxT2t4dTS7jXYsr5ZDa01nFqm9+J+2xp222PD/e17cU9raK3Bln+919Baw6llei/uv23JrmG3PQZbpvfintbQWhvup5bpvbjftgZb1jerwZbpvbinNbTWhvupZXov7mkNt60N97fvxT2t4dTS7jXYMr0X99vWsNseG+5v34t7WkNrbbifWrJraK3htjXY0u412DK9F/e0hlNLu9dgy/Re3NMablsb7m/fi3taw257DLac7m2Z3ot7WkNrDbb89b2437Y23Nc3q8GW6b24pzW01ob7qaXda9htj8Fu/Hhx+oh7WsNuewytNbTWhvupZXov7retwZb1zWqwZXov7retYbc9Ntzfvhf3tIbW2nA/tUzvxT2t4ba14X57r6G1hlPL9F7cb1sb7uub1WDL9F7c0xpOLe1egy3Te3G/bQ277bHh/va9uKc1nFravQZb1jerobWGU8v0XtxvW8Nue2y4v30v7mkNrTXY8q/3GlprOLVM78X9ty3ZNey2x2DL9F7c0xpaa8P91DK9F/fb1mDL+mY12DK9F/e0htbacD+1TO/FPa3htrXh/va9uKc1nFravQZbpvfiftsadttjw/3te3FPa2itDfdTS3YNrTXctgZb2r0GW6b34p7WcGpp9xpsmd6Le1rDbWvD/e17cU9r2G2PwZbTvS3Te3FPa2itwZa/vhf329aG+/pmNdgyvRf3tIbW2nA/tbR7DbvtMdiNHy9OH3FPa9htj6G1htbacD+1TO/F/bY12LK+WQ22TO/F/bY17LbHhvvb9+Ke1tBaG+6nlum9uKc13LY23G/vNbTWcGqZ3ov7bWvDfX2zGmyZ3ot7WsOppd1rsGV6L+63rWG3PTbc374X97SGU0u712DL+mY1tNZwapnei/tta9htjw33t+/FPa2htQZb/vVeQ2sNp5bpvbj/tiW7ht32GGyZ3ot7WkNrbbifWqb34n7bGmxZ36wGW6b34p7W0Fob7qeW6b24pzXctjbc374X97SGU0u712DL9F7cb1vDbntsuL99L+5pDa214X5qya6htYbb1mBLu9dgy/Re3NMaTi3tXoMt03txT2u4bW24v30v7mkNu+0x2HK6t2V6L+5pDa012PLX9+J+29pwX9+sBlum9+Ke1tBaG+6nlnavYbc9Brvx48XpI+5pDbvtMbTW0Fob7qeW6b2437YGW9Y3q8GW6b2437aG3fbYcH/7XtzTGlprw/3UMr0X97SG29aG++29htYaTi3Te3G/bW24r29Wgy3Te3FPazi1tHsNtkzvxf22Ney2x4b72/fintZwamn3GmxZ36yG1hpOLdN7cb9tDbvtseH+9r24pzW01mDLv95raK3h1DK9F/fftmTXsNsegy3Te3FPa2itDfdTy/Re3G9bgy3rm9Vgy/Re3NMaWmvD/dQyvRf3tIbb1ob72/fintZwamn3GmyZ3ov7bWvYbY8N97fvxT2tobU23E8t2TW01nDbGmxp9xpsmd6Le1rDqaXda7Blei/uaQ23rQ33t+/FPa1htz0GW073tkzvxT2tobUGW/76XtxvWxvu65vVYMv0XtzTGlprw/3U0u417LbHYDd+vDh9xD2tYbc9htYaWmvD/dQyvRf329Zgy/pmNdgyvRf329aw2x4b7m/fi3taQ2ttuJ9apvfintZw29pwv73X0FrDqWV6L+63rQ339c1qsGV6L+5pDaeWdq/Blum9uN+2ht322HB/+17c0xpOLe1egy3rm9XQWsOpZXov7retYbc9Ntzfvhf3tIbWGmz513sNrTWcWqb34v7bluwadttjsGV6L+5pDa214X5qmd6L+21rsGV9sxpsmd6Le1pDa224n1qm9+Ke1nDb2nB/+17c0xpOLe1egy3Te3G/bQ277bHh/va9uKc1tNaG+6klu4bWGm5bgy3tXoMt03txT2s4tbR7DbZM78U9reG2teH+9r24pzXstsdgy+nelum9uKc1tNZgy1/fi/tta8N9fbMabJnei3taQ2ttuJ9a2r2G3fYY7MaPF6ePuKc17LbH0FpDa224n1qm9+J+2xpsWd+sBlum9+J+2xp222PD/e17cU9raK0N91PL9F7c0xpuWxvut/caWms4tUzvxf22teG+vlkNtkzvxT2t4dTS7jXYMr0X99vWsNseG+5v34t7WsOppd1rsGV9sxpaazi1TO/F/bY17LbHhvvb9+Ke1tBagy3/eq+htYZTy/Re3H/bkl3DbnsMtkzvxT2tobU23E8t03txv20NtqxvVoMt03txT2torQ33U8v0XtzTGm5bG+5v34t7WsOppd1rsGV6L+63rWG3PTbc374X97SG1tpwP7Vk19Baw21rsKXda7Blei/uaQ2nlnavwZbpvbinNdy2Ntzfvhf3tIbd9hhsOd3bMr0X97SG1hps+et7cb9tbbivb1aDLdN7cU9raK0N91NLu9ew2x6D3fjx4vQR97SG3fYYWmtorQ33U8v0XtxvW4Mt65vVYMv0XtxvW8Nue2y4v30v7mkNrbXhfmqZ3ot7WsNta8P99l5Daw2nlum9uN+2NtzXN6vBlum9uKc1nFravQZbpvfiftsadttjw/3te3FPazi1tHsNtqxvVkNrDaeW6b2437aG3fbYcH/7XtzTGlprsOVf7zW01nBqmd6L+29bsmvYbY/Blum9uKc1tNaG+6llei/ut63BlvXNarBlei/uaQ2tteF+apnei3taw21rw/3te3FPazi1tHsNtkzvxf22Ney2x4b72/fintbQWhvup5bsGlpruG0NtrR7DbZM78U9reHU0u412DK9F/e0htvWhvvb9+Ke1rDbHoMtp3tbpvfintbQWoMtf30v7retDff1zWqwZXov7mkNrbXhfmpp9xp222OwGz9enD7intaw2x5Daw2tteF+apnei/tta7BlfbMabJnei/tta9htjw33t+/FPa2htTbcTy3Te3FPa7htbbjf3mtoreHUMr0X99vWhvv6ZjXYMr0X97SGU0u712DL9F7cb1vDbntsuL99L+5pDaeWdq/BlvXNamit4dQyvRf329aw2x4b7m/fi3taQ2sNtvzrvYbWGk4t03tx/21Ldg277THYMr0X97SG1tpwP7VM78X9tjXYsr5ZDbZM78U9raG1NtxPLdN7cU9ruG1tuL99L+5pDaeWdq/Blum9uN+2ht322HB/+17c0xpaa8P91JJdQ2sNt63BlnavwZbpvbinNZxa2r0GW6b34p7WcNvacH/7XtzTGnbbY7DldG/L9F7c0xpaa7Dlr+/F/ba14b6+WQ22TO/FPa2htTbcTy3tXsNuewx248eL00fc0xp222NoraG1NtxPLdN7cb9tDbasb1aDLdN7cb9tDbvtseH+9r24pzW01ob7qWV6L+5pDbetDffbew2tNZxapvfiftvacF/frAZbpvfintZwamn3GmyZ3ov7bWvYbY8N97fvxT2t4dTS7jXYsr5ZDa01nFqm9+J+2xp222PD/e17cU9raK3Bln+919Baw6llei/uv23JrmG3PQZbpvfintbQWhvup5bpvbjftgZb1jerwZbpvbinNbTWhvupZXov7mkNt60N97fvxT2t4dTS7jXYMr0X99vWsNseG+5v34t7WkNrbbifWrJraK3htjXY0u412DK9F/e0hlNLu9dgy/Re3NMablsb7m/fi3taw257DLac7m2Z3ot7WkNrDbb89b2437Y23Nc3q8GW6b24pzW01ob7qaXda9htj8Fu/Hhx+oh7WsNuewytNbTWhvupZXov7retwZb1zWqwZXov7retYbc9Ntzfvhf3tIbW2nA/tUzvxT2t4ba14X57r6G1hlPL9F7cb1sb7uub1WDL9F7c0xpOLe1egy3Te3G/bQ277bHh/va9uKc1nFravQZb1jerobWGU8v0XtxvW8Nue2y4v30v7mkNrTXY8q/3GlprOLVM78X9ty3ZNey2x2DL9F7c0xpaa8P91DK9F/fb1mDL+mY12DK9F/e0htbacD+1TO/FPa3htrXh/va9uKc1nFravQZbpvfiftsadttjw/3te3FPa2itDfdTS3YNrTXctgZb2r0GW6b34p7WcGpp9xpsmd6Le1rDbWvD/e17cU9r2G2PwZbTvS3Te3FPa2itwZa/vhf329aG+/pmNdgyvRf3tIbW2nA/tbR7DbvtMdiNHy9OH3FPa9htj6G1htbacD+1TO/F/bY12LK+WQ22TO/F/bY17LbHhvvb9+Ke1tBaG+6nlum9uKc13LY23G/vNbTWcGqZ3ov7bWvDfX2zGmyZ3ot7WsOppd1rsGV6L+63rWG3PTbc374X97SGU0u712DL+mY1tNZwapnei/tta9htjw33t+/FPa2htQZb/vVeQ2sNp5bpvbj/tiW7ht32GGyZ3ot7WkNrbbifWqb34n7bGmxZ36wGW6b34p7W0Fob7qeW6b24pzXctjbc374X97SGU0u712DL9F7cb1vDbntsuL99L+5pDa214X5qya6htYbb1mBLu9dgy/Re3NMaTi3tXoMt03txT2u4bW24v30v7mkNu+0x2HK6t2V6L+5pDa012PLX9+J+29pwX9+sBlum9+Ke1tBaG+6nlnavYbc9Brvx48XpI+5pDbvtMbTW0Fob7qeW6b2437YGW9Y3q8GW6b2437aG3fbYcH/7XtzTGlprw/3UMr0X97SG29aG++29htYaTi3Te3G/bW24r29Wgy3Te3FPazi1tHsNtkzvxf22Ney2x4b72/fintZwamn3GmxZ36yG1hpOLdN7cb9tDbvtseH+9r24pzW01mDLv95raK3h1DK9F/fftmTXsNsegy3Te3FPa2itDfdTy/Re3G9bgy3rm9Vgy/Re3NMaWmvD/dQyvRf3tIbb1ob72/fintZwamn3GmyZ3ov7bWvYbY8N97fvxT2tobU23E8t2TW01nDbGmxp9xpsmd6Le1rDqaXda7Blei/uaQ23rQ33t+/FPa1htz0GW073tkzvxT2tobUGW/76XtxvWxvu65vVYMv0XtzTGlprw/3U0u417LbHYDd+vDh9xD2tYbc9htYaWmvD/dQyvRf329Zgy/pmNdgyvRf329aw2x4b7m/fi3taQ2ttuJ9apvfintZw29pwv73X0FrDqWV6L+63rQ339c1qsGV6L+5pDaeWdq/Blum9uN+2ht322HB/+17c0xpOLe1egy3rm9XQWsOpZXov7retYbc9Ntzfvhf3tIbWGmz513sNrTWcWqb34v7bluwadttjsGV6L+5pDa214X5qmd6L+21rsGV9sxpsmd6Le1pDa224n1qm9+Ke1nDb2nB/+17c0xpOLe1egy3Te3G/bQ277bHh/va9uKc1tNaG+6klu4bWGm5bgy3tXoMt03txT2s4tbR7DbZM78U9reG2teH+9r24pzXstsdgy+nelum9uKc1tNZgy1/fi/tta8N9fbMabJnei3taQ2ttuJ9a2r2G3fYY7MaPF6ePuKc17LbH0FpDa224n1qm9+J+2xpsWd+sBlum9+J+2xp222PD/e17cU9raK0N91PL9F7c0xpuWxvut/caWms4tUzvxf22teG+vlkNtkzvxT2t4dTS7jXYMr0X99vWsNseG+5v34t7WsOppd1rsGV9sxpaazi1TO/F/bY17LbHhvvb9+Ke1tBagy3/eq+htYZTy/Re3H/bkl3DbnsMtkzvxT2tobU23E8t03txv20NtqxvVoMt03txT2torQ33U8v0XtzTGm5bG+5v34t7WsOppd1rsGV6L+63rWG3PTbc374X97SG1tpwP7Vk19Baw21rsKXda7Blei/uaQ2nlnavwZbpvbinNdy2Ntzfvhf3tIbd9hhsOd3bMr0X97SG1hps+et7cb9tbbivb1aDLdN7cU9raK0N91NLu9ew2x6D3fjx4vQR97SG3fYYWmtorQ33U8v0XtxvW4Mt65vVYMv0XtxvW8Nue2y4v30v7mkNrbXhfmqZ3ot7WsNta8P99l5Daw2nlum9uN+2NtzXN6vBlum9uKc1nFravQZbpvfiftsadttjw/3te3FPazi1tHsNtqxvVkNrDaeW6b2437aG3fbYcH/7XtzTGlprsOVf7zW01nBqmd6L+29bsmvYbY/Blum9uKc1tNaG+6llei/ut63BlvXNarBlei/uaQ2tteF+apnei3taw21rw/3te3FPazi1tHsNtkzvxf22Ney2x4b72/fintbQWhvup5bsGlpruG0NtrR7DbZM78U9reHU0u412DK9F/e0htvWhvvb9+Ke1rDbHoMtp3tbpvfintbQWoMtf30v7retDff1zWqwZXov7mkNrbXhfmpp9xp222OwGz9enD7intaw2x5Daw2tteF+apnei/tta7BlfbMabJnei/tta9htjw33t+/FPa2htTbcTy3Te3FPa7htbbjf3mtoreHUMr0X99vWhvv6ZjXYMr0X97SGU0u712DL9F7cb1vDbntsuL99L+5pDaeWdq/BlvXNamit4dQyvRf329aw2x4b7m/fi3taQ2sNtvzrvYbWGk4t03tx/21Ldg277THYMr0X97SG1tpwP7VM78X9tjXYsr5ZDbZM78U9raG1NtxPLdN7cU9ruG1tuL99L+5pDaeWdq/Blum9uN+2ht322HB/+17c0xpaa8P91JJdQ2sNt63BlnavwZbpvbinNZxa2r0GW6b34p7WcNvacH/7XtzTGnbbY7DldG/L9F7c0xpaa7Dlr+/F/ba14b6+WQ22TO/FPa2htTbcTy3tXsNuewx248eL00fc0xp222NoraG1NtxPLdN7cb9tDbasb1aDLdN7cb9tDbvtseH+9r24pzW01ob7qWV6L+5pDbetDffbew2tNZxapvfiftvacF/frAZbpvfintZwamn3GmyZ3ov7bWvYbY8N97fvxT2t4dTS7jXYsr5ZDa01nFqm9+J+2xp222PD/e17cU9raK3Bln+919Baw6llei/uv23JrmG3PQZbpvfintbQWhvup5bpvbjftgZb1jerwZbpvbinNbTWhvupZXov7mkNt60N97fvxT2t4dTS7jXYMr0X99vWsNseG+5v34t7WkNrbbifWrJraK3htjXY0u412DK9F/e0hlNLu9dgy/Re3NMablsb7m/fi3taw257DLac7m2Z3ot7WkNrDbb89b2437Y23Nc3q8GW6b24pzW01ob7qaXda9htj8Fu/Hhx+oh7WsNuewytNbTWhvupZXov7retwZb1zWqwZXov7retYbc9Ntzfvhf3tIbW2nA/tUzvxT2t4ba14X57r6G1hlPL9F7cb1sb7uub1WDL9F7c0xpOLe1egy3Te3G/bQ277bHh/va9uKc1nFravQZb1jerobWGU8v0XtxvW8Nue2y4v30v7mkNrTXY8q/3GlprOLVM78X9ty3ZNey2x2DL9F7c0xpaa8P91DK9F/fb1mDL+mY12DK9F/e0htbacD+1TO/FPa3htrXh/va9uKc1nFravQZbpvfiftsadttjw/3te3FPa2itDfdTS3YNrTXctgZb2r0GW6b34p7WcGpp9xpsmd6Le1rDbWvD/e17cU9r2G2PwZbTvS3Te3FPa2itwZa/vhf329aG+/pmNdgyvRf3tIbW2nA/tbR7DbvtMdiNHy9OH3FPa9htj6G1htbacD+1TO/F/bY12LK+WQ22TO/F/bY17LbHhvvb9+Ke1tBaG+6nlum9uKc13LY23G/vNbTWcGqZ3ov7bWvDfX2zGmyZ3ot7WsOppd1rsGV6L+63rWG3PTbc374X97SGU0u712DL+mY1tNZwapnei/tta9htjw33t+/FPa2htQZb/vVeQ2sNp5bpvbj/tiW7ht32GGyZ3ot7WkNrbbifWqb34n7bGmxZ36wGW6b34p7W0Fob7qeW6b24pzXctjbc374X97SGU0u712DL9F7cb1vDbntsuL99L+5pDa214X5qya6htYbb1mBLu9dgy/Re3NMaTi3tXoMt03txT2u4bW24v30v7mkNu+0x2HK6t2V6L+5pDa012PLX9+J+29pwX9+sBlum9+Ke1tBaG+6nlnavYbc9Brvx48XpI+5pDbvtMbTW0Fob7qeW6b2437YGW9Y3q8GW6b2437aG3fbYcH/7XtzTGlprw/3UMr0X97SG29aG++29htYaTi3Te3G/bW24r29Wgy3Te3FPazi1tHsNtkzvxf22Ney2x4b72/fintZwamn3GmxZ36yG1hpOLdN7cb9tDbvtseH+9r24pzW01mDLv95raK3h1DK9F/fftmTXsNsegy3Te3FPa2itDfdTy/Re3G9bgy3rm9Vgy/Re3NMaWmvD/dQyvRf3tIbb1ob72/fintZwamn3GmyZ3ov7bWvYbY8N97fvxT2tobU23E8t2TW01nDbGmxp9xpsmd6Le1rDqaXda7Blei/uaQ23rQ33t+/FPa1htz0GW073tkzvxT2tobUGW/76XtxvWxvu65vVYMv0XtzTGlprw/3U0u417LbHYDd+vDh9xD2tYbc9htYaWmvD/dQyvRf329Zgy/pmNdgyvRf329aw2x4b7m/fi3taQ2ttuJ9apvfintZw29pwv73X0FrDqWV6L+63rQ339c1qsGV6L+5pDaeWdq/Blum9uN+2ht322HB/+17c0xpOLe1egy3rm9XQWsOpZXov7retYbc9Ntzfvhf3tIbWGmz513sNrTWcWqb34v7bluwadttjsGV6L+5pDa214X5qmd6L+21rsGV9sxpsmd6Le1pDa224n1qm9+Ke1nDb2nB/+17c0xpOLe1egy3Te3G/bQ277bHh/va9uKc1tNaG+6klu4bWGm5bgy3tXoMt03txT2s4tbR7DbZM78U9reG2teH+9r24pzXstsdgy+nelum9uKc1tNZgy1/fi/tta8N9fbMabJnei3taQ2ttuJ9a2r2G3fYY7MaPF6ePuKc17LbH0FpDa224n1qm9+J+2xpsWd+sBlum9+J+2xp222PD/e17cU9raK0N91PL9F7c0xpuWxvut/caWms4tUzvxf22teG+vlkNtkzvxT2t4dTS7jXYMr0X99vWsNseG+5v34t7WsOppd1rsGV9sxpaazi1TO/F/bY17LbHhvvb9+Ke1tBagy3/eq+htYZTy/Re3H/bkl3DbnsMtkzvxT2tobU23E8t03txv20NtqxvVoMt03txT2torQ33U8v0XtzTGm5bG+5v34t7WsOppd1rsGV6L+63rWG3PTbc374X97SG1tpwP7Vk19Baw21rsKXda7Blei/uaQ2nlnavwZbpvbinNdy2Ntzfvhf3tIbd9hhsOd3bMr0X97SG1hps+et7cb9tbbivb1aDLdN7cU9raK0N91NLu9ew2x6D3fjx4vQR97SG3fYYWmtorQ33U8v0XtxvW4Mt65vVYMv0XtxvW8Nue2y4v30v7mkNrbXhfmqZ3ot7WsNta8P99l5Daw2nlum9uN+2NtzXN6vBlum9uKc1nFravQZbpvfiftsadttjw/3te3FPazi1tHsNtqxvVkNrDaeW6b2437aG3fbYcH/7XtzTGlprsOVf7zW01nBqmd6L+29bsmvYbY/Blum9uKc1tNaG+6llei/ut63BlvXNarBlei/uaQ2tteF+apnei3taw21rw/3te3FPazi1tHsNtkzvxf22Ney2x4b72/fintbQWhvup5bsGlpruG0NtrR7DbZM78U9reHU0u412DK9F/e0htvWhvvb9+Ke1rDbHoMtp3tbpvfintbQWoMtf30v7retDff1zWqwZXov7mkNrbXhfmpp9xp222OwGz9enD7intaw2x5Daw2tteF+apnei/tta7BlfbMabJnei/tta9htjw33t+/FPa2htTbcTy3Te3FPa7htbbjf3mtoreHUMr0X99vWhvv6ZjXYMr0X97SGU0u712DL9F7cb1vDbntsuL99L+5pDaeWdq/BlvXNamit4dQyvRf329aw2x4b7m/fi3taQ2sNtvzrvYbWGk4t03tx/21Ldg277THYMr0X97SG1tpwP7VM78X9tjXYsr5ZDbZM78U9raG1NtxPLdN7cU9ruG1tuL99L+5pDaeWdq/Blum9uN+2ht322HB/+17c0xpaa8P91JJdQ2sNt63BlnavwZbpvbinNZxa2r0GW6b34p7WcNvacH/7XtzTGnbbY7DldG/L9F7c0xpaa7Dlr+/F/ba14b6+WQ22TO/FPa2htTbcTy3tXsNuewx248eL00fc0xp222NoraG1NtxPLdN7cb9tDbasb1aDLdN7cb9tDbvtseH+9r24pzW01ob7qWV6L+5pDbetDffbew2tNZxapvfiftvacF/frAZbpvfintZwamn3GmyZ3ov7bWvYbY8N97fvxT2t4dTS7jXYsr5ZDa01nFqm9+J+2xp222PD/e17cU9raK3Bln+919Baw6llei/uv23JrmG3PQZbpvfintbQWhvup5bpvbjftgZb1jerwZbpvbinNbTWhvupZXov7mkNt60N97fvxT2t4dTS7jXYMr0X99vWsNseG+5v34t7WkNrbbifWrJraK3htjXY0u412DK9F/e0hlNLu9dgy/Re3NMablsb7m/fi3taw257DLac7m2Z3ot7WkNrDbb89b2437Y23Nc3q8GW6b24pzW01ob7qaXda9htj8Fu/Hhx+oh7WsNuewytNbTWhvupZXov7retwZb1zWqwZXov7retYbc9Ntzfvhf3tIbW2nA/tUzvxT2t4ba14X57r6G1hlPL9F7cb1sb7uub1WDL9F7c0xpOLe1egy3Te3G/bQ277bHh/va9uKc1nFravQZb1jerobWGU8v0XtxvW8Nue2y4v30v7mkNrTXY8q/3GlprOLVM78X9ty3ZNey2x2DL9F7c0xpaa8P91DK9F/fb1mDL+mY12DK9F/e0htbacD+1TO/FPa3htrXh/va9uKc1nFravQZbpvfiftsadttjw/3te3FPa2itDfdTS3YNrTXctgZb2r0GW6b34p7WcGpp9xpsmd6Le1rDbWvD/e17cU9r2G2PwZbTvS3Te3FPa2itwZa/vhf329aG+/pmNdgyvRf3tIbW2nA/tbR7DbvtMdiNHy9OH3FPa9htj6G1htbacD+1TO/F/bY12LK+WQ22TO/F/bY17LbHhvvb9+Ke1tBaG+6nlum9uKc13LY23G/vNbTWcGqZ3ov7bWvDfX2zGmyZ3ot7WsOppd1rsGV6L+63rWG3PTbc374X97SGU0u712DL+mY1tNZwapnei/tta9htjw33t+/FPa2htQZb/vVeQ2sNp5bpvbj/tiW7ht32GGyZ3ot7WkNrbbifWqb34n7bGmxZ36wGW6b34p7W0Fob7qeW6b24pzXctjbc374X97SGU0u712DL9F7cb1vDbntsuL99L+5pDa214X5qya6htYbb1mBLu9dgy/Re3NMaTi3tXoMt03txT2u4bW24v30v7mkNu+0x2HK6t2V6L+5pDa012PLX9+J+29pwX9+sBlum9+Ke1tBaG+6nlnavYbc9Brvx48XpI+5pDbvtMbTW0Fob7qeW6b2437YGW9Y3q8GW6b2437aG3fbYcH/7XtzTGlprw/3UMr0X97SG29aG++29htYaTi3Te3G/bW24r29Wgy3Te3FPazi1tHsNtkzvxf22Ney2x4b72/fintZwamn3GmxZ36yG1hpOLdN7cb9tDbvtseH+9r24pzW01mDLv95raK3h1DK9F/fftmTXsNsegy3Te3FPa2itDfdTy/Re3G9bgy3rm9Vgy/Re3NMaWmvD/dQyvRf3tIbb1ob72/fintZwamn3GmyZ3ov7bWvYbY8N97fvxT2tobU23E8t2TW01nDbGmxp9xpsmd6Le1rDqaXda7Blei/uaQ23rQ33t+/FPa1htz0GW073tkzvxT2tobUGW/76XtxvWxvu65vVYMv0XtzTGlprw/3U0u417LbHYDd+vDh9xD2tYbc9htYaWmvD/dQyvRf329Zgy/pmNdgyvRf329aw2x4b7m/fi3taQ2ttuJ9apvfintZw29pwv73X0FrDqWV6L+63rQ339c1qsGV6L+5pDaeWdq/Blum9uN+2ht322HB/+17c0xpOLe1egy3rm9XQWsOpZXov7retYbc9Ntzfvhf3tIbWGmz513sNrTWcWqb34v7bluwadttjsGV6L+5pDa214X5qmd6L+21rsGV9sxpsmd6Le1pDa224n1qm9+Ke1nDb2nB/+17c0xpOLe1egy3Te3G/bQ277bHh/va9uKc1tNaG+6klu4bWGm5bgy3tXoMt03txT2s4tbR7DbZM78U9reG2teH+9r24pzXstsdgy+nelum9uKc1tNZgy1/fi/tta8N9fbMabJnei3taQ2ttuJ9a2r2G3fYY7MaPF6ePuKc17LbH0FpDa224n1qm9+J+2xpsWd+sBlum9+J+2xp222PD/e17cU9raK0N91PL9F7c0xpuWxvut/caWms4tUzvxf22teG+vlkNtkzvxT2t4dTS7jXYMr0X99vWsNseG+5v34t7WsOppd1rsGV9sxpaazi1TO/F/bY17LbHhvvb9+Ke1tBagy3/eq+htYZTy/Re3H/bkl3DbnsMtkzvxT2tobU23E8t03txv20NtqxvVoMt03txT2torQ33U8v0XtzTGm5bG+5v34t7WsOppd1rsGV6L+63rWG3PTbc374X97SG1tpwP7Vk19Baw21rsKXda7Blei/uaQ2nlnavwZbpvbinNdy2Ntzfvhf3tIbd9hhsOd3bMr0X97SG1hps+et7cb9tbbivb1aDLdN7cU9raK0N91NLu9ew2x6D3fjx4vQR97SG3fYYWmtorQ33U8v0XtxvW4Mt65vVYMv0XtxvW8Nue2y4v30v7mkNrbXhfmqZ3ot7WsNta8P99l5Daw2nlum9uN+2NtzXN6vBlum9uKc1nFravQZbpvfiftsadttjw/3te3FPazi1tHsNtqxvVkNrDaeW6b2437aG3fbYcH/7XtzTGlprsOVf7zW01nBqmd6L+29bsmvYbY/Blum9uKc1tNaG+6llei/ut63BlvXNarBlei/uaQ2tteF+apnei3taw21rw/3te3FPazi1tHsNtkzvxf22Ney2x4b72/fintbQWhvup5bsGlpruG0NtrR7DbZM78U9reHU0u412DK9F/e0htvWhvvb9+Ke1rDbHoMtp3tbpvfintbQWoMtf30v7retDff1zWqwZXov7mkNrbXhfmpp9xp222OwG+eLj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+Pj4+P/6f5fhp+fHx8fHx8fHx8fHx8fHx8fHx8fHx8fHx8fPzH+X4afnx8fHx8fHx8fHx8fHx8fHx8fHx8fHx8fHz8x/l+Gn58fHx8fHx8fHx8fHx8fHx8fHx8fHx8fHx8/Mf5fhp+fHx8fHx8fHx8fHx8fHx8fHx8fHx8fHx8fPzH+X4afnx8fHx8fHx8fHx8fHx8fHx8fHx8fHx8fHz8p/m///v/AKky5jo8b16bAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altre firme Barcode supportate per Java"
    content: |
        "Puoi anche firmare Tiff con altri tipi di firma. Si prega di consultare l'elenco di seguito."
    format: 
        
       
back_to_top:
    enable: true
---