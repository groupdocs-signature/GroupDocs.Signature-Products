---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: ro
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
head_title: ".NET, Java, API-uri cloud și aplicații online pentru semnătura documentelor"
head_description: "Obțineți o soluție de semnătură electronică pentru documente all-in-one pentru .NET, Java și aplicații bazate pe cloud. Semnează online formate comune de documente folosind funcția simplă de glisare și plasare"

############################# Header ############################
title: "Semnează documente<br>cu API-ul Node.js"
description: "Semnează documente și imagini digitale pe orice platformă folosind API-urile noastre flexibile și soluțiile bazate pe aplicații pentru programatori și utilizatori finali."
words:
  for: "pentru"

actions:
  main: "Descărcați de pe NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licențiere"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Sunteți gata să începeți?"
  description: "Încercați gratuit funcțiile GroupDocs.Signature sau solicitați o licență"

release:
  title: "Versiunea {0} a fost lansată"
  notes: "Vezi ce este nou"
  downloads: "Descărcări"

code:
  title: "Semnarea PDF-urilor de către Node.js"
  more: "Mai multe exemple"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Selectați documentul PDF
    let signature = new Signature("sample.pdf");
    
    // Furnizați text
    let options = new TextSignOptions("John Smith");
    
    // Setați culoarea
    options.ForeColor = Color.Red;
    
    // Semnează documentul și salvează în fișier
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Prezentare generală GroupDocs.Signature"
  description: "Bibliotecă de semnare a documentelor care este gata pentru a fi utilizată în aplicațiile Node.js"
  features:
    # feature loop
    - title: "Soluție de semnătură digitală pentru documente de afaceri cu Node.js"
      content: "GroupDocs.Signature for Node.js via Java oferă un set cuprinzător de opțiuni de semnătură digitală pentru PDF, documente Office și imagini. Sunt disponibile text, coduri de bare, imagini, certificate digitale și metadate. Procesarea eficientă a documentelor asigură eficiență."

    # feature loop
    - title: "Manipularea avansată a documentelor semnate"
      content: "GroupDocs.Signature vă împuternicește să procesați documente semnate. Căutați și validați semnăturile folosind diverse criterii. În plus, extrageți informații detaliate despre document sau generați imagini de previzualizare ale paginilor."

    # feature loop
    - title: "Diverse formate de ieșire"
      content: "Soluția noastră oferă un control extins asupra formatului de ieșire al documentelor semnate. Poziționați cu precizie semnăturile pe orice pagină și personalizați-le aspectul. Salvați documentele semnate în numeroase formate acceptate și, opțional, asigurați-le cu parole."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independenta platformei"
  description: "GroupDocs.Signature for Node.js via Java realizează procesarea documentelor cu diferite sisteme de operare"
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
  title: "Formate de fișiere acceptate"
  description: |
    GroupDocs.Signature for Node.js via Java facilitează operațiunile pentru [formatele de fișiere populare](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "Caracteristicile GroupDocs.Signature"
  description: "Semnează PDF-uri, documente Office și imagini cu semnături digitale"

  items:
    # feature loop
    - icon: "sign"
      title: "Semnături de afaceri"
      content: "Folosiți diferite tipuri de semnături pentru a semna documente. Plasați semnăturile digitale exact pe orice locație a paginii."

    # feature loop
    - icon: "custom"
      title: "Personalizarea aspectului semnăturii"
      content: "Personalizați aspectele vizuale ale semnăturilor ajustând culoarea, fontul, marginile, rotația și multe altele pentru a obține rezultatul dorit."

    # feature loop
    - icon: "password"
      title: "Documente protejate prin parolă"
      content: "Pentru multe formate de documente acceptate, protejați documentele semnate cu o parolă pentru un plus de securitate."

    # feature loop
    - icon: "protect"
      title: "Prevenirea modificărilor neautorizate"
      content: "Protejați documentele de afaceri esențiale semnate cu certificate digitale de modificări neautorizate."

    # feature loop
    - icon: "convert"
      title: "Formatele de ieșire dorite"
      content: "Obțineți fără efort documente semnate în orice format acceptat. Convertiți cu ușurință documentele MS Word în format PDF."

    # feature loop
    - icon: "preview"
      title: "Previzualizarea documentelor"
      content: "Salvați pagini individuale de document ca imagini pentru nevoile viitoare."

    # feature loop
    - icon: "search"
      title: "Căutare semnătură"
      content: "Preluați informații despre semnăturile adăugate anterior în documentele dvs."

    # feature loop
    - icon: "validate"
      title: "Validarea documentului"
      content: "Verificați autenticitatea semnăturilor prezentate în orice document."

    # feature loop
    - icon: "update"
      title: "Managementul semnăturilor"
      content: "Ștergeți, mutați sau modificați semnăturile plasate pe orice pagină a documentului."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemple de cod"
  description: "Exemple ilustrative care prezintă operațiuni tipice GroupDocs.Signature for Node.js via Java"
  items:
    # code sample loop
    - title: "Marcați PDF-ul cu coduri QR"
      content: |
        Încorporarea [codurilor de bare](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) în anumite pagini de document PDF poate eficientiza procesele de afaceri. Această secțiune oferă un exemplu de adăugare a unui cod QR utilizând GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Cum să puneți codul QR în PDF.">}}
        ```javascript {style=abap}
        // Încărcați documentul pentru semnare
        let signature = new Signature("file_to_sign.pdf");
        
        // Creați opțiuni de cod QR cu text predefinit
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configurați tipul și poziția de codare a codului QR pe ​​pagină
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Semnați documentul și salvați-l ca fișier rezultat
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Protejarea unui DOCX cu o semnătură digitală"
      content: |
        [Protejați-vă documentele](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) prin semnături bazate pe certificate digitale. Semnătura digitală vă protejează documentele de afaceri împotriva modificării conținutului.
        {{< landing/code title="Iată cum puteți asigura integritatea documentului.">}}
        ```javascript {style=abap}   
        // Încărcați documentul pentru a fi semnat digital
        let signature = new Signature("file_to_sign.docx");
        
        // Specificați opțiunile de semnare digitală și furnizați calea către fișierul de certificat
        let options = new DigitalSignOptions("certificate.pfx");

        // Setați parola certificatului
        options.Password = "1234567890";

        // Semnează documentul și salvează-l în calea dorită
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
