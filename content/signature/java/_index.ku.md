---
############################# Static ############################
layout: "landing"
date: 2024-02-29T14:43:06
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: ku
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
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

############################# Head ############################
head_title: ".NET, Java, API-yên Cloud & Serlêdanên Îmzekirina Belgeya Serhêl"
head_description: "Ji bo .NET, Java û serîlêdanên ewr-based çareseriya e-îmzaya belgeya tev-di-yek bistînin. Formên belgeyên hevpar ên serhêl bi karanîna taybetmendiya kaş û avêtinê ya hêsan îmze bikin"

############################# Header ############################
title: "Belgeyên îmze bikin<br>bi rêya Java API"
description: "Dokument û wêneyên dîjîtal li ser her platformê bi karanîna API-yên me yên maqûl û çareseriyên bingehîn ên sepanê ji bo bernamenûs û bikarhênerên dawîn îmze bikin."
words:
  for: "bo"

actions:
  main: "belaş Maven Download"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Lîsanskirin"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Amade ne ku dest pê bikin?"
  description: "Taybetmendiyên GroupDocs.Signature belaş biceribîne an destûrnameyek bixwaze"

release:
  title: "Guhertoya {0} derket"
  notes: "Binêrin ka çi nû ye"
  downloads: "Downloads"

code:
  title: "Pelên PDF-ê di Java de îmze bikin"
  more: "Nimûneyên bêtir"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Belgeya PDF-ê hilbijêrin
    Signature signature = new Signature("sample.pdf");
    
    // Nivîsar pêşkêş bikin
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Belge îmze bikin û pelê hilînin
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Overview"
  description: "API ji bo pêkanîna îmzekirina belgeyê û karûbarên têkildar ên di sepanên Java de"
  features:
    # feature loop
    - title: "Belgeyên karsaziyê yên bi îmzeyên dîjîtal ên li Java-yê çêtir kirin"
      content: "Îmzekirina bilez û xwerû: GroupDocs.Signature ji bo Java ji bo PDF, wêne û belgeyên Office vebijarkên îmzaya dîjîtal ên berfireh pêşkêşî dike. Hûn dikarin nivîs, barkod, QR-kod, sertîfîkayên dîjîtal, wêne, an metadata veşartî bikar bînin. Pêvajoya belgeyê bilez û bikêr e."

    # feature loop
    - title: "Manîpulasyona belgeyên îmzekirî"
      content: "Pêvajoya pêşkeftî ya belgeyê bi karanîna GroupDocs.Signature ji bo Java-yê li ser belgeyên îmzekirî operasyonên bi hêz pêk tîne. Hûn dikarin îmzeyên ku li belgeyên karsaziyê hatine zêdekirin bi karanîna pîvanên cûda yên kêrhatî bigerin û rast bikin. Wekî din, hûn dikarin di derbarê belgeyê de agahdariya berfireh bigihînin an wêneyên pêşdîtinê yên rûpelên wê bistînin."

    # feature loop
    - title: "Cûrbecûr vebijarkên derketinê"
      content: "Vebijarkên îmzakirina zexm dihêlin hûn ji bo belgeyên ku bi GroupDocs.Signature ji bo Java-yê hatine îmzekirin derketinê xweş bikin. Hûn dikarin bi rastî her îmzeyê li ser her rûpelê belgeyê bicîh bikin û xuyangê wê bi awayên cihêreng mîheng bikin. Java API piştgirî dide tomarkirina belgeyên karsaziya îmzekirî di gelek formên piştgirî de û vebijarkên ji bo ewlekirina wan bi şîfreyan peyda dike."

