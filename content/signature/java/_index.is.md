---
############################# Static ############################
layout: "landing"
date: 2023-09-13T10:36:50
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: is
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, Cloud API & Online Document Signature Apps"
head_description: "Fáðu allt í einu skjalalausn fyrir rafræna undirskrift fyrir .NET, Java og skýjaforrit. Skrifaðu undir algeng skjalasnið á netinu með því að nota einfaldan draga og sleppa eiginleika"

############################# Header ############################
title: "Skrifaðu undir skjöl<br>í gegnum Java API"
description: "Skrifaðu undir stafræn skjöl og myndir á hvaða vettvang sem er með því að nota sveigjanleg API og app byggðar lausnir fyrir forritara og endanotendur."
words:
  for: "fyrir"

actions:
  main: "Maven niðurhal ókeypis"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Leyfisveitingar"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Tilbúinn til að byrja?"
  description: "Prófaðu GroupDocs.Signature eiginleika ókeypis eða biddu um leyfi"

release:
  title: "Útgáfa {0} gefin út"
  notes: "Sjáðu hvað er nýtt"
  downloads: "Niðurhal"

code:
  title: "Skráðu PDF skjöl í Java"
  more: "Fleiri dæmi"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Veldu PDF skjal
    Signature signature = new Signature("sample.pdf");
    
    // Gefðu upp texta
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Skrifaðu undir skjal og vistaðu í skrá
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Yfirlit"
  description: "API til að framkvæma undirritun skjala og tengdar aðgerðir í Java forritum"
  features:
    # feature loop
    - title: "Bætt viðskiptaskjöl með stafrænum undirskriftum í Java"
      content: "Fljótleg og sérhannaðar undirskrift: GroupDocs.Signature fyrir Java býður upp á fjölbreytt úrval af stafrænum undirskriftarmöguleikum fyrir PDF-skjöl, myndir og Office-skjöl. Þú getur notað texta, strikamerki, QR-kóða, stafræn skilríki, myndir eða falin lýsigögn. Skjalavinnslan er hröð og skilvirk."

    # feature loop
    - title: "Meðhöndla undirrituð skjöl"
      content: "Ítarleg skjalavinnsla felur í sér öflugar aðgerðir á undirrituðum skjölum með GroupDocs.Signature fyrir Java. Hægt er að leita að og staðfesta undirskriftir sem hafa verið bætt við viðskiptaskjöl með ýmsum gagnlegum forsendum. Að auki geturðu nálgast nákvæmar upplýsingar um skjalið eða fengið forskoðunarmyndir af síðum þess."

    # feature loop
    - title: "Fjölbreytt framleiðsluval"
      content: "Öflugir undirskriftarvalkostir gera þér kleift að sérsníða úttakið fyrir skjöl sem eru undirrituð með GroupDocs.Signature fyrir Java. Þú getur staðsett hvaða undirskrift sem er nákvæmlega á hvaða skjalasíðu sem er og stillt útlit hennar á ýmsa vegu. Java API styður vistun undirritaðra viðskiptaskjala á fjölmörgum studdum sniðum og býður upp á möguleika til að tryggja þau með lykilorðum."

