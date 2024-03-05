---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: kk
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
head_title: ".NET, Java, Cloud API және онлайн құжат қолтаңба қолданбалары"
head_description: ".NET, Java және бұлтқа негізделген қолданбалар үшін барлығы бір құжаттың электрондық қолтаңба шешімін алыңыз. Қарапайым апарып тастау мүмкіндігін пайдаланып, жалпы құжат пішіміне онлайн қол қойыңыз"

############################# Header ############################
title: "Құжаттарға қол қою<br>Node.js API көмегімен"
description: "Бағдарламашылар мен түпкі пайдаланушыларға арналған икемді API және қолданбаға негізделген шешімдерді пайдаланып, кез келген платформада сандық құжаттар мен кескіндерге қол қойыңыз."
words:
  for: "үшін"

actions:
  main: "NPM сайтынан жүктеп алыңыз"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Лицензиялау"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Бастауға дайынсыз ба?"
  description: "GroupDocs.Signature мүмкіндіктерін тегін пайдаланып көріңіз немесе лицензия сұраңыз"

release:
  title: "{0} нұсқасы шығарылды"
  notes: "Жаңалықтарды қараңыз"
  downloads: "Жүктеулер"

code:
  title: "Node.js арқылы PDF файлдарына қол қою"
  more: "Қосымша мысалдар"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // PDF құжатын таңдаңыз
    let signature = new Signature("sample.pdf");
    
    // Мәтінді беру
    let options = new TextSignOptions("John Smith");
    
    // Түс орнату
    options.ForeColor = Color.Red;
    
    // Құжатқа қол қойып, файлға сақтаңыз
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature шолу"
  description: "Node.js қолданбаларында пайдалануға дайын құжаттарға қол қою кітапханасы"
  features:
    # feature loop
    - title: "Node.js бар іскери құжаттарға арналған сандық қолтаңбалар шешімі"
      content: "GroupDocs.Signature for Node.js via Java PDF, Office құжаттары мен кескіндері үшін сандық қолтаңба опцияларының жан-жақты жинағын ұсынады. Мәтін, штрих-кодтар, суреттер, сандық сертификаттар және метадеректер қол жетімді. Құжаттарды өңдеу тиімділікті қамтамасыз етеді."

    # feature loop
    - title: "Қол қойылған құжаттармен кеңейтілген манипуляция"
      content: "GroupDocs.Signature қол қойылған құжаттарды өңдеуге мүмкіндік береді. Әртүрлі критерийлер арқылы қолтаңбаларды іздеңіз және растаңыз. Қосымша құжат туралы толық ақпаратты шығарып алыңыз немесе беттердің алдын ала қарау кескіндерін жасаңыз."

    # feature loop
    - title: "Әртүрлі шығыс пішімдері"
      content: "Біздің шешіміміз қол қойылған құжаттардың шығу пішімін кең бақылауды қамтамасыз етеді. Қолтаңбаларды кез келген бетте дәл орналастырыңыз және олардың сыртқы түрін реттеңіз. Қол қойылған құжаттарды көптеген қолдау көрсетілетін пішімдерде сақтаңыз және оларды құпия сөздермен қорғаңыз."