############################# Platforms ############################
platforms:
  enable: true
  title: "Serxwebûna platformê"
  description: "GroupDocs.Signature ji bo Java pergalên xebitandinê, çarçove û rêveberên pakêtê yên jêrîn piştgirî dike"
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
  title: "Formatên pelê piştgirî kirin"
  description: |
    GroupDocs.Signature ji bo Java operasyonên bi [formên pelan](https://docs.groupdocs.com/signature/java/supported-document-formats/) yên jêrîn piştgirî dike.
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
  description: "Îmzekirina PDF, Belgeyên Ofîsê, û wêneyan bi îmzeyên dîjîtal"

  items:
    # feature loop
    - icon: "sign"
      title: "Zêdekirina Îmzeyan"
      content: "Bi danîna îmzayek dîjîtal tam li her cîhek li ser her rûpelê, belgeyek bi karanîna cûrbecûr cûrbecûr îmzeyên piştgirîkirî îmze bikin."

    # feature loop
    - icon: "custom"
      title: "Xweserkirina encamên"
      content: "Bi eyarkirina reng, font, sînor, zivirandin, û taybetmendiyên din re xuyangê îmzeyê xweş bikin da ku bigihîjin encama xwestinê."

    # feature loop
    - icon: "password"
      title: "Ewlekirina belgeyên bi şîfre"
      content: "Ji bo gelek celeb belgeyên piştgirî, hûn dikarin belgeya îmzekirî bi şîfreyek biparêzin."

    # feature loop
    - icon: "protect"
      title: "Pêşîlêgirtina guhertinên bê destûr"
      content: "Belgeyên karsaziya girîng ên ku bi sertîfîkayek dîjîtal ve hatine îmzekirin ji guhertinên bêdestûr biparêzin."

    # feature loop
    - icon: "convert"
      title: "Di formên xwestî de encam digirin"
      content: "Pelên encamên îmzekirî di her formatek piştgirî de bi hêsanî bistînin. Di heman demê de hûn dikarin belgeyên MS Word-ê jî bêyî hewldan veguherînin PDF-ê."

    # feature loop
    - icon: "preview"
      title: "Pêşdîtina belgeyê"
      content: "Her rûpelek belgeyek wekî wêneyek ji bo pêvajoyek pêşerojê hilînin."

    # feature loop
    - icon: "search"
      title: "Li îmzeyan digere"
      content: "Mimkun e ku meriv di belgeyên taybetî de li ser îmzeyên ku berê hatine zêdekirin agahdarî bistînin."

    # feature loop
    - icon: "validate"
      title: "Belgeyên erêkirin"
      content: "Rastiya îmzeyan li ser her belgeyek îmzekirî rast bikin."

    # feature loop
    - icon: "update"
      title: "Îmzeyan îdare dikin"
      content: "Dema ku îmzeyek li ser rûpelek belgeyê were danîn, li gorî hewcedariyê dikare were jêbirin, barkirin an nûvekirin."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Nimûneyên kodê"
  description: "Hin rewşên tîpîk GroupDocs.Signature ji bo operasyonên Java bikar tînin"
  items:
    # code sample loop
    - title: "Belgeya PDF-ê bi QR-kodê xweş bikin"
      content: |
        Zêdekirina pêvajoyên karsaziyê bi zêdekirina [QR-kod](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) li ser rûpelên taybetî yên belgeyên PDF-ê dikare hêja be. Mînakek heye ku meriv çawa kodek QR bi karanîna GroupDocs.Signature ji bo Java-yê zêde dike.
        {{< landing/code title="Belgeya PDF-ê bi QR-kodê xweş bikin">}}
        ```java {style=abap}
        // Belgeyê ji bo îmzekirinê barkirin
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Vebijarkên koda QR-ê bi nivîsa pêşwextkirî biafirînin
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Li ser rûpelê celeb û cîhê kodkirina koda QR-ê mîheng bikin
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Belgeyê îmze bikin û wekî pelê encamê hilînin
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Ji bo parastina DOCX-ê îmzeya dîjîtal bikar bînin"
      content: |
        Hûn dikarin [Belgeyekê biparêzin](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) îmzeyên kesane an pargîdanî yên ku wekî sertîfîkayên dîjîtal hatine hilanîn bikar bînin. Belgeyên ku bi sertîfîkayê hatine ewlekirin bêyî betalkirina îmzeyê nayên guhertin.
        {{< landing/code title="Ji bo parastina DOCX-ê îmzeya dîjîtal bikar bînin">}}
        ```java {style=abap}   
        // Belgeya ku bi dîjîtal were imze kirin bar bikin
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Vebijarkên îmzekirina dîjîtal diyar bikin û riya pelê sertîfîkayê peyda bikin
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Şîfreya sertîfîkayê saz bikin
        options.setPassword("1234567890");

        // Belgeyê îmze bikin û li ser riya xwestinê hilînin
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
