---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:49
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: ro
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
head_title: "Biblioteca de semnături digitale Java - GroupDocs.Signature"
head_description: "Îmbunătățiți aplicațiile Java prin semnături electronice cu GroupDocs.Signature. Semnează documente de afaceri rapid și fără efort."

############################# Header ############################
title: "Semnează documente<br>prin API-ul Java"
description: "Semnează documente și imagini digitale pe orice platformă folosind API-urile noastre flexibile și soluțiile bazate pe aplicații pentru programatori și utilizatori finali."
words:
  for: "pentru"

actions:
  main: "Descărcare gratuită Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Licențiere"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Sunteți gata să începeți?"
  description: "Încercați gratuit funcțiile GroupDocs.Signature sau solicitați o licență"

release:
  title: "Versiunea {0} a fost lansată"
  notes: "Vezi ce este nou"
  downloads: "Descărcări"

code:
  title: "Semnează fișiere PDF în Java"
  more: "Mai multe exemple"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Selectați documentul PDF
    Signature signature = new Signature("sample.pdf");
    
    // Furnizați text
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Semnează documentul și salvează în fișier
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Prezentare generală GroupDocs.Signature"
  description: "API pentru efectuarea semnării documentelor și a operațiunilor conexe în aplicațiile Java"
  features:
    # feature loop
    - title: "Documente de afaceri îmbunătățite cu semnături digitale în Java"
      content: "Semnare rapidă și personalizabilă: GroupDocs.Signature pentru Java oferă o gamă largă de opțiuni de semnătură digitală pentru PDF-uri, imagini și documente Office. Puteți utiliza text, coduri de bare, coduri QR, certificate digitale, imagini sau metadate ascunse. Procesarea documentelor este rapidă și eficientă."

    # feature loop
    - title: "Manipularea documentelor semnate"
      content: "Procesarea avansată a documentelor implică operații puternice asupra documentelor semnate folosind GroupDocs.Signature pentru Java. Puteți căuta și valida semnăturile care au fost adăugate în documentele de afaceri folosind diverse criterii utile. În plus, puteți accesa informații detaliate despre document sau puteți obține imagini de previzualizare ale paginilor acestuia."

    # feature loop
    - title: "Varietate de opțiuni de ieșire"
      content: "Opțiunile de semnare robuste vă permit să personalizați rezultatul documentelor semnate cu GroupDocs.Signature pentru Java. Puteți poziționa cu precizie orice semnătură pe orice pagină de document și puteți configura aspectul acesteia în diverse moduri. API-ul Java acceptă salvarea documentelor comerciale semnate în numeroase formate acceptate și oferă opțiuni pentru securizarea lor cu parole."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independenta platformei"
  description: "GroupDocs.Signature pentru Java acceptă următoarele sisteme de operare, cadre și manageri de pachete"
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
  title: "Formate de fișiere acceptate"
  description: |
    GroupDocs.Signature pentru Java acceptă operațiuni cu următoarele [formate de fișiere](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### formatele Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Imagini și alte formate
        * **Portabil:** PDF
        * **Imagini:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Alte formate de birou:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Alte formate
        * **Web:** HTML, MHTML
        * **Arhive:** ZIP, TAR, 7Z
        * **Certificate:** PFX

############################# Features ############################
features:
  enable: true
  title: "Funcții GroupDocs.Signature"
  description: "Semnează PDF-uri, documente Office și imagini cu semnături digitale"

  items:
    # feature loop
    - icon: "sign"
      title: "Adăugarea de semnături"
      content: "Semnați un document folosind diferite tipuri de semnături acceptate, plasând o semnătură digitală exact în orice poziție de pe orice pagină."

    # feature loop
    - icon: "custom"
      title: "Personalizarea rezultatelor"
      content: "Personalizați aspectul semnăturii ajustând culoarea, fontul, chenarul, rotația și alte caracteristici pentru a obține rezultatul dorit."

    # feature loop
    - icon: "password"
      title: "Securizarea documentelor cu parola"
      content: "Pentru multe tipuri de documente acceptate, puteți proteja documentul semnat cu o parolă."

    # feature loop
    - icon: "protect"
      title: "Prevenirea modificărilor neautorizate"
      content: "Protejați documentele importante de afaceri semnate cu un certificat digital de modificările neautorizate."

    # feature loop
    - icon: "convert"
      title: "Obținerea rezultatelor în formatele dorite"
      content: "Obțineți cu ușurință fișiere cu rezultate semnate în orice format acceptat. De asemenea, puteți converti documente MS Word în PDF fără efort."

    # feature loop
    - icon: "preview"
      title: "Previzualizarea documentului"
      content: "Salvați orice pagină a unui document ca imagine pentru procesare ulterioară."

    # feature loop
    - icon: "search"
      title: "Căutarea semnăturilor"
      content: "Este posibil să obțineți informații despre semnăturile adăugate anterior în anumite documente."

    # feature loop
    - icon: "validate"
      title: "Validarea documentelor"
      content: "Validați corectitudinea semnăturilor pe orice document semnat."

    # feature loop
    - icon: "update"
      title: "Gestionarea semnăturilor"
      content: "Odată ce o semnătură este plasată pe pagina unui document, aceasta poate fi ștearsă, mutată sau actualizată după cum este necesar."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemple de cod"
  description: "Unele cazuri de utilizare ale operațiunilor tipice GroupDocs.Signature pentru Java"
  items:
    # code sample loop
    - title: "Îmbunătățiți documentul PDF cu codul QR"
      content: |
        Îmbunătățirea proceselor de afaceri prin adăugarea [QR-codes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) în anumite pagini de documente PDF poate fi valoroasă. Există un exemplu despre cum să adăugați un cod QR utilizând GroupDocs.Signature pentru Java.
        {{< landing/code title="Îmbunătățiți documentul PDF cu codul QR">}}
        ```java {style=abap}
        // Încărcați documentul pentru semnare
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Creați opțiuni de cod QR cu text predefinit
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configurați tipul și poziția de codare a codului QR pe ​​pagină
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Semnați documentul și salvați-l ca fișier rezultat
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Utilizați semnătura digitală pentru a proteja un DOCX"
      content: |
        Puteți [Proteza un document](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) folosind semnături personale sau corporative stocate ca certificate digitale. Documentele securizate cu certificat nu pot fi modificate fără invalidarea semnăturii.
        {{< landing/code title="Utilizați semnătura digitală pentru a proteja un DOCX">}}
        ```java {style=abap}   
        // Încărcați documentul pentru a fi semnat digital
        Signature signature = new Signature("file_to_sign.docx");
        
        // Specificați opțiunile de semnare digitală și furnizați calea către fișierul de certificat
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Setați parola certificatului
        options.setPassword("1234567890");

        // Semnează documentul și salvează-l în calea dorită
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---