############################# Platforms ############################
platforms:
  enable: true
  title: "Платформаның тәуелсіздігі"
  description: "GroupDocs.Signature for Node.js via Java әртүрлі операциялық жүйелермен құжаттарды өңдеуді жүзеге асырады"
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
    GroupDocs.Signature for Node.js via Java [танымал файл пішімдері](https://docs.groupdocs.com/signature/java/supported-document-formats/) үшін операцияларды жеңілдетеді.
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
  title: "GroupDocs.Signature мүмкіндіктері"
  description: "PDF файлдарына, Office құжаттарына және кескіндерге цифрлық қолтаңбамен қол қойыңыз"

  items:
    # feature loop
    - icon: "sign"
      title: "Іскерлік қолтаңбалар"
      content: "Құжаттарға қол қою үшін әртүрлі қолтаңба түрлерін қолданыңыз. Цифрлық қолтаңбаны кез келген бетке дәл орналастырыңыз."

    # feature loop
    - icon: "custom"
      title: "Қолтаңба көрінісін теңшеу"
      content: "Қажетті нәтижеге қол жеткізу үшін түсті, қаріпті, жиектерді, айналдыруды және т.б. реттеу арқылы қолтаңбалардың көрнекі аспектілерін бейімдеңіз."

    # feature loop
    - icon: "password"
      title: "Құпия сөзбен қорғалған құжаттар"
      content: "Көптеген қолдау көрсетілетін құжат пішімдері үшін қосымша қауіпсіздік үшін қол қойылған құжаттарды құпия сөзбен қорғаңыз."

    # feature loop
    - icon: "protect"
      title: "Рұқсат етілмеген өзгертулердің алдын алу"
      content: "Сандық сертификаттармен қол қойылған маңызды бизнес құжаттарды рұқсатсыз өзгертулерден қорғаңыз."

    # feature loop
    - icon: "convert"
      title: "Қажетті шығыс пішімдері"
      content: "Қолдау көрсетілетін кез келген форматта қол қойылған құжаттарды оңай алыңыз. MS Word құжаттарын PDF пішіміне оңай түрлендіріңіз."

    # feature loop
    - icon: "preview"
      title: "Құжаттарды алдын ала қарау"
      content: "Жеке құжат беттерін болашақ қажеттіліктер үшін кескіндер ретінде сақтаңыз."

    # feature loop
    - icon: "search"
      title: "Қолтаңбаны іздеу"
      content: "Құжаттарыңызда бұрын қосылған қолтаңбалар туралы ақпаратты шығарып алыңыз."

    # feature loop
    - icon: "validate"
      title: "Құжатты тексеру"
      content: "Кез келген құжатта қойылған қолдардың түпнұсқалығын тексеріңіз."

    # feature loop
    - icon: "update"
      title: "Қолтаңбаны басқару"
      content: "Кез келген құжат бетінде орналастырылған қолтаңбаларды жойыңыз, орнын ауыстырыңыз немесе өзгертіңіз."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Код үлгілері"
  description: "Әдеттегі GroupDocs.Signature for Node.js via Java операцияларын көрсететін көрнекі мысалдар"
  items:
    # code sample loop
    - title: "QR кодтары бар PDF файлын белгілеңіз"
      content: |
        Арнайы PDF құжат беттеріне [штрихкодтарды](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) қосу бизнес процестерін жеңілдетеді. Бұл бөлім GroupDocs.Signature for Node.js via Java арқылы QR кодын қосу мысалын береді.
        {{< landing/code title="QR кодын PDF файлына қалай қоюға болады.">}}
        ```javascript {style=abap}
        // Қол қою үшін құжатты жүктеңіз
        let signature = new Signature("file_to_sign.pdf");
        
        // Алдын ала анықталған мәтінмен QR коды опцияларын жасаңыз
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Беттегі QR кодын кодтау түрі мен орнын конфигурациялаңыз
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Құжатқа қол қойыңыз және оны нәтиже файлы ретінде сақтаңыз
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX жүйесін цифрлық қолтаңбамен қорғау"
      content: |
        [Құжаттарды қорғау](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) цифрлық сертификаттарға негізделген қолтаңбалар арқылы. Цифрлық қолтаңба бизнес құжаттарыңызды мазмұнды өзгертуден қорғайды.
        {{< landing/code title="Міне, құжаттың тұтастығын қамтамасыз ету жолы.">}}
        ```javascript {style=abap}   
        // Цифрлық қол қою үшін құжатты жүктеңіз
        let signature = new Signature("file_to_sign.docx");
        
        // Сандық қол қою опцияларын көрсетіңіз және сертификат файлына жолды беріңіз
        let options = new DigitalSignOptions("certificate.pfx");

        // Сертификат құпия сөзін орнатыңыз
        options.Password = "1234567890";

        // Құжатқа қол қойып, оны қажетті жолға сақтаңыз
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
