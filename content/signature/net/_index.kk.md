---
############################# Static ############################
layout: "landing"
date: 2023-10-23T14:58:10
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: kk
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, Cloud API және онлайн құжат қолтаңба қолданбалары"
head_description: ".NET, Java және бұлтқа негізделген қолданбалар үшін барлығы бір құжаттың электрондық қолтаңба шешімін алыңыз. Қарапайым апарып тастау мүмкіндігін пайдаланып, жалпы құжат пішіміне онлайн қол қойыңыз"

############################# Header ############################
title: "Құжаттарға қол қою<br>.NET API арқылы"
description: "Бағдарламашылар мен түпкі пайдаланушыларға арналған икемді API және қолданбаға негізделген шешімдерді пайдаланып, кез келген платформада сандық құжаттар мен кескіндерге қол қойыңыз."
words:
  for: "үшін"

actions:
  main: "NuGet тегін жүктеп алу"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Лицензиялау"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Бастауға дайынсыз ба?"
  description: "GroupDocs.Signature мүмкіндіктерін тегін пайдаланып көріңіз немесе лицензия сұраңыз"

release:
  title: "{0} нұсқасы шығарылды"
  notes: "Жаңалықтарды қараңыз"
  downloads: "Жүктеулер"

code:
  title: "C# тілінде PDF файлдарына қол қою"
  more: "Қосымша мысалдар"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // PDF құжатын таңдаңыз
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Мәтінді беру
        var options = new TextSignOptions("John Smith")
        {
            // Түс орнату
            ForeColor = Color.Red
        };
        // Құжатқа қол қойып, файлға сақтаңыз
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature шолу"
  description: ".NET қолданбаларында құжатқа қол қоюды және қатысты әрекеттерді орындауға арналған API"
  features:
    # feature loop
    - title: "C# тілінде іскери құжаттарға қолтаңбаларды қосу"
      content: "Құжаттарға қол қою: .NET үшін GroupDocs.Signature көмегімен PDF және Office құжаттарына мәтін, кескіндер, штрих-кодтар және сандық сертификаттар сияқты әртүрлі қолтаңба түрлерін қосуға болады. Бұл API құжаттарыңызға кез келген дерлік деректер түрімен, соның ішінде жасырын метадеректермен қол қоюға мүмкіндік береді."

    # feature loop
    - title: "Қол қойылған құжаттарды өңдеу"
      content: "Қосымша өңдеу: GroupDocs.Signature арқылы қол қойылған құжаттарда күшті әрекеттерді орындауға болады. Бұған бизнес құжаттарында бар қолтаңбаларды іздеу және оларды нақты критерийлер арқылы тексеру кіреді. Сонымен қатар, құжат ақпаратын шығарып алуға және осы .NET API арқылы беттерді алдын ала қарауға болады."

    # feature loop
    - title: "Нәтижелерді теңшеу"
      content: ".NET үшін GroupDocs.Signature кеңейтілген теңшеу опцияларын ұсынады. Қолтаңбаларды құжат бетінің кез келген жеріне дәл орналастырып, әртүрлі параметрлерді пайдаланып олардың көрінісін реттеуге болады. Сонымен қатар, бұл API өңделген құжаттарды қолдау көрсетілетін пішімдердің кең ауқымында сақтауды қолдайды."

