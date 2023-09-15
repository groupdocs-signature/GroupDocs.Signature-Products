---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:22
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: hu
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, felhő API-k és online dokumentum-aláíró alkalmazások"
head_description: "Szerezzen minden az egyben dokumentum-aláírási megoldást .NET, Java és felhőalapú alkalmazásokhoz. A gyakori dokumentumformátumok online aláírása egyszerű fogd és vidd funkcióval"

############################# Header ############################
title: "Írja alá a dokumentumokat<br>.NET API-n keresztül"
description: "A programozóknak és végfelhasználóknak szánt rugalmas API-jaink és alkalmazásalapú megoldásaink segítségével bármilyen platformon aláírhat digitális dokumentumokat és képeket."
words:
  for: "számára"

actions:
  main: "Ingyenes NuGet letöltés"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Engedélyezés"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Készen áll az indulásra?"
  description: "Próbálja ki a GroupDocs.Signature szolgáltatásait ingyenesen, vagy kérjen licencet"

release:
  title: "A(z) {0} verzió megjelent"
  notes: "Tekintse meg az újdonságokat"
  downloads: "Letöltések"

code:
  title: "PDF fájlok aláírása C#-ban"
  more: "További példák"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Válassza ki a PDF dokumentumot
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Szöveg megadása
        var options = new TextSignOptions("John Smith")
        {
            // Állítsa be a színt
            ForeColor = Color.Red
        };
        // Írja alá a dokumentumot és mentse el a fájlba
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature áttekintése"
  description: "API dokumentumok aláírására és kapcsolódó műveletek végrehajtására .NET alkalmazásokban"
  features:
    # feature loop
    - title: "Aláírások hozzáadása üzleti dokumentumokhoz C#-ban"
      content: "Dokumentumok aláírása: A GroupDocs.Signature for .NET segítségével különféle típusú aláírásokat, például szöveget, képeket, vonalkódokat és digitális tanúsítványokat adhat hozzá PDF és Office dokumentumokhoz. Ez az API lehetővé teszi a dokumentumok aláírását szinte bármilyen adattípussal, beleértve a rejtett metaadatokat is."

    # feature loop
    - title: "Aláírt dokumentumok feldolgozása"
      content: "További feldolgozás: Hatékony műveleteket hajthat végre aláírt dokumentumokon a GroupDocs.Signature segítségével. Ez magában foglalja a meglévő aláírások keresését az üzleti dokumentumokban, és azok ellenőrzését meghatározott kritériumok alapján. Ezenkívül ezen a .NET API-n keresztül lekérheti a dokumentuminformációkat és megtekintheti az oldalakat."

    # feature loop
    - title: "Az eredmények testreszabása"
      content: "A GroupDocs.Signature for .NET kiterjedt testreszabási lehetőségeket kínál. Pontosan elhelyezheti az aláírásokat a dokumentumoldalon bárhol, és különféle beállításokkal módosíthatja megjelenésüket. Ezenkívül ez az API támogatja a feldolgozott dokumentumok mentését a támogatott formátumok széles körében."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platformfüggetlenség"
  description: "A GroupDocs.Signature for .NET a következő operációs rendszereket, keretrendszereket és csomagkezelőket támogatja"
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
    A GroupDocs.Signature for .NET a következő [fájlformátumokkal](https://docs.groupdocs.com/signature/net/supported-document-formats/) támogatja a műveleteket.
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
  title: "GroupDocs.Signature funkciók"
  description: "PDF-ek, Office-dokumentumok és képek gyors és pontos aláírása"

  items:
    # feature loop
    - icon: "sign"
      title: "Dokumentum aláírása"
      content: "Adjon hozzá egy vagy több támogatott aláírástípust pontosan az üzleti dokumentumok bármely meghatározott helyén."

    # feature loop
    - icon: "custom"
      title: "Az aláírások testreszabása"
      content: "Használjon olyan funkciókat, mint a szín, a betűtípus, a keret, az elforgatás stb., az aláírások megjelenésének konfigurálásához."

    # feature loop
    - icon: "password"
      title: "Dokumentum jelszavas védelme"
      content: "Biztosítson bizonyos dokumentumtípusokat az aláírás utáni jelszó beállításával."

    # feature loop
    - icon: "protect"
      title: "Védelem a változások ellen"
      content: "Megakadályozza a fontos üzleti dokumentumok módosításait, miután egy aláírást csatolt egy digitális tanúsítvánnyal."

    # feature loop
    - icon: "convert"
      title: "Az aláírt fájlok konvertálása más formátumba"
      content: "Az aláírt fájlokat konvertálja a kívánt formátumba, például mentse el a Word-dokumentumot PDF-ként."

    # feature loop
    - icon: "preview"
      title: "Oldal-előnézetek kibontása"
      content: "Kivonja az oldalakat az aláírt dokumentumokból egyedi képként a későbbi feldolgozáshoz."

    # feature loop
    - icon: "search"
      title: "Aláírás keresés a dokumentumokban"
      content: "Információk lekérése az adott dokumentumokban korábban hozzáadott aláírásokról."

    # feature loop
    - icon: "validate"
      title: "Érvényesítse az aláírt dokumentumokat"
      content: "Ellenőrizze a dokumentumok megfelelő aláírását az érvényesítési funkciók segítségével."

    # feature loop
    - icon: "update"
      title: "Az aláírások frissítése vagy törlése"
      content: "Könnyen áthelyezheti az adott aláírásokat az oldalon, módosíthatja a szövegüket vagy törölheti őket probléma nélkül."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kódminták"
  description: "Néhány eset a tipikus GroupDocs.Signature használatához .NET műveletekhez"
  items:
    # code sample loop
    - title: "QR-kód hozzáadása a PDF-hez"
      content: |
        A [QR-kódok](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) hozzáadása a PDF-dokumentumok egyes oldalaihoz javíthatja az üzleti folyamatokat. Az alábbiakban egy példa látható QR-kód hozzáadására a GroupDocs.Signature használatával.
        {{< landing/code title="Hogyan helyezhet el QR-kódot PDF-be.">}}
        ```csharp {style=abap}
        // Töltse be az aláírandó dokumentumot
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Hozzon létre QR-kód opciókat előre meghatározott szöveggel
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Konfigurálja a QR-kód kódolási típusát és pozícióját az oldalon
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Írja alá a dokumentumot, és mentse el eredményfájlként
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX-dokumentum védelme digitális tanúsítvánnyal"
      content: |
        A [Dokumentum védelmét](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) használhatja digitális tanúsítványként tárolt személyes vagy vállalati aláírásokkal. Az ilyen védett dokumentumok az aláírás érvénytelenítése nélkül nem módosíthatók.
        {{< landing/code title="Így biztosíthatja a dokumentum integritását.">}}
        ```csharp {style=abap}   
        // Töltse be a digitálisan aláírandó dokumentumot
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Adja meg a digitális aláírás beállításait, és adja meg a tanúsítványfájl elérési útját
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Állítsa be a tanúsítvány jelszavát
                Password = "1234567890"
            };
            // Írja alá a dokumentumot, és mentse el a kívánt útvonalra
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
