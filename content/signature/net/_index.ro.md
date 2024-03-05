---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
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
head_title: ".NET, Java, API-uri cloud și aplicații online pentru semnătura documentelor"
head_description: "Obțineți o soluție de semnătură electronică pentru documente all-in-one pentru .NET, Java și aplicații bazate pe cloud. Semnează online formate comune de documente folosind funcția simplă de glisare și plasare"

############################# Header ############################
title: "Semnează documente<br>prin .NET API"
description: "Semnează documente și imagini digitale pe orice platformă folosind API-urile noastre flexibile și soluțiile bazate pe aplicații pentru programatori și utilizatori finali."
words:
  for: "pentru"

actions:
  main: "Descărcare gratuită NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licențiere"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Sunteți gata să începeți?"
  description: "Încercați gratuit funcțiile GroupDocs.Signature sau solicitați o licență"

release:
  title: "Versiunea {0} a fost lansată"
  notes: "Vezi ce este nou"
  downloads: "Descărcări"

code:
  title: "Semnează fișiere PDF în C#"
  more: "Mai multe exemple"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Selectați documentul PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Furnizați text
        var options = new TextSignOptions("John Smith")
        {
            // Setați culoarea
            ForeColor = Color.Red
        };
        // Semnează documentul și salvează în fișier
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Prezentare generală GroupDocs.Signature"
  description: "API pentru efectuarea semnării documentelor și operațiunilor conexe în aplicațiile .NET"
  features:
    # feature loop
    - title: "Adăugarea de semnături la documentele de afaceri în C#"
      content: "Semnarea documentelor: Cu GroupDocs.Signature pentru .NET, puteți adăuga diferite tipuri de semnături, cum ar fi text, imagini, coduri de bare și certificate digitale, la documentele PDF și Office. Acest API vă permite să vă semnați documentele cu aproape orice tip de date, inclusiv metadate ascunse."

    # feature loop
    - title: "Prelucrarea documentelor semnate"
      content: "Procesare suplimentară: puteți efectua operațiuni puternice pe documente semnate folosind GroupDocs.Signature. Aceasta include căutarea semnăturilor existente în documentele de afaceri și verificarea lor folosind criterii specifice. În plus, puteți prelua informații despre document și pagini de previzualizare prin intermediul acestui API .NET."

    # feature loop
    - title: "Personalizarea rezultatelor"
      content: "GroupDocs.Signature pentru .NET oferă opțiuni extinse de personalizare. Puteți poziționa cu precizie semnăturile oriunde pe pagina unui document și puteți ajusta aspectul acestora folosind o varietate de setări. În plus, acest API acceptă salvarea documentelor procesate într-o gamă largă de formate acceptate."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independenta platformei"
  description: "GroupDocs.Signature pentru .NET acceptă următoarele sisteme de operare, cadre și manageri de pachete"
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
    GroupDocs.Signature pentru .NET acceptă operațiuni cu următoarele [formate de fișiere](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  description: "Semnează PDF-uri, documente Office și imagini rapid și precis"

  items:
    # feature loop
    - icon: "sign"
      title: "Semnarea documentelor"
      content: "Adăugați unul sau mai multe tipuri de semnături acceptate cu precizie la orice poziție specificată pe documentele de afaceri."

    # feature loop
    - icon: "custom"
      title: "Personalizați semnăturile"
      content: "Utilizați caracteristici precum culoarea, fontul, chenarul, rotația etc., pentru a configura aspectul semnăturilor."

    # feature loop
    - icon: "password"
      title: "Protecția prin parolă a documentului"
      content: "Securizați anumite tipuri de documente setând o parolă după semnare."

    # feature loop
    - icon: "protect"
      title: "Protecție împotriva schimbărilor"
      content: "Preveniți modificările documentelor importante de afaceri după ce adăugați o semnătură cu un certificat digital."

    # feature loop
    - icon: "convert"
      title: "Convertiți fișierele semnate în alte formate"
      content: "Convertiți fișierele semnate în formatele dorite, cum ar fi salvarea unui document Word ca PDF."

    # feature loop
    - icon: "preview"
      title: "Extrageți previzualizările paginii"
      content: "Extrageți pagini din documente semnate ca imagini individuale pentru procesări viitoare."

    # feature loop
    - icon: "search"
      title: "Căutarea semnăturilor în documente"
      content: "Preluați informații despre semnăturile adăugate anterior în anumite documente."

    # feature loop
    - icon: "validate"
      title: "Validați documentele semnate"
      content: "Verificați semnarea corectă a documentelor folosind funcții de validare."

    # feature loop
    - icon: "update"
      title: "Actualizați sau ștergeți semnăturile"
      content: "Repoziționați cu ușurință anumite semnături pe o pagină, modificați-le textul sau ștergeți-le fără probleme."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemple de cod"
  description: "Unele cazuri de utilizare tipice GroupDocs.Signature pentru operațiuni .NET"
  items:
    # code sample loop
    - title: "Adăugați codul QR în PDF"
      content: |
        Adăugarea [QR-codes](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) la anumite pagini de documente PDF poate îmbunătăți procesele de afaceri. Mai jos este un exemplu despre cum să adăugați un cod QR utilizând GroupDocs.Signature.
        {{< landing/code title="Cum să puneți codul QR în PDF.">}}
        ```csharp {style=abap}
        // Încărcați documentul pentru semnare
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Creați opțiuni de cod QR cu text predefinit
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Configurați tipul și poziția de codare a codului QR pe ​​pagină
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Semnați documentul și salvați-l ca fișier rezultat
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Protejarea unui document DOCX folosind un certificat digital"
      content: |
        Puteți [Proteja un document](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) folosind semnături personale sau corporative stocate ca certificate digitale. Astfel de documente protejate nu pot fi modificate fără invalidarea semnăturii.
        {{< landing/code title="Iată cum puteți asigura integritatea documentului.">}}
        ```csharp {style=abap}   
        // Încărcați documentul pentru a fi semnat digital
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // Specificați opțiunile de semnare digitală și furnizați calea către fișierul de certificat
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Setați parola certificatului
                Password = "1234567890"
            };
            // Semnează documentul și salvează-l în calea dorită
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---
