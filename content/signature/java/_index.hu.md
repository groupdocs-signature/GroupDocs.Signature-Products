---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:49
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
head_title: "Java digitális aláírás könyvtár - GroupDocs.Signature"
head_description: "Engedélyezze a Java-alkalmazásokat e-aláírásokkal a GroupDocs.Signature segítségével. Aláírja az üzleti dokumentumokat gyorsan és könnyedén."

############################# Header ############################
title: "Írja alá a dokumentumokat<br>Java API-n keresztül"
description: "A programozóknak és végfelhasználóknak szánt rugalmas API-jaink és alkalmazásalapú megoldásaink segítségével bármilyen platformon aláírhat digitális dokumentumokat és képeket."
words:
  for: "számára"

actions:
  main: "Ingyenes Maven letöltés"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Engedélyezés"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Készen áll az indulásra?"
  description: "Próbálja ki a GroupDocs.Signature szolgáltatásait ingyenesen, vagy kérjen licencet"

release:
  title: "A(z) {0} verzió megjelent"
  notes: "Tekintse meg az újdonságokat"
  downloads: "Letöltések"

code:
  title: "PDF fájlok aláírása Java nyelven"
  more: "További példák"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Válassza ki a PDF dokumentumot
    Signature signature = new Signature("sample.pdf");
    
    // Szöveg megadása
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Írja alá a dokumentumot és mentse el a fájlba
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature áttekintése"
  description: "API dokumentum-aláírási és kapcsolódó műveletek végrehajtásához Java alkalmazásokban"
  features:
    # feature loop
    - title: "Továbbfejlesztett üzleti dokumentumok digitális aláírással Java nyelven"
      content: "Gyors és testreszabható aláírás: A GroupDocs.Signature for Java a digitális aláírási lehetőségek széles skáláját kínálja PDF-ekhez, képekhez és Office-dokumentumokhoz. Használhat szöveget, vonalkódokat, QR-kódokat, digitális tanúsítványokat, képeket vagy rejtett metaadatokat. A dokumentumfeldolgozás gyors és hatékony."

    # feature loop
    - title: "Az aláírt dokumentumok kezelése"
      content: "A fejlett dokumentumfeldolgozás hatékony műveleteket foglal magában az aláírt dokumentumokon a GroupDocs.Signature for Java használatával. Különféle hasznos kritériumok segítségével megkeresheti és ellenőrizheti az üzleti dokumentumokhoz hozzáadott aláírásokat. Ezenkívül hozzáférhet a dokumentumra vonatkozó részletes információkhoz, vagy előnézeti képeket kaphat az oldalairól."

    # feature loop
    - title: "Különféle kimeneti lehetőségek"
      content: "A robusztus aláírási lehetőségek lehetővé teszik a GroupDocs.Signature for Java programmal aláírt dokumentumok kimenetének testreszabását. Bármely aláírást pontosan elhelyezhet bármely dokumentumoldalon, és különféle módokon konfigurálhatja annak megjelenését. A Java API támogatja az aláírt üzleti dokumentumok mentését számos támogatott formátumban, és lehetőséget biztosít ezek jelszavas biztosítására."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platformfüggetlenség"
  description: "A GroupDocs.Signature for Java a következő operációs rendszereket, keretrendszereket és csomagkezelőket támogatja"
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
  title: "Támogatott fájlformátumok"
  description: |
    A GroupDocs.Signature for Java a következő [fájlformátumokkal](https://docs.groupdocs.com/signature/java/supported-document-formats/) támogatja a műveleteket.
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
  description: "PDF-ek, Office-dokumentumok és képek aláírása digitális aláírással"

  items:
    # feature loop
    - icon: "sign"
      title: "Aláírások hozzáadása"
      content: "Aláírjon egy dokumentumot különböző támogatott aláírástípusokkal úgy, hogy digitális aláírást helyez el precízen, bármely oldal bármely pontján."

    # feature loop
    - icon: "custom"
      title: "Az eredmények testreszabása"
      content: "Testreszabhatja az aláírás megjelenését a szín, a betűtípus, a szegély, az elforgatás és egyéb funkciók módosításával a kívánt eredmény elérése érdekében."

    # feature loop
    - icon: "password"
      title: "Dokumentumok titkosítása jelszóval"
      content: "Számos támogatott dokumentumtípus esetén az aláírt dokumentumot jelszóval védheti."

    # feature loop
    - icon: "protect"
      title: "A jogosulatlan változtatások megakadályozása"
      content: "Védje meg a digitális tanúsítvánnyal aláírt fontos üzleti dokumentumokat a jogosulatlan módosításoktól."

    # feature loop
    - icon: "convert"
      title: "Eredmények elérése a kívánt formátumban"
      content: "Könnyen beszerezhet aláírt eredményfájlokat bármilyen támogatott formátumban. Az MS Word dokumentumokat könnyedén PDF formátumba konvertálhatja."

    # feature loop
    - icon: "preview"
      title: "Dokumentum előnézete"
      content: "Mentse el a dokumentum bármely oldalát képként a későbbi feldolgozáshoz."

    # feature loop
    - icon: "search"
      title: "Aláírások keresése"
      content: "A korábban hozzáadott aláírásokról konkrét dokumentumokban lehet tájékozódni."

    # feature loop
    - icon: "validate"
      title: "A dokumentumok érvényesítése"
      content: "Minden aláírt dokumentumon ellenőrizze az aláírások helyességét."

    # feature loop
    - icon: "update"
      title: "Aláírások kezelése"
      content: "Miután egy aláírást elhelyezett egy dokumentumoldalon, szükség szerint törölheti, áthelyezheti vagy frissítheti."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kódminták"
  description: "Egyes esetekben a tipikus GroupDocs.Signature Java műveleteket használják"
  items:
    # code sample loop
    - title: "Javítsa a PDF dokumentumot QR-kóddal"
      content: |
        Értékes lehet az üzleti folyamatok fejlesztése a [QR-kódok](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) hozzáadásával a PDF-dokumentumok egyes oldalaihoz. Van egy példa QR-kód hozzáadására a GroupDocs.Signature for Java használatával.
        {{< landing/code title="Javítsa a PDF dokumentumot QR-kóddal">}}
        ```java {style=abap}
        // Töltse be az aláírandó dokumentumot
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Hozzon létre QR-kód opciókat előre meghatározott szöveggel
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurálja a QR-kód kódolási típusát és pozícióját az oldalon
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Írja alá a dokumentumot, és mentse el eredményfájlként
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Használjon digitális aláírást a DOCX védelméhez"
      content: |
        A digitális tanúsítványként tárolt személyes vagy vállalati aláírások használatával [megvédheti a dokumentumokat](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/). A tanúsítvánnyal védett dokumentumok az aláírás érvénytelenítése nélkül nem módosíthatók.
        {{< landing/code title="Használjon digitális aláírást a DOCX védelméhez">}}
        ```java {style=abap}   
        // Töltse be a digitálisan aláírandó dokumentumot
        Signature signature = new Signature("file_to_sign.docx");
        
        // Adja meg a digitális aláírás beállításait, és adja meg a tanúsítványfájl elérési útját
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Állítsa be a tanúsítvány jelszavát
        options.setPassword("1234567890");

        // Írja alá a dokumentumot, és mentse el a kívánt útvonalra
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---