############################# Platforms ############################
platforms:
  enable: true
  title: "Платформаның тәуелсіздігі"
  description: "GroupDocs.Signature for .NET келесі операциялық жүйелерге, фреймворктарға және пакет менеджерлеріне қолдау көрсетеді"
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
  title: "Қолдау көрсетілетін файл пішімдері"
  description: |
    .NET үшін GroupDocs.Signature келесі [файл пішімдері](https://docs.groupdocs.com/signature/net/supported-document-formats/) бар әрекеттерді қолдайды.
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office пішімдері
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Суреттер және басқа пішімдер
        * **Портативті:** PDF
        * **Суреттер:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Басқа кеңсе пішімдері:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Басқа форматтар
        * **желі:** HTML, MHTML
        * **Мұрағаттар:** ZIP, TAR, 7Z
        * **Сертификаттар:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Қол қою мүмкіндіктері"
  description: "PDF файлдарына, кеңсе құжаттарына және кескіндерге жылдам және дәл қол қою"

  items:
    # feature loop
    - icon: "sign"
      title: "Құжатқа қол қою"
      content: "Іскерлік құжаттардағы кез келген көрсетілген орынға бір немесе бірнеше қолдау көрсетілетін қолтаңба түрлерін дәл қосыңыз."

    # feature loop
    - icon: "custom"
      title: "Қолтаңбаларды теңшеу"
      content: "Қолтаңбалардың көрінісін конфигурациялау үшін түс, қаріп, жиек, бұру, т.б. сияқты мүмкіндіктерді пайдаланыңыз."

    # feature loop
    - icon: "password"
      title: "Құжатты құпия сөзбен қорғау"
      content: "Қол қойғаннан кейін құпия сөз орнату арқылы белгілі бір құжат түрлерін қорғаңыз."

    # feature loop
    - icon: "protect"
      title: "Өзгерістерден қорғау"
      content: "Сандық сертификаты бар қолтаңбаны қосқаннан кейін маңызды бизнес құжаттарына өзгерістер енгізуге жол бермеңіз."

    # feature loop
    - icon: "convert"
      title: "Қол қойылған файлдарды басқа пішімдерге түрлендіру"
      content: "Қол қойылған файлдарды қажетті пішімдерге түрлендіру, мысалы, Word құжатын PDF ретінде сақтау."

    # feature loop
    - icon: "preview"
      title: "Беттің алдын ала қарауларын шығарып алыңыз"
      content: "Болашақта өңдеу үшін жеке кескіндер ретінде қол қойылған құжаттардан беттерді шығарып алыңыз."

    # feature loop
    - icon: "search"
      title: "Құжаттардағы қолтаңбаны іздеу"
      content: "Арнайы құжаттардағы бұрын қосылған қолтаңбалар туралы ақпаратты шығарып алыңыз."

    # feature loop
    - icon: "validate"
      title: "Қол қойылған құжаттарды растау"
      content: "Валидация мүмкіндіктерін пайдаланып құжаттарға дұрыс қол қоюды тексеріңіз."

    # feature loop
    - icon: "update"
      title: "Қолтаңбаларды жаңарту немесе жою"
      content: "Беттегі арнайы қолтаңбалардың орнын оңай өзгертіңіз, олардың мәтінін өзгертіңіз немесе ешбір мәселесіз жойыңыз."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Код үлгілері"
  description: "Кейбіреулер .NET операциялары үшін әдеттегі GroupDocs.Signature жағдайларын пайдаланады"
  items:
    # code sample loop
    - title: "PDF файлына QR кодын қосыңыз"
      content: |
        PDF құжаттарының арнайы беттеріне [QR-кодтарын](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) қосу бизнес процестерін жақсартады. Төменде GroupDocs.Signature арқылы QR кодын қосудың мысалы берілген.
        {{< landing/code title="QR кодын PDF файлына қалай қоюға болады.">}}
        ```csharp {style=abap}
        // Қол қою үшін құжатты жүктеңіз
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Алдын ала анықталған мәтінмен QR коды опцияларын жасаңыз
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Беттегі QR кодын кодтау түрі мен орнын конфигурациялаңыз
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Құжатқа қол қойыңыз және оны нәтиже файлы ретінде сақтаңыз
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX құжатын цифрлық сертификат арқылы қорғау"
      content: |
        Сандық сертификаттар ретінде сақталған жеке немесе корпоративтік қолтаңбаларды пайдаланып, [Құжатты қорғауға](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) болады. Мұндай қорғалған құжаттарды қолды жарамсыз деп өзгертуге болмайды.
        {{< landing/code title="Міне, құжаттың тұтастығын қамтамасыз ету жолы.">}}
        ```csharp {style=abap}   
        // Цифрлық қол қою үшін құжатты жүктеңіз
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Сандық қол қою опцияларын көрсетіңіз және сертификат файлына жолды беріңіз
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Сертификат құпия сөзін орнатыңыз
                Password = "1234567890"
            };
            // Құжатқа қол қойып, оны қажетті жолға сақтаңыз
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
