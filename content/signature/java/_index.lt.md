---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "„Java“ skaitmeninio parašo API, pridėkite el. parašą prie PDF „Word Excel“ vaizdo"
head_description: "Java skaitmeninio parašo API. Elektroninio parašo biblioteka, skirta skaitmeniniam PDF, Microsoft Word, Excel skaičiuoklių, PowerPoint pristatymų ir vaizdo dokumentų formatų pasirašymui."

############################# Header ############################
title: "Java API skaitmeniniams parašams tvarkyti"
description: "Tvarkykite el. vaizdo parašą, QR kodą, brūkšninį kodą, metaduomenis, teksto ir antspaudų tipus „Java“ programose, skirtose vaizdų ir skaitmeninių dokumentų failų formatams pasirašyti."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Apžvalga"

            # button loop
            - link: "#features"
              text: "funkcijos"

            # button loop
            - link: "#support"
              text: "Palaikymas"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Tiesioginė demonstracija"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Kainodara"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API padeda kurti Java programas su elektroninio parašo funkcija, kad būtų galima pasirašyti palaikomų formatų skaitmeninius dokumentus neįdiegiant jokios išorinės programinės įrangos. Jis palaiko manipuliavimą ir valdymą įvairių tipų el. parašais, tokiais kaip vaizdas, brūkšninis kodas, QR kodas, antspaudas, tekstas, optiniai ir metaduomenys. Visi jūsų elektroniniai verslo dokumentai, pvz., „Microsoft Office Word“, „PowerPoint“ pristatymai, „Excel“ skaičiuoklės, vaizdai ir PDF failai, gali būti pasirašyti skaitmeniniu būdu, tinkinant parašo ypatybes, pvz., šešėlis, matmenys, lygiavimas ir daugiau pagal jūsų poreikius. Skaitmeninio parašo biblioteka yra paprasta ir lengva, susidedanti iš vieno DLL failo, kurį galima lengvai integruoti į naują arba esamą Java programą.  

      Naudodami GroupDocs.Signature for Java API galite įkelti visus registruotus sertifikatus iš sistemos arba rasti esamus parašus naudodami paprastą ir išplėstinę paiešką. Galimybės dirbti su slaptažodžiu apsaugotais dokumentais, nurodant bendras parašo ypatybes (teksto dydį, neskaidrumą, pasukimą, patikrinimą, šrifto ypatybes, spalvų parinktis, puslapio numerį, plotį, viršuje, kairėje ir tt) ir įvairių tipų el. parašo diegimo palaikymas daro jį patikimu. Elektroninių parašų valdymo sprendimas skaitmeniniams dokumentams.  

      GroupDocs.Signature for Java yra suderinamas su visomis Java versijomis ir palaiko populiarias operacines sistemas (Windows, Linux, MacOS), kurios gali paleisti Java Runtime
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Tai yra „Java“ skirtų „GroupDocs.Signature“ funkcijų apžvalga:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Parašo tipai"
          content: |
            * Teksto parašas
            * Vaizdo parašas
            * Skaitmeniniai parašai
            * QR kodo parašas
            * Brūkšninio kodo parašas
            * Antspaudas Parašas
            * Formos lauko parašas
      
      ## TAB TWO ##
      tab_two:
        description: |
          „Java“ elektroninio pasirašymo API palaiko įvairius toliau išvardytus dokumentų failų formatus. [Palaikomi dokumentų formatai.](https://docs.groupdocs.com/signature/java/supported-document-formats/)

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Other Formats"
              content: |
                * **Vaizdai**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Metafailai**: EMF, WMF, CMX
                * **Nešiojami**: PDF
                * **Keičiama vektorinė grafika**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Kiti**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for Java palaiko šias operacines sistemas, karkasus ir paketų tvarkykles:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operacinės sistemos"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Palaikomi karkasai"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Plėtros aplinkos"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Sukurkite automatizavimo įrankį"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Parašas, skirtas Java funkcijoms"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Kurkite, skaitykite, keiskite, slėpkite ir ištrinkite el. parašus iš palaikomų dokumentų formatų"

      # feature loop
      - icon: "fas fa-eye"
        content: "Prieiga prie pasirašyto dokumento iš srauto, santykinio kelio arba absoliutaus kelio"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Taikyti teksto parašą dokumentams, skaičiuoklėms, pristatymams, vaizdams ir PDF failams"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Pridėkite teksto parašą kaip komentarą, lipduką, vaizdą prie PDF failų, taip pat sukonfigūruokite stilių ir spalvą"

      # feature loop
      - icon: "fas fa-code"
        content: "Pasirašykite PDF dokumentą, vaizdo failą ir gaukite išvestį skirtingu failo formatu"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Skaitmeniniu būdu pasirašykite vaizdus naudodami tekstinį parašą kaip vandens ženklą ir pridėkite skaidrumą, pasukimą prie el. parašo"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Ieškokite sertifikatų ir pasirašykite „Microsoft Word“, „Excel“ ir PDF dokumentus naudodami skaitmeninius sertifikatus"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Pasirašykite teksto apdorojimo dokumentų formatus su vietinio teksto vandens ženklais"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Naudokite QR kodą, brūkšninį kodą norėdami pasirašyti žodį, skaidrę, langelį, PDF ir vaizdo failus"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Konfigūruokite ir pritaikykite antspaudų parašus saugiems palaikomiems failų formatams"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Nustatykite ir priskirkite vaizdo parašus dokumentams, skaičiuoklėms, pristatymams, vaizdams ir PDF failams"

      # feature loop
      - icon: "fas fa-columns"
        content: "Konfigūruokite parašo ypatybes, pvz., išvaizdą ir pojūtį, paraštes, lygiavimą ir kt."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Taikykite skaitmeninį parašą slaptažodžiu apsaugotam dokumentui"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Atlikite PDF dokumentų teksto patikrinimą naudodami parašo tvarkyklę"

      # feature loop
      - icon: "fas fa-print"
        content: "Skaitmeninis Word, Cell, PDF dokumentų tikrinimas naudojant .CER ir .PFX sertifikatų talpyklas"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Nurodykite skirtingus PDF teksto parašų matavimo vienetų tipus (pvz., milimetrus, pikselius ir kt.)"

      # feature loop
      - icon: "fas fa-lock"
        content: "Gaukite dokumento informaciją naudodami failą arba URL – pridėkite formos laukų parašus prie PDF dokumentų"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Pridėkite tinkintą duomenų objektą, įterptąją VCard, el. paštą, EPC, MeCard arba įvykio objektą prie QR kodo"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Skirtingų šepetėlių stilių taikymas parašams, pvz., gradiento, radialinio, vientiso ir tekstūros teptukas"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Pasirašykite dokumentą, esantį FTP arba Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Nustatykite teksto lygiavimą dokumentų, skaidrių, vaizdų ir PDF failų formose"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Ieškokite, patikrinkite ir skaitmeniniu būdu pasirašykite „PowerPoint“ pristatymo dokumentus"

      # feature loop
      - icon: "fas fa-cube"
        content: "Įdėkite parašą naudodami pikselius langelių dokumentuose ir nustatykite teksto padėtį antspaudo parašams"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Įdiekite stačiakampį antspaudą su užapvalintais kampais"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Išplėskite brūkšninio kodo ir QR kodo parašus vaizdo duomenų turiniu"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Pridėkite šifruotus metaduomenų parašus dirbdami su pasirašymo ir paieškos parinktimis"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Įterpkite pasirinktinius objektus į metaduomenų parašus „Word“, „Excel“ ir pristatymuose"

    more_feature:
      # more_feature_loop
      - title: "Lengvai konfigūruokite ir pritaikykite el. parašus"
        content: |
          GroupDocs.Signature for Java API leidžia konfigūruoti ir pridėti el. parašus prie palaikomų dokumentų formatų. Toliau pateikiamas kodo pavyzdys, parodantis, kaip paprasta PDF failui pritaikyti tekstinį parašą:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // nustatyti parašo poziciją
          options.setLeft(100);
          options.setTop(100);
          
          // nustatyti parašo stačiakampį
          options.setWidth(100);
          options.setHeight(30);

          // nustatyti teksto spalvą ir šriftą
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // pasirašyti dokumentą į bylą
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Palaikomi el. parašo brūkšninio kodo kodavimo tipai"
        content: |
          Naudodami GroupDocs.Signature for Java API galite pritaikyti brūkšninio kodo ir QR kodo parašus palaikomiems failų formatams. GroupDocs.Signature for Java palaiko daugybę brūkšninio kodo kodavimo tipų, kad atitiktų daugumą reikalavimų. Palaikomi brūkšninio kodo kodavimo tipai: kodas 11, kodas 128, kodas 16K/32, duomenų juostos kodai, GS1 kodo blokas, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14 ir kodas39. Kodas39 Išplėstas.

          Panašiai GroupDocs.Signature for Java API leidžia naudoti QR kodo tipus, pvz., QR, Aztec ir Data Matrix. Palaikomi QR kodo kodavimo tipai: Aztec, DataMatrix, GS1 DataMatrix ir GS1 QR.

      # more_feature_loop
      - title: "Ieškoti parašų ir sertifikatų"
        content: |
          Naudodami GroupDocs.Signature, skirtą Java API, galite ieškoti QR kodo ir brūkšninio kodo parašų bet kuriame dokumente, pristatyme, skaičiuoklėje, paveikslėlyje, taip pat PDF faile ir gauti paieškos rezultatą. Taip pat galite ieškoti pasirinktinių duomenų objektų iš dokumentų, pasirašytų QR kodo parašu, taip pat ieškoti standartinių VCard ir el. pašto objektų iš dokumentų, pasirašytų QR kodu. Taip pat palaikomas QR kodo parašų užšifruoto teksto tikrinimas ir metaduomenų parašo paieška PDF dokumentuose. Taikykite papildomus paieškos kriterijus Words & Cells dokumentų skaitmeniniams parašams.  

          Paieškos parinktis taip pat pasiekiama „Word“ dokumentų, skaidrių ir skaičiuoklių metaduomenų parašui, o PDF dokumentų paieška formos lauke.

      # more_feature_loop
      - title: "Konfigūruokite el. parašo ypatybes"
        content: |
          Siekiant pagerinti galutinių naudotojų UX, GroupDocs.Signature for Java API suteikia daug ypatybių, kurias galima gana lengvai konfigūruoti. Galite nustatyti šrifto ir spalvų parinktis (fono spalva, priekinio plano spalva, paryškintas, kursyvas, pabrauktas, šriftų šeima, šrifto dydis ir tt), fono ir kraštinės parinktis (fono spalva, fono skaidrumas, kraštinės spalva, kraštinės brūkšnio stilius, kraštinės svoris, Kraštinių skaidrumas ir tt), parašo paraštės (kairė, viršuje, plotis, aukštis, užpildymas ir tt) ir vaizdo parašo srities bei parašo lygiavimo nustatymas (horizontalus lygiavimas, vertikalus lygiavimas ir tt).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature siūlo dokumentų pasirašymo API kitoms populiarioms kūrimo aplinkoms"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---