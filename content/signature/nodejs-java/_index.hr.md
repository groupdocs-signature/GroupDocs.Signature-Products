---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:51
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: hr
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
head_title: "Node.js API za digitalni potpis - GroupDocs.Signature"
head_description: "Integrirajte sigurne e-potpise u Node.js aplikacije s GroupDocs.Signature. Pojednostavite radni tijek potpisivanja dokumenata jednostavno i učinkovito."

############################# Header ############################
title: "Potpišite dokumente<br>s Node.js API-jem"
description: "Potpišite digitalne dokumente i slike na bilo kojoj platformi koristeći naše fleksibilne API-je i rješenja temeljena na aplikacijama za programere i krajnje korisnike."
words:
  for: "za"

actions:
  main: "Preuzmite s NPM-a"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licenciranje"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Jeste li spremni za početak?"
  description: "Isprobajte značajke GroupDocs.Signature besplatno ili zatražite licencu"

release:
  title: "Objavljena verzija {0}"
  notes: "Pogledajte što je novo"
  downloads: "Preuzimanja"

code:
  title: "Potpisivanje PDF-ova pomoću Node.js"
  more: "Više primjera"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Odaberite PDF dokument
    let signature = new Signature("sample.pdf");
    
    // Navedite tekst
    let options = new TextSignOptions("John Smith");
    
    // Postavite boju
    options.ForeColor = Color.Red;
    
    // Potpišite dokument i spremite ga u datoteku
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Pregled GroupDocs.Signature"
  description: "Biblioteka za potpisivanje dokumenata koja je spremna za korištenje u Node.js aplikacijama"
  features:
    # feature loop
    - title: "Rješenje za digitalne potpise za poslovne dokumente s Node.js"
      content: "GroupDocs.Signature for Node.js via Java nudi opsežan skup opcija digitalnog potpisa za PDF, Office dokumente i slike. Dostupni su tekst, crtični kodovi, slike, digitalni certifikati i metapodaci. Pojednostavljena obrada dokumenata osigurava učinkovitost."

    # feature loop
    - title: "Napredno rukovanje potpisanim dokumentima"
      content: "GroupDocs.Signature vam omogućuje obradu potpisanih dokumenata. Pretražujte i potvrđujte potpise koristeći različite kriterije. Osim toga, izvucite detaljne informacije o dokumentu ili generirajte slike za pregled stranica."

    # feature loop
    - title: "Različiti izlazni formati"
      content: "Naše rješenje pruža opsežnu kontrolu nad izlaznim formatom potpisanih dokumenata. Precizno pozicionirajte potpise na bilo kojoj stranici i prilagodite njihov izgled. Spremite potpisane dokumente u brojnim podržanim formatima i opcionalno ih zaštitite lozinkama."

############################# Platforms ############################
platforms:
  enable: true
  title: "Neovisnost o platformi"
  description: "GroupDocs.Signature for Node.js via Java izvodi obradu dokumenata s različitim operativnim sustavima"
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
  title: "Podržani formati datoteka"
  description: |
    GroupDocs.Signature for Node.js via Java olakšava rad za [popularne formate datoteka](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office formati
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Slike i drugi formati
        * **Prijenosni:** PDF
        * **Slike:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Ostali uredski formati:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Ostali formati
        * **mreža:** HTML, MHTML
        * **Arhiva:** ZIP, TAR, 7Z
        * **Certifikati:** PFX

############################# Features ############################
features:
  enable: true
  title: "Značajke GroupDocs.Signature"
  description: "Potpišite PDF-ove, Office dokumente i slike digitalnim potpisima"

  items:
    # feature loop
    - icon: "sign"
      title: "Poslovni potpisi"
      content: "Koristite različite vrste potpisa za potpisivanje dokumenata. Precizno postavite digitalne potpise na bilo koju stranicu."

    # feature loop
    - icon: "custom"
      title: "Prilagodba izgleda potpisa"
      content: "Prilagodite vizualne aspekte potpisa podešavanjem boje, fonta, obruba, rotacije i još mnogo toga kako biste postigli željeni rezultat."

    # feature loop
    - icon: "password"
      title: "Dokumenti zaštićeni lozinkom"
      content: "Za mnoge podržane formate dokumenata zaštitite potpisane dokumente lozinkom za dodatnu sigurnost."

    # feature loop
    - icon: "protect"
      title: "Sprječavanje neovlaštenih izmjena"
      content: "Zaštitite ključne poslovne dokumente potpisane digitalnim certifikatima od neovlaštenih izmjena."

    # feature loop
    - icon: "convert"
      title: "Željeni izlazni formati"
      content: "Bez napora nabavite potpisane dokumente u bilo kojem podržanom formatu. Pretvorite MS Word dokumente u PDF format s lakoćom."

    # feature loop
    - icon: "preview"
      title: "Pregled dokumenata"
      content: "Spremite pojedinačne stranice dokumenta kao slike za buduće potrebe."

    # feature loop
    - icon: "search"
      title: "Pretraga potpisa"
      content: "Dohvatite informacije o prethodno dodanim potpisima unutar vaših dokumenata."

    # feature loop
    - icon: "validate"
      title: "Provjera valjanosti dokumenata"
      content: "Provjerite vjerodostojnost potpisa u bilo kojem dokumentu."

    # feature loop
    - icon: "update"
      title: "Upravljanje potpisom"
      content: "Izbrišite, premjestite ili modificirajte sve potpise postavljene na bilo koju stranicu dokumenta."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Uzorci kodova"
  description: "Ilustrativni primjeri koji prikazuju tipične GroupDocs.Signature for Node.js via Java operacije"
  items:
    # code sample loop
    - title: "Označite PDF QR kodovima"
      content: |
        Uključivanje [crtičnih kodova](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) u određene stranice PDF dokumenta može pojednostaviti poslovne procese. Ovaj odjeljak pruža primjer dodavanja QR koda pomoću GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Kako staviti QR kod u PDF.">}}
        ```javascript {style=abap}
        // Učitajte dokument za potpisivanje
        let signature = new Signature("file_to_sign.pdf");
        
        // Stvorite opcije QR koda s unaprijed definiranim tekstom
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurirajte vrstu kodiranja QR koda i položaj na stranici
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Potpišite dokument i spremite ga kao datoteku rezultata
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Zaštita DOCX-a digitalnim potpisom"
      content: |
        [Zaštitite svoje dokumente](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) potpisima na temelju digitalnih certifikata. Digitalni potpis štiti vaše poslovne dokumente od promjene sadržaja.
        {{< landing/code title="Evo kako osigurati integritet dokumenta.">}}
        ```javascript {style=abap}   
        // Učitajte dokument koji želite digitalno potpisati
        let signature = new Signature("file_to_sign.docx");
        
        // Navedite opcije digitalnog potpisivanja i navedite put do datoteke certifikata
        let options = new DigitalSignOptions("certificate.pfx");

        // Postavite lozinku certifikata
        options.Password = "1234567890";

        // Potpišite dokument i spremite ga na željenu putanju
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
