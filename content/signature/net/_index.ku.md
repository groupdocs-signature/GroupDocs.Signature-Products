---
############################# Static ############################
layout: "landing"
date: 2023-09-13T10:36:52
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: ku
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, API-yên Cloud & Serlêdanên Îmzekirina Belgeya Serhêl"
head_description: "Ji bo .NET, Java û serîlêdanên ewr-based çareseriya e-îmzaya belgeya tev-di-yek bistînin. Formên belgeyên hevpar ên serhêl bi karanîna taybetmendiya kaş û avêtinê ya hêsan îmze bikin"

############################# Header ############################
title: "Belgeyên îmze bikin<br>bi rêya .NET API"
description: "Dokument û wêneyên dîjîtal li ser her platformê bi karanîna API-yên me yên maqûl û çareseriyên bingehîn ên sepanê ji bo bernamenûs û bikarhênerên dawîn îmze bikin."
words:
  for: "bo"

actions:
  main: "Daxistina NuGet Belaş"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Lîsanskirin"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Amade ne ku dest pê bikin?"
  description: "Taybetmendiyên GroupDocs.Signature belaş biceribîne an destûrnameyek bixwaze"

release:
  title: "Guhertoya {0} derket"
  notes: "Binêrin ka çi nû ye"
  downloads: "Downloads"

code:
  title: "Pelên PDF-ê di C# de îmze bikin"
  more: "Nimûneyên bêtir"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Belgeya PDF-ê hilbijêrin
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Nivîsar pêşkêş bikin
        var options = new TextSignOptions("John Smith")
        {
            // Rengê danîn
            ForeColor = Color.Red
        };
        // Belge îmze bikin û pelê hilînin
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Overview"
  description: "API ji bo pêkanîna îmzekirina belgeyê û operasyonên têkildar di serîlêdanên .NET de"
  features:
    # feature loop
    - title: "Di C# de li belgeyên karsaziyê zêdekirina îmzeyan"
      content: "Îmzekirina belgeyan: Bi GroupDocs.Signature ji bo .NET-ê, hûn dikarin cûrbecûr îmzeyan, wek nivîs, wêne, barkod û sertîfîkayên dîjîtal, li belgeyên PDF û Office zêde bikin. Ev API dihêle hûn belgeyên xwe bi hema hema her celeb daneyê, tevî metadata veşartî, îmze bikin."

    # feature loop
    - title: "Pêvajoya belgeyên îmzekirî"
      content: "Pêvajoya pêvek: Hûn dikarin bi karanîna GroupDocs.Signature li ser belgeyên îmzekirî operasyonên hêzdar bikin. Di vê yekê de lêgerîna îmzeyên heyî yên di nav belgeyên karsaziyê de û verastkirina wan bi karanîna pîvanên taybetî pêk tê. Wekî din, hûn dikarin bi vê .NET API-ê agahdariya belgeyê bistînin û rûpelan pêşdîtin bikin."

    # feature loop
    - title: "Xweserkirina encamên"
      content: "GroupDocs.Signature ji bo .NET vebijarkên xwerûkirinê yên berfireh pêşkêşî dike. Hûn dikarin bi rastî îmzeyan li her derê li ser rûpelek belgeyê bicîh bikin û bi karanîna cûrbecûr mîhengan xuyangê wan rast bikin. Wekî din, ev API piştgirî dide tomarkirina belgeyên pêvajoyî di nav cûrbecûr formên piştgirî de."

