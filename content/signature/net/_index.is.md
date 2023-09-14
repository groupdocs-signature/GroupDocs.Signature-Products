---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:22
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
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, Cloud API & Online Document Signature Apps"
head_description: "Fáðu allt í einu skjalalausn fyrir rafræna undirskrift fyrir .NET, Java og skýjaforrit. Skrifaðu undir algeng skjalasnið á netinu með því að nota einfaldan draga og sleppa eiginleika"

############################# Header ############################
title: "Skrifaðu undir skjöl<br>í gegnum .NET API"
description: "Skrifaðu undir stafræn skjöl og myndir á hvaða vettvang sem er með því að nota sveigjanleg API og app byggðar lausnir fyrir forritara og endanotendur."
words:
  for: "fyrir"

actions:
  main: "Ókeypis niðurhal NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Leyfisveitingar"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Tilbúinn til að byrja?"
  description: "Prófaðu GroupDocs.Signature eiginleika ókeypis eða biddu um leyfi"

release:
  title: "Útgáfa {0} gefin út"
  notes: "Sjáðu hvað er nýtt"
  downloads: "Niðurhal"

code:
  title: "Skráðu PDF skjöl í C#"
  more: "Fleiri dæmi"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Veldu PDF skjal
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Gefðu upp texta
        var options = new TextSignOptions("John Smith")
        {
            // Stilltu lit
            ForeColor = Color.Red
        };
        // Skrifaðu undir skjal og vistaðu í skrá
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Yfirlit"
  description: "API til að framkvæma undirritun skjala og tengdar aðgerðir í .NET forritum"
  features:
    # feature loop
    - title: "Bætir undirskriftum við viðskiptaskjöl í C#"
      content: "Skjalaundirskrift: Með GroupDocs.Signature fyrir .NET geturðu bætt ýmsum gerðum undirskrifta, svo sem texta, myndum, strikamerkjum og stafrænum skilríkjum, við PDF og Office skjöl. Þetta API gerir þér kleift að undirrita skjölin þín með næstum hvaða gagnategund sem er, þar á meðal falin lýsigögn."

    # feature loop
    - title: "Vinnsla undirritaðra skjala"
      content: "Viðbótarvinnsla: Þú getur framkvæmt öflugar aðgerðir á undirrituðum skjölum með GroupDocs.Signature. Þetta felur í sér að leita að núverandi undirskriftum í viðskiptaskjölum og sannreyna þær með sérstökum forsendum. Að auki geturðu sótt skjalaupplýsingar og forskoðað síður í gegnum þetta .NET API."

    # feature loop
    - title: "Sérsníða niðurstöður"
      content: "GroupDocs.Signature fyrir .NET býður upp á víðtæka aðlögunarmöguleika. Þú getur staðsett undirskriftir nákvæmlega hvar sem er á skjalasíðu og stillt útlit þeirra með ýmsum stillingum. Ennfremur styður þetta API vistun unnum skjölum á fjölmörgum studdum sniðum."

############################# Platforms ############################
platforms:
  enable: true
  title: "Sjálfstæði vettvangs"
  description: "GroupDocs.Signature fyrir .NET styður eftirfarandi stýrikerfi, ramma og pakkastjóra"
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
  title: "Stutt skráarsnið"
  description: |
    GroupDocs.Signature fyrir .NET styður aðgerðir með eftirfarandi [skráarsniðum](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  description: "Undirritun PDF skjöl, skrifstofuskjöl og myndir hratt og örugglega"

  items:
    # feature loop
    - icon: "sign"
      title: "Undirritun skjala"
      content: "Bættu við einni eða mörgum studdum gerðum undirskrifta nákvæmlega á hvaða tilteknu stað sem er á viðskiptaskjölum."

    # feature loop
    - icon: "custom"
      title: "Sérsníða undirskriftir"
      content: "Notaðu eiginleika eins og lit, leturgerð, ramma, snúning osfrv., til að stilla útlit undirskrifta."

    # feature loop
    - icon: "password"
      title: "Skjalavörn með lykilorði"
      content: "Tryggðu ákveðnar skjalagerðir með því að setja lykilorð eftir undirritun."

    # feature loop
    - icon: "protect"
      title: "Vernd gegn breytingum"
      content: "Koma í veg fyrir breytingar á mikilvægum viðskiptaskjölum eftir að hafa bætt við undirskrift með stafrænu skilríki."

    # feature loop
    - icon: "convert"
      title: "Umbreyttu undirrituðum skrám í önnur snið"
      content: "Umbreyttu undirrituðum skrám í æskileg snið, svo sem að vista Word skjal sem PDF."

    # feature loop
    - icon: "preview"
      title: "Dragðu út forsýningar á síðu"
      content: "Dragðu út síður úr undirrituðum skjölum sem einstakar myndir til framtíðarvinnslu."

    # feature loop
    - icon: "search"
      title: "Undirskriftarleit í skjölum"
      content: "Sæktu upplýsingar um áður bættar undirskriftir í tilteknum skjölum."

    # feature loop
    - icon: "validate"
      title: "Staðfesta undirrituð skjöl"
      content: "Staðfestu rétta undirritun skjala með því að nota löggildingareiginleika."

    # feature loop
    - icon: "update"
      title: "Uppfæra eða eyða undirskriftum"
      content: "Breyttu ákveðnum undirskriftum auðveldlega á síðu, breyttu texta þeirra eða eyddu þeim án vandræða."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kóða sýnishorn"
  description: "Sumir nota dæmigerða GroupDocs.Signature fyrir .NET aðgerðir"
  items:
    # code sample loop
    - title: "Bættu QR-kóða við PDF"
      content: |
        Að bæta [QR-kóðum](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) við sérstakar síður af PDF skjölum getur aukið viðskiptaferla. Hér að neðan er dæmi um hvernig á að bæta við QR kóða með GroupDocs.Signature.
        {{< landing/code title="Hvernig á að setja QR kóða á PDF.">}}
        ```csharp {style=abap}
        // Hladdu skjalinu til að undirrita
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Búðu til QR kóða valkosti með fyrirfram skilgreindum texta
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Stilltu QR kóða kóðun gerð og staðsetningu á síðunni
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Skrifaðu undir skjalið og vistaðu það sem niðurstöðuskrá
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Að vernda DOCX skjal með stafrænu vottorði"
      content: |
        Þú getur [verndað skjal](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) með því að nota persónulegar undirskriftir eða fyrirtækjaundirskriftir sem eru geymdar sem stafræn skilríki. Slíkum vernduðum skjölum er ekki hægt að breyta án þess að ógilda undirskriftina.
        {{< landing/code title="Hér er hvernig á að tryggja heilindi skjalsins.">}}
        ```csharp {style=abap}   
        // Hladdu skjalinu sem á að skrifa undir stafrænt
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Tilgreindu valkosti fyrir stafræna undirskrift og gefðu upp slóðina að vottorðaskránni
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Stilltu lykilorð vottorðsins
                Password = "1234567890"
            };
            // Skrifaðu undir skjalið og vistaðu það á viðkomandi slóð
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
