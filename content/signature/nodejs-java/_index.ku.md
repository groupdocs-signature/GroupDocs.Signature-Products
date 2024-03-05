---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: ku
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: ".NET, Java, API-yên Cloud & Serlêdanên Îmzekirina Belgeya Serhêl"
head_description: "Ji bo .NET, Java û serîlêdanên ewr-based çareseriya e-îmzaya belgeya tev-di-yek bistînin. Formên belgeyên hevpar ên serhêl bi karanîna taybetmendiya kaş û avêtinê ya hêsan îmze bikin"

############################# Header ############################
title: "Belgeyên îmze bikin<br>bi Node.js API"
description: "Dokument û wêneyên dîjîtal li ser her platformê bi karanîna API-yên me yên maqûl û çareseriyên bingehîn ên sepanê ji bo bernamenûs û bikarhênerên dawîn îmze bikin."
words:
  for: "bo"

actions:
  main: "Ji NPM dakêşin"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Lîsanskirin"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Amade ne ku dest pê bikin?"
  description: "Taybetmendiyên GroupDocs.Signature belaş biceribîne an destûrnameyek bixwaze"

release:
  title: "Guhertoya {0} derket"
  notes: "Binêrin ka çi nû ye"
  downloads: "Downloads"

code:
  title: "Îmzekirina PDF-ê ji hêla Node.js ve"
  more: "Nimûneyên bêtir"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Belgeya PDF-ê hilbijêrin
    let signature = new Signature("sample.pdf");
    
    // Nivîsar pêşkêş bikin
    let options = new TextSignOptions("John Smith");
    
    // Rengê danîn
    options.ForeColor = Color.Red;
    
    // Belge îmze bikin û pelê hilînin
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Overview"
  description: "Pirtûkxaneya îmzekirina belgeyan ku amade ye ku di sepanên Node.js de were bikar anîn"
  features:
    # feature loop
    - title: "Çareseriya Îmzeya Dîjîtal ji bo Belgeyên Karsaziyê bi Node.js"
      content: "GroupDocs.Signature for Node.js via Java ji bo PDF, belgeyên Office û wêneyan komek berfireh vebijarkên îmzeya dîjîtal pêşkêşî dike. Nivîs, barkod, wêne, sertîfîkayên dîjîtal û metadata hene. Pêvajoya belgeya rêkûpêk karîgeriyê misoger dike."

    # feature loop
    - title: "Manîpulasyona Pêşketî ya Belgeyên Îmzekirî"
      content: "GroupDocs.Signature hêz dide te ku hûn belgeyên îmzekirî bişopînin. Bi karanîna pîvanên cihêreng li îmzeyan bigerin û rast bikin. Wekî din, agahdariya belgeya berfireh derxînin an wêneyên pêşdîtina rûpelan biafirînin."

    # feature loop
    - title: "Formatên Derketinê yên Cihêreng"
      content: "Çareseriya me li ser formata derketinê ya belgeyên îmzekirî kontrolek berfireh peyda dike. Di her rûpelê de îmzeyan bi cih bikin û xuyangê wan xweş bikin. Belgeyên îmzekirî di gelek formên piştgirîkirî de hilînin û bi vebijarkî wan bi şîfreyan ewle bikin."

