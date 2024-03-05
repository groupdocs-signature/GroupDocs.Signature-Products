---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: hu
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
head_title: ".NET, Java, felhő API-k és online dokumentum-aláíró alkalmazások"
head_description: "Szerezzen minden az egyben dokumentum-aláírási megoldást .NET, Java és felhőalapú alkalmazásokhoz. A gyakori dokumentumformátumok online aláírása egyszerű fogd és vidd funkcióval"

############################# Header ############################
title: "Írja alá a dokumentumokat<br>Node.js API-val"
description: "A programozóknak és végfelhasználóknak szánt rugalmas API-jaink és alkalmazásalapú megoldásaink segítségével bármilyen platformon aláírhat digitális dokumentumokat és képeket."
words:
  for: "számára"

actions:
  main: "Töltse le az NPM-ről"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Engedélyezés"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Készen áll az indulásra?"
  description: "Próbálja ki a GroupDocs.Signature szolgáltatásait ingyenesen, vagy kérjen licencet"

release:
  title: "A(z) {0} verzió megjelent"
  notes: "Tekintse meg az újdonságokat"
  downloads: "Letöltések"

code:
  title: "PDF-ek aláírása a Node.js segítségével"
  more: "További példák"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Válassza ki a PDF dokumentumot
    let signature = new Signature("sample.pdf");
    
    // Szöveg megadása
    let options = new TextSignOptions("John Smith");
    
    // Állítsa be a színt
    options.ForeColor = Color.Red;
    
    // Írja alá a dokumentumot és mentse el a fájlba
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature áttekintése"
  description: "Dokumentum-aláíró könyvtár, amely készen áll a Node.js alkalmazásokban való használatra"
  features:
    # feature loop
    - title: "Digitális aláírási megoldás üzleti dokumentumokhoz a Node.js segítségével"
      content: "A GroupDocs.Signature for Node.js via Java a digitális aláírási lehetőségek átfogó készletét kínálja PDF, Office dokumentumok és képek számára. Szöveg, vonalkód, képek, digitális tanúsítványok és metaadatok állnak rendelkezésre. Az egyszerűsített dokumentumfeldolgozás biztosítja a hatékonyságot."

    # feature loop
    - title: "Az aláírt dokumentumok haladó kezelése"
      content: "A GroupDocs.Signature feljogosítja Önt aláírt dokumentumok feldolgozására. Aláírások keresése és érvényesítése különféle kritériumok alapján. Ezenkívül részletes dokumentuminformációkat is kivonhat, vagy előnézeti képeket készíthet az oldalakról."

    # feature loop
    - title: "Változatos kimeneti formátumok"
      content: "Megoldásunk kiterjedt szabályozást biztosít az aláírt dokumentumok kimeneti formátuma felett. Pontosan elhelyezheti az aláírásokat bármely oldalon, és testreszabhatja azok megjelenését. Az aláírt dokumentumokat számos támogatott formátumban elmentheti, és opcionálisan jelszavakkal is védheti."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platformfüggetlenség"
  description: "A GroupDocs.Signature for Node.js via Java dokumentumfeldolgozást végez különféle operációs rendszerekkel"
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
  title: "Támogatott fájlformátumok"
  description: |
    A GroupDocs.Signature for Node.js via Java megkönnyíti a [népszerű fájlformátumok](https://docs.groupdocs.com/signature/java/supported-document-formats/) műveleteit.
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office formátumok
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Képek és egyéb formátumok
        * **Hordozható:** PDF
        * **Képek:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Egyéb irodai formátumok:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Egyéb formátumok
        * **Web:** HTML, MHTML
        * **Levéltár:** ZIP, TAR, 7Z
        * **Tanúsítványok:** PFX

############################# Features ############################
features:
  enable: true
  title: "A GroupDocs.Signature szolgáltatásai"
  description: "Aláírhat PDF-eket, Office-dokumentumokat és képeket digitális aláírással"

  items:
    # feature loop
    - icon: "sign"
      title: "Üzleti aláírások"
      content: "Használjon különféle aláírási típusokat dokumentumok aláírásához. Pontosan helyezze el a digitális aláírásokat az oldal bármely helyén."

    # feature loop
    - icon: "custom"
      title: "Az aláírás megjelenésének testreszabása"
      content: "A kívánt eredmény elérése érdekében testreszabhatja az aláírások vizuális aspektusait a szín, a betűtípus, a szegélyek, az elforgatás és egyebek módosításával."

    # feature loop
    - icon: "password"
      title: "Jelszóval védett dokumentumok"
      content: "Számos támogatott dokumentumformátum esetén védje az aláírt dokumentumokat jelszóval a nagyobb biztonság érdekében."

    # feature loop
    - icon: "protect"
      title: "A jogosulatlan módosítások megelőzése"
      content: "Védje meg a digitális tanúsítvánnyal aláírt alapvető üzleti dokumentumokat a jogosulatlan módosításoktól."

    # feature loop
    - icon: "convert"
      title: "Kívánt kimeneti formátumok"
      content: "Könnyedén megkaphatja az aláírt dokumentumokat bármilyen támogatott formátumban. Könnyedén konvertálhat MS Word dokumentumokat PDF formátumba."

    # feature loop
    - icon: "preview"
      title: "Dokumentumok előnézete"
      content: "Mentse el az egyes dokumentumoldalakat képként a jövőbeli igényekhez."

    # feature loop
    - icon: "search"
      title: "Aláírás keresése"
      content: "Információk lekérése a dokumentumokban korábban hozzáadott aláírásokról."

    # feature loop
    - icon: "validate"
      title: "Dokumentum érvényesítése"
      content: "Ellenőrizze bármely dokumentumban szereplő aláírások hitelességét."

    # feature loop
    - icon: "update"
      title: "Aláíráskezelés"
      content: "Törölje, helyezze át vagy módosítsa a dokumentum bármely oldalán elhelyezett aláírásokat."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kódminták"
  description: "Szemléltető példák, amelyek a GroupDocs.Signature for Node.js via Java tipikus műveleteit mutatják be"
  items:
    # code sample loop
    - title: "Jelölje meg a PDF-et QR-kódokkal"
      content: |
        A [vonalkódok](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) konkrét PDF-dokumentumoldalakba történő beépítése leegyszerűsítheti az üzleti folyamatokat. Ez a rész egy példát mutat be QR-kód hozzáadására a GroupDocs.Signature for Node.js via Java használatával.
        {{< landing/code title="Hogyan helyezhet el QR-kódot PDF-be.">}}
        ```javascript {style=abap}
        // Töltse be az aláírandó dokumentumot
        let signature = new Signature("file_to_sign.pdf");
        
        // Hozzon létre QR-kód opciókat előre meghatározott szöveggel
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurálja a QR-kód kódolási típusát és pozícióját az oldalon
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Írja alá a dokumentumot, és mentse el eredményfájlként
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX védelme digitális aláírással"
      content: |
        [Védje meg dokumentumait](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) digitális tanúsítványokon alapuló aláírásokkal. A digitális aláírás megvédi üzleti dokumentumait a tartalom változásától.
        {{< landing/code title="Így biztosíthatja a dokumentum integritását.">}}
        ```javascript {style=abap}   
        // Töltse be a digitálisan aláírandó dokumentumot
        let signature = new Signature("file_to_sign.docx");
        
        // Adja meg a digitális aláírás beállításait, és adja meg a tanúsítványfájl elérési útját
        let options = new DigitalSignOptions("certificate.pfx");

        // Állítsa be a tanúsítvány jelszavát
        options.Password = "1234567890";

        // Írja alá a dokumentumot, és mentse el a kívánt útvonalra
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
