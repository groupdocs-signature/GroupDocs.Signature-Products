---
############################# Static ############################
layout: "landing"
date: 2024-03-04T17:52:03
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: lt
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
head_title: ".NET, Java, debesies API ir internetinių dokumentų parašų programos"
head_description: "Gaukite „viskas viename“ dokumentų el. parašo sprendimą, skirtą .NET, „Java“ ir debesies programoms. Pasirašykite įprastus dokumentų formatus internete naudodami paprastą vilkimo ir nuleidimo funkciją"

############################# Header ############################
title: "Pasirašykite dokumentus<br>su Node.js API"
description: "Pasirašykite skaitmeninius dokumentus ir vaizdus bet kurioje platformoje naudodami mūsų lanksčias API ir programuotojams ir galutiniams vartotojams skirtus sprendimus."
words:
  for: "dėl"

actions:
  main: "Atsisiųskite iš NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licencijavimas"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Pasiruošę pradėti?"
  description: "Išbandykite GroupDocs.Signature funkcijas nemokamai arba paprašykite licencijos"

release:
  title: "Išleista {0} versija"
  notes: "Pažiūrėkite, kas naujo"
  downloads: "Atsisiuntimai"

code:
  title: "PDF pasirašymas naudojant Node.js"
  more: "Daugiau pavyzdžių"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```javascript {style=abap}   
    // Pasirinkite PDF dokumentą
    let signature = new Signature("sample.pdf");
    
    // Pateikite tekstą
    let options = new TextSignOptions("John Smith");
    
    // Nustatyti spalvą
    options.ForeColor = Color.Red;
    
    // Pasirašykite dokumentą ir išsaugokite faile
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Parašo apžvalga"
  description: "Dokumentų pasirašymo biblioteka, paruošta naudoti Node.js programose"
  features:
    # feature loop
    - title: "Skaitmeninių parašų sprendimas verslo dokumentams su Node.js"
      content: "GroupDocs.Signature for Node.js via Java siūlo platų PDF, „Office“ dokumentų ir vaizdų skaitmeninio parašo parinkčių rinkinį. Galimas tekstas, brūkšniniai kodai, vaizdai, skaitmeniniai sertifikatai ir metaduomenys. Supaprastintas dokumentų apdorojimas užtikrina efektyvumą."

    # feature loop
    - title: "Pažangus pasirašytų dokumentų manipuliavimas"
      content: "GroupDocs.Signature suteikia jums galimybę apdoroti pasirašytus dokumentus. Ieškokite ir patvirtinkite parašus naudodami įvairius kriterijus. Be to, išskleiskite išsamią dokumento informaciją arba generuokite puslapių peržiūros vaizdus."

    # feature loop
    - title: "Įvairūs išvesties formatai"
      content: "Mūsų sprendimas suteikia plačią pasirašytų dokumentų išvesties formato kontrolę. Tiksliai išdėstykite parašus bet kuriame puslapyje ir pritaikykite jų išvaizdą. Išsaugokite pasirašytus dokumentus daugeliu palaikomų formatų ir pasirinktinai apsaugokite juos slaptažodžiais."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platformos nepriklausomybė"
  description: "GroupDocs.Signature for Node.js via Java apdoroja dokumentus su įvairiomis operacinėmis sistemomis"
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
  title: "Palaikomi failų formatai"
  description: |
    GroupDocs.Signature for Node.js via Java palengvina [populiarių failų formatų](https://docs.groupdocs.com/signature/java/supported-document-formats/) operacijas.
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office formatai
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Vaizdai ir kiti formatai
        * **Nešiojami:** PDF
        * **Vaizdai:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Kiti biuro formatai:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Kiti formatai
        * **Žiniatinklis:** HTML, MHTML
        * **Archyvai:** ZIP, TAR, 7Z
        * **Sertifikatai:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature funkcijos"
  description: "Pasirašykite PDF, Office dokumentus ir vaizdus skaitmeniniais parašais"

  items:
    # feature loop
    - icon: "sign"
      title: "Verslo parašai"
      content: "Pasirašyti dokumentus naudokite įvairių tipų parašus. Tiksliai įdėkite skaitmeninius parašus bet kurioje puslapio vietoje."

    # feature loop
    - icon: "custom"
      title: "Parašo išvaizdos tinkinimas"
      content: "Pritaikykite vizualius parašų aspektus koreguodami spalvą, šriftą, kraštines, pasukimą ir daugiau, kad pasiektumėte norimą rezultatą."

    # feature loop
    - icon: "password"
      title: "Slaptažodžiu apsaugoti dokumentai"
      content: "Daugeliui palaikomų dokumentų formatų apsaugokite pasirašytus dokumentus slaptažodžiu, kad padidintumėte saugumą."

    # feature loop
    - icon: "protect"
      title: "Neleistinų modifikacijų prevencija"
      content: "Apsaugokite svarbiausius verslo dokumentus, pasirašytus skaitmeniniais sertifikatais, nuo neteisėtų pakeitimų."

    # feature loop
    - icon: "convert"
      title: "Norimi išvesties formatai"
      content: "Lengvai gaukite pasirašytus dokumentus bet kokiu palaikomu formatu. Lengvai konvertuokite MS Word dokumentus į PDF formatą."

    # feature loop
    - icon: "preview"
      title: "Dokumentų peržiūra"
      content: "Išsaugokite atskirus dokumento puslapius kaip vaizdus būsimiems poreikiams."

    # feature loop
    - icon: "search"
      title: "Parašo paieška"
      content: "Gaukite informaciją apie anksčiau pridėtus parašus savo dokumentuose."

    # feature loop
    - icon: "validate"
      title: "Dokumento patvirtinimas"
      content: "Patikrinkite bet kuriame dokumente pateiktų parašų autentiškumą."

    # feature loop
    - icon: "update"
      title: "Parašo valdymas"
      content: "Ištrinkite, perkelkite arba modifikuokite bet kuriame dokumento puslapyje esančius parašus."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kodo pavyzdžiai"
  description: "Iliustratyvūs pavyzdžiai, demonstruojantys įprastas GroupDocs.Signature for Node.js via Java operacijas"
  items:
    # code sample loop
    - title: "Pažymėkite PDF su QR kodais"
      content: |
        [Brūkšninių kodų](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) įtraukimas į konkrečius PDF dokumentų puslapius gali supaprastinti verslo procesus. Šioje skiltyje pateikiamas QR kodo pridėjimo naudojant GroupDocs.Signature for Node.js via Java pavyzdys.
        {{< landing/code title="Kaip įdėti QR kodą į PDF.">}}
        ```javascript {style=abap}
        // Įdėkite dokumentą pasirašyti
        let signature = new Signature("file_to_sign.pdf");
        
        // Sukurkite QR kodo parinktis su iš anksto nustatytu tekstu
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigūruokite QR kodo kodavimo tipą ir vietą puslapyje
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Pasirašykite dokumentą ir išsaugokite jį kaip rezultato failą
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX apsauga skaitmeniniu parašu"
      content: |
        [Apsaugokite savo dokumentus](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) parašais, pagrįstais skaitmeniniais sertifikatais. Skaitmeninis parašas apsaugo jūsų verslo dokumentus nuo turinio pasikeitimo.
        {{< landing/code title="Štai kaip užtikrinti dokumento vientisumą.">}}
        ```javascript {style=abap}   
        // Įkelkite dokumentą, kurį norite pasirašyti skaitmeniniu būdu
        let signature = new Signature("file_to_sign.pdf");
        
        // Nurodykite skaitmeninio pasirašymo parinktis ir nurodykite kelią į sertifikato failą
        let options = new DigitalSignOptions("certificate.pfx");

        // Nustatykite sertifikato slaptažodį
        options.Password = "1234567890";

        // Pasirašykite dokumentą ir išsaugokite jį norimame kelyje
        signature.Sign("digitally_signed.pdf", options);

        ```
        {{< /landing/code >}}

---