############################# Platforms ############################
platforms:
  enable: true
  title: "Serxwebûna platformê"
  description: "GroupDocs.Signature ji bo .NET pergalên xebitandinê yên jêrîn, çarçove û rêveberên pakêtê piştgirî dike"
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
  title: "Formatên pelê piştgirî kirin"
  description: |
    GroupDocs.Signature ji bo .NET operasyonên bi [formatên pelan] yên jêrîn piştgirî dike (https://docs.groupdocs.com/signature/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formatên Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Wêne & Formên Din
        * **Cîtêgûherr:** PDF
        * **Images:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Formên ofîsê yên din:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Formên din
        * **Tevn:** HTML, MHTML
        * **Kitik:** ZIP, TAR, 7Z
        * **Sertîfîkayên:** PFX

############################# Features ############################
features:
  enable: true
  title: "Taybetmendiyên GroupDocs.Signature"
  description: "Îmzekirina PDF, Belgeyên Ofîsê, û Wêneyan bi lez û bez"

  items:
    # feature loop
    - icon: "merge"
      title: "îmzekirina belgeyê"
      content: "Li ser her pozîsyonek diyarkirî li ser belgeyên karsaziyê yek an çend celebên piştgirîkirî yên îmzeyan rast lê zêde bikin."

    # feature loop
    - icon: "split"
      title: "Kesayetî îmzeyan"
      content: "Taybetmendiyên wekî reng, font, sînor, zivirandin, hwd., bikar bînin da ku xuyabûna îmzeyan mîheng bikin."

    # feature loop
    - icon: "move"
      title: "Parastina şîfreya belgeyê"
      content: "Piştî îmzekirinê bi danîna şîfreyek hin celeb belgeyan ewle bikin."

    # feature loop
    - icon: "remove"
      title: "Parastina ji guhertinan"
      content: "Piştî pêvekirina îmzeyek bi sertîfîkayek dîjîtal re pêşî li guhertinên belgeyên karsaziyê yên girîng bigirin."

    # feature loop
    - icon: "rotate"
      title: "Pelên îmzekirî bi formatên din veguherînin"
      content: "Pelên îmzekirî veguherînin formên xwestinê, wekî tomarkirina belgeyek Word-ê wekî PDF-ê."

    # feature loop
    - icon: "swap"
      title: "Pêşdîtinên rûpelê derxînin"
      content: "Rûpelên ji belgeyên îmzekirî wekî wêneyên kesane ji bo pêvajoyek pêşerojê derxînin."

    # feature loop
    - icon: "extract"
      title: "Di belgeyan de lêgerîna îmzeyan"
      content: "Agahdariya li ser îmzeyên ku berê di belgeyên taybetî de hatine zêdekirin bistînin."

    # feature loop
    - icon: "orientation"
      title: "Belgeyên îmzekirî rast bikin"
      content: "Bi karanîna taybetmendiyên pejirandinê, îmzekirina rast a belgeyan verast bikin."

    # feature loop
    - icon: "preview"
      title: "Îmzeyan nûve bikin an jêbikin"
      content: "Bi hêsanî îmzeyên taybetî li ser rûpelek ji nû ve bi cîh bikin, nivîsa wan biguhezînin, an bêyî pirsgirêk wan jêbirin."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Nimûneyên kodê"
  description: "Hinek rewşên tîpîk GroupDocs.Signature ji bo operasyonên .NET bikar tînin"
  items:
    # code sample loop
    - title: "QR-kodê li PDF-ê zêde bikin"
      content: |
        Zêdekirina [QR-kod](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) li ser rûpelên taybetî yên belgeyên PDF dikare pêvajoyên karsaziyê zêde bike. Li jêr mînakek e ku meriv çawa kodek QR bi karanîna GroupDocs.Signature zêde dike.
        {{< landing/code title="Meriv çawa koda QR-ê li PDF-ê dixe.">}}
        ```csharp {style=abap}
        // Belgeyê ji bo îmzekirinê barkirin
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Vebijarkên koda QR-ê bi nivîsa pêşwextkirî biafirînin
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Li ser rûpelê celeb û cîhê kodkirina koda QR-ê mîheng bikin
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Belgeyê îmze bikin û wekî pelê encamê hilînin
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Parastina belgeyek DOCX bi karanîna sertîfîkayek dîjîtal"
      content: |
        Hûn dikarin [Belgeyekê biparêzin](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) îmzeyên kesane an pargîdanî yên ku wekî sertîfîkayên dîjîtal hatine hilanîn bikar bînin. Belgeyên weha parastî bêyî betalkirina îmzeyê nayên guhertin.
        {{< landing/code title="Li vir e ku meriv çawa yekbûna belgeyê piştrast dike.">}}
        ```csharp {style=abap}   
        // Belgeya ku bi dîjîtal were imze kirin bar bikin
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Vebijarkên îmzekirina dîjîtal diyar bikin û riya pelê sertîfîkayê peyda bikin
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Şîfreya sertîfîkayê saz bikin
                Password = "1234567890"
            };
            // Belgeyê îmze bikin û li ser riya xwestinê hilînin
            signature.Sign("digitally_signed.pdf", options);
        }
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