############################# Platforms ############################
platforms:
  enable: true
  title: "Sjálfstæði vettvangs"
  description: "GroupDocs.Signature fyrir Java styður eftirfarandi stýrikerfi, ramma og pakkastjóra"
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
  title: "Stutt skráarsnið"
  description: |
    GroupDocs.Signature fyrir Java styður aðgerðir með eftirfarandi [skráarsniðum](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office snið
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Myndir og önnur snið
        * **Færanlegt:** PDF
        * **Myndir:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Önnur skrifstofusnið:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Önnur snið
        * **vefur:** HTML, MHTML
        * **Skjalasafn:** ZIP, TAR, 7Z
        * **Skírteini:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature eiginleikar"
  description: "Undirritun PDF skjöl, skrifstofuskjöl og myndir með stafrænum undirskriftum"

  items:
    # feature loop
    - icon: "merge"
      title: "Að bæta við undirskriftum"
      content: "Skrifaðu undir skjal með því að nota ýmsar studdar undirskriftargerðir með því að setja stafræna undirskrift nákvæmlega hvar sem er á hvaða síðu sem er."

    # feature loop
    - icon: "split"
      title: "Sérsníða niðurstöður"
      content: "Sérsníddu einkennisútlitið með því að stilla lit, leturgerð, ramma, snúning og aðra eiginleika til að ná tilætluðum árangri."

    # feature loop
    - icon: "move"
      title: "Að tryggja skjöl með lykilorði"
      content: "Fyrir margar studdar skjalagerðir geturðu verndað undirritaða skjalið með lykilorði."

    # feature loop
    - icon: "remove"
      title: "Koma í veg fyrir óheimilar breytingar"
      content: "Verndaðu mikilvæg viðskiptaskjöl sem eru undirrituð með stafrænu vottorði gegn óheimilum breytingum."

    # feature loop
    - icon: "rotate"
      title: "Að fá niðurstöður í æskilegu sniði"
      content: "Fáðu auðveldlega undirritaðar niðurstöðuskrár á hvaða studdu sniði sem er. Þú getur líka umbreytt MS Word skjölum í PDF áreynslulaust."

    # feature loop
    - icon: "swap"
      title: "Forskoðun skjala"
      content: "Vistaðu hvaða síðu sem er í skjali sem mynd til framtíðarvinnslu."

    # feature loop
    - icon: "extract"
      title: "Er að leita að undirskriftum"
      content: "Hægt er að fá upplýsingar um áður bættar undirskriftir í ákveðin skjöl."

    # feature loop
    - icon: "orientation"
      title: "Staðfesta skjöl"
      content: "Staðfestu réttmæti undirskrifta á hverju undirrituðu skjali."

    # feature loop
    - icon: "preview"
      title: "Umsjón með undirskriftum"
      content: "Þegar undirskrift hefur verið sett á skjalasíðu er hægt að eyða henni, færa hana eða uppfæra eftir þörfum."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kóða sýnishorn"
  description: "Sumir nota dæmigerða GroupDocs.Signature fyrir Java aðgerðir"
  items:
    # code sample loop
    - title: "Bættu PDF skjal með QR-kóða"
      content: |
        Það getur verið dýrmætt að bæta viðskiptaferla með því að bæta [QR-kóðum](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) við sérstakar síður af PDF skjölum. Það er dæmi um hvernig á að bæta við QR kóða með GroupDocs.Signature fyrir Java.
        {{< landing/code title="Bættu PDF skjal með QR-kóða">}}
        ```java {style=abap}
        // Hladdu skjalinu til að undirrita
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Búðu til QR kóða valkosti með fyrirfram skilgreindum texta
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Stilltu QR kóða kóðun gerð og staðsetningu á síðunni
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Skrifaðu undir skjalið og vistaðu það sem niðurstöðuskrá
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Notaðu stafræna undirskrift til að vernda DOCX"
      content: |
        Þú getur [verndað skjal](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) með því að nota persónulegar undirskriftir eða fyrirtækjaundirskriftir sem eru geymdar sem stafræn skilríki. Ekki er hægt að breyta skjölum sem eru tryggð með vottorði án þess að ógilda undirskriftina.
        {{< landing/code title="Notaðu stafræna undirskrift til að vernda DOCX">}}
        ```java {style=abap}   
        // Hladdu skjalinu sem á að skrifa undir stafrænt
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Tilgreindu valkosti fyrir stafræna undirskrift og gefðu upp slóðina að vottorðaskránni
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Stilltu lykilorð vottorðsins
        options.setPassword("1234567890");

        // Skrifaðu undir skjalið og vistaðu það á viðkomandi slóð
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

############################# Reviews ############################
# reviews:
# enable: true
# title: "{reviews.title}"
# description: "{reviews.description}"

# items:
#   # review loop
#   - title: "GroupDocs.Viewer"
#     content: "{reviews.review_1.content}"
#     author: "{reviews.review_1.author}"
#     company: "{reviews.review_1.company}"

#   # review loop
#   - title: "GroupDocs.Viewer"
#     content: "{reviews.review_2.content}"
#     author: "{reviews.review_2.author}"
#     company: "{reviews.review_2.company}"
---