############################# Platforms ############################
platforms:
  enable: true
  title: "Serxwebûna platformê"
  description: "GroupDocs.Signature for Node.js via Java bi pergalên xebitandinê yên cihêreng pêvajokirina belgeyê pêk tîne"
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
  title: "Formatên pelê piştgirî kirin"
  description: |
    GroupDocs.Signature for Node.js via Java xebatên ji bo [formatên pelê yên populer](https://docs.groupdocs.com/signature/java/supported-document-formats/) hêsan dike.
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formatên Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Wêne & Formên Din
        * **Cîtêgûherr:** PDF
        * **Images:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Formên ofîsê yên din:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Formên din
        * **Tevn:** HTML, MHTML
        * **Kitik:** ZIP, TAR, 7Z
        * **Sertîfîkayên:** PFX

############################# Features ############################
features:
  enable: true
  title: "Taybetmendiyên GroupDocs.Signature"
  description: "PDF, belgeyên Office, û wêneyan bi îmzeyên dîjîtal îmze bikin"

  items:
    # feature loop
    - icon: "sign"
      title: "Îmzeyan Business"
      content: "Ji bo îmzekirina belgeyan cûreyên cûda yên îmzeyan bikar bînin. Îmzeyên dîjîtal tam li her cîhê rûpelê bi cîh bikin."

    # feature loop
    - icon: "custom"
      title: "Xweserîkirina Xuyabûna Îmzeyê"
      content: "Aliyên dîtbarî yên îmzeyan bi eyarkirina reng, font, sînor, zivirandin, û hêj bêtir biguhezînin da ku bigihîjin encama xweya xwestinê."

    # feature loop
    - icon: "password"
      title: "Belgeyên Parastî-Şîfre"
      content: "Ji bo gelek formatên belgeyên piştgirîkirî, ji bo ewlehiya zêde belgeyên îmzekirî bi şîfreyek biparêzin."

    # feature loop
    - icon: "protect"
      title: "Pêşîlêgirtina Guherandinên Bêdestûr"
      content: "Belgeyên karsaziya girîng ên ku bi sertîfîkayên dîjîtal ve hatine îmzekirin ji guhertinên bêdestûr biparêzin."

    # feature loop
    - icon: "convert"
      title: "Formatên derketinê yên xwestî"
      content: "Belgeyên îmzekirî di her formatek piştgirî de bêhêvî bistînin. Belgeyên MS Word-ê bi hêsanî bi formata PDF-ê veguherînin."

    # feature loop
    - icon: "preview"
      title: "Documents Previewing"
      content: "Ji bo hewcedariyên pêşerojê rûpelên belgeyên kesane wekî wêne hilînin."

    # feature loop
    - icon: "search"
      title: "Lêgerîna Îmzeyan"
      content: "Agahdariya li ser îmzeyên ku berê hatine zêdekirin di nav belgeyên xwe de bistînin."

    # feature loop
    - icon: "validate"
      title: "Validation Document"
      content: "Rastiya îmzeyên ku di her belgeyê de têne pêşkêş kirin verast bikin."

    # feature loop
    - icon: "update"
      title: "Îmze Management"
      content: "Îmzayên ku li ser her rûpelek belgeyê hatine danîn jêbirin, veguhezînin, an biguhezînin."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Nimûneyên kodê"
  description: "Nimûneyên diyarker ên ku operasyonên tîpîk ên GroupDocs.Signature for Node.js via Java nîşan didin"
  items:
    # code sample loop
    - title: "PDF-ê bi kodên QR-ê nîşan bikin"
      content: |
        Tevlihevkirina [barkod](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) di nav rûpelên belgeyên PDF-ê yên taybetî de dikare pêvajoyên karsaziyê xweş bike. Ev beş mînakek zêdekirina kodek QR bi karanîna GroupDocs.Signature for Node.js via Java peyda dike.
        {{< landing/code title="Meriv çawa koda QR-ê li PDF-ê dixe.">}}
        ```javascript {style=abap}
        // Belgeyê ji bo îmzekirinê barkirin
        let signature = new Signature("file_to_sign.pdf");
        
        // Vebijarkên koda QR-ê bi nivîsa pêşwextkirî biafirînin
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Li ser rûpelê celeb û cîhê kodkirina koda QR-ê mîheng bikin
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Belgeyê îmze bikin û wekî pelê encamê hilînin
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Parastina DOCX bi Nîşanek dîjîtal"
      content: |
        [Belgeyên xwe biparêzin](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) bi îmzeyan li ser bingeha sertîfîkayên dîjîtal. Îmzeya dîjîtal belgeyên karsaziya we li hember guhertina naverokê diparêze.
        {{< landing/code title="Li vir e ku meriv çawa yekbûna belgeyê piştrast dike.">}}
        ```javascript {style=abap}   
        // Belgeya ku bi dîjîtal were imze kirin bar bikin
        let signature = new Signature("file_to_sign.docx");
        
        // Vebijarkên îmzekirina dîjîtal diyar bikin û riya pelê sertîfîkayê peyda bikin
        let options = new DigitalSignOptions("certificate.pfx");

        // Şîfreya sertîfîkayê saz bikin
        options.Password = "1234567890";

        // Belgeyê îmze bikin û li ser riya xwestinê hilînin
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
