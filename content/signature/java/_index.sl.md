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
head_title: "API za digitalni podpis Java, dodajte e-podpis v sliko PDF Word Excel"
head_description: "API za digitalni podpis Java. Knjižnica elektronskih podpisov za digitalno podpisovanje PDF, Microsoft Word, Excel preglednic, PowerPoint predstavitev in formatov slikovnih dokumentov."

############################# Header ############################
title: "Java API za upravljanje digitalnih podpisov"
description: "Upravljajte e-podpis slike, QR-kode, črtne kode, metapodatkov, besedila in vrst žigov v aplikacijah Java za podpisovanje slik in formatov datotek digitalnih dokumentov."
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
              text: "Pregled"

            # button loop
            - link: "#features"
              text: "Lastnosti"

            # button loop
            - link: "#support"
              text: "Podpora"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Demo v živo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Cenitev"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API vam pomaga razviti aplikacije Java s funkcijo elektronskih podpisov za podpisovanje digitalnih dokumentov podprtih formatov brez namestitve zunanje programske opreme. Podpira manipulacijo in upravljanje različnih vrst e-podpisov, kot so slika, črtna koda, QR-koda, žig, besedilo, optični in metapodatki. Vse vaše elektronske poslovne dokumente, kot so Microsoft Office Word, PowerPoint predstavitve, Excelove preglednice, slike in datoteke PDF, je mogoče digitalno podpisati s prilagoditvijo lastnosti podpisa, npr. senco, dimenzije, poravnavo in več glede na vaše zahteve. Knjižnica digitalnega podpisa je preprosta in lahka, sestavljena iz ene same datoteke DLL, ki jo je mogoče preprosto integrirati v novo ali obstoječo aplikacijo Java.  

      Preko GroupDocs.Signature for Java API lahko naložite vsa registrirana potrdila iz sistema ali poiščete obstoječe podpise s preprostim in naprednim iskanjem. Možnosti za delo z dokumenti, zaščitenimi z geslom, določanje običajnih lastnosti podpisa (velikost besedila, motnost, rotacija, preverjanje, lastnosti pisave, barvne možnosti, številka strani, širina, zgoraj, levo itd.) in podpora za izvajanje različnih vrst e-podpisov, zaradi česar je zanesljiv Rešitev za upravljanje e-podpisov za digitalne dokumente.  

      GroupDocs.Signature for Java je združljiv z vsemi različicami Jave in podpira priljubljene operacijske sisteme (Windows, Linux, MacOS), ki lahko izvajajo Java runtime
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          To je pregled funkcij GroupDocs.Signature za Javo:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Vrste podpisov"
          content: |
            * Besedilni podpis
            * Podpis slike
            * Digitalni podpisi
            * Podpis kode QR
            * Podpis črtne kode
            * Žig Podpis
            * Podpis polja obrazca
      
      ## TAB TWO ##
      tab_two:
        description: |
          API za elektronsko podpisovanje Java podpira različne formate datotek dokumentov, kot je navedeno spodaj. [Podprti formati dokumentov.](https://docs.groupdocs.com/signature/java/supported-document-formats/)

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
                * **Slike**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Metadatoteke**: EMF, WMF, CMX
                * **Prenosni**: PDF
                * **Razširljiva vektorska grafika**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **drugi**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for Java podpira naslednje operacijske sisteme, ogrodja in upravitelje paketov:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operacijski sistemi"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Podprta ogrodja"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Razvojna okolja"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Orodje za avtomatizacijo gradnje"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature for Java Features"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Ustvarjanje, branje, spreminjanje, skrivanje in brisanje e-podpisov iz podprtih formatov dokumentov"

      # feature loop
      - icon: "fas fa-eye"
        content: "Dostop do podpisanega dokumenta iz toka, relativne poti ali absolutne poti"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Uporabite besedilni podpis za dokumente, preglednice, predstavitve, slike in datoteke PDF"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Dodajte besedilni podpis kot opombo, nalepko, sliko v datoteke PDF, konfigurirajte tudi slog in barvo"

      # feature loop
      - icon: "fas fa-code"
        content: "Podpišite dokument PDF, slikovno datoteko in pridobite izpis v drugačni obliki zapisa datoteke"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Digitalno podpišite slike z besedilnim podpisom kot vodnim žigom in dodajte prosojnost, rotacijo v e-podpis"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Iščite po potrdilih in podpisujte dokumente Microsoft Word, Excel in PDF z digitalnimi potrdili"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Formate dokumentov za obdelavo besedila podpišite z izvornimi besedilnimi vodnimi žigi"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Uporabite QR-kodo, črtno kodo za podpis besed, diapozitivov, celic, PDF in slikovnih datotek"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Konfigurirajte in uporabite podpise žigov za zaščito podprtih formatov datotek"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Nastavite in dodelite slikovne podpise dokumentom, preglednicam, predstavitvam, slikam in datotekam PDF"

      # feature loop
      - icon: "fas fa-columns"
        content: "Konfigurirajte lastnosti podpisa, npr. videz in občutek, robove, poravnavo itd."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Uporaba digitalnega podpisa za dokument, zaščiten z geslom"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Izvedite preverjanje besedila dokumentov PDF z uporabo orodja za obravnavo podpisov"

      # feature loop
      - icon: "fas fa-print"
        content: "Digitalno preverjanje dokumentov Word, Cell, PDF z vsebniki potrdil .CER in .PFX"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Določite različne vrste merskih enot (npr. milimetre, slikovne pike itd.) za besedilne podpise PDF"

      # feature loop
      - icon: "fas fa-lock"
        content: "Pridobite informacije o dokumentu prek datoteke ali URL-ja - dodajte podpise polj obrazca v dokumente PDF"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Dodajte predmet podatkov po meri, vdelano kartico VCard, e-pošto, EPC, MeCard ali predmet dogodka v kodo QR"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Uporabite različne sloge čopičev za podpise, npr. Gradient, Radial, Solid in Texture Brush"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Podpišite dokument, ki se nahaja na FTP ali Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Nastavite poravnavo besedila znotraj oblik za dokumente, diapozitive, slike in datoteke PDF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Iskanje, preverjanje in digitalno podpisovanje PowerPoint predstavitvenih dokumentov"

      # feature loop
      - icon: "fas fa-cube"
        content: "Postavite podpis z uporabo slikovnih pik v celičnih dokumentih in pozicioniranje besedila za podpise z žigi"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Implementirajte podpis pravokotnega žiga z zaobljenimi vogali"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Razširite podpise črtne kode in kode QR z vsebino slikovnih podatkov"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Med delom z možnostmi podpisovanja in iskanja dodajte podpise šifriranih metapodatkov"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Vdelajte predmete po meri v podpise metapodatkov v Wordu, Excelu in predstavitvah"

    more_feature:
      # more_feature_loop
      - title: "Preprosto konfigurirajte in uporabite e-podpise"
        content: |
          GroupDocs.Signature for Java API omogoča konfiguracijo in dodajanje e-podpisov podprtim formatom dokumentov. Sledi primer kode, ki prikazuje, kako preprosto je uporabiti besedilni podpis v datoteki PDF:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // nastavite položaj podpisa
          options.setLeft(100);
          options.setTop(100);
          
          // nastavite podpisni pravokotnik
          options.setWidth(100);
          options.setHeight(30);

          // nastavite barvo besedila in pisavo
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // podpišite dokument v datoteko
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Podprte vrste kodiranja črtne kode za e-podpis"
        content: |
          Z API-jem GroupDocs.Signature for Java lahko uporabite podpise črtne kode in kode QR za podprte formate datotek. GroupDocs.Signature za Javo podpira ogromno vrst kodiranja črtne kode, da zadosti večini zahtev. Podprte vrste kodiranja črtne kode vključujejo Code 11, Code 128, Code 16K/32, Databar kode, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard in Code39 Razširjeno.

          Podobno API GroupDocs.Signature for Java omogoča uporabo vrst kod QR, kot so QR, Aztec in Data Matrix. Podprte vrste kodiranja QR-Code vključujejo Aztec, DataMatrix, GS1 DataMatrix in GS1 QR.

      # more_feature_loop
      - title: "Iskanje podpisov in potrdil"
        content: |
          Prek API-ja GroupDocs.Signature for Java lahko iščete podpise kode QR in črtne kode v katerem koli dokumentu, predstavitvi, preglednici, sliki in datoteki PDF ter pridobite rezultate iskanja. Iščete lahko tudi podatkovne objekte po meri iz dokumentov, podpisanih s podpisom QR-Code, ter poiščete standardno VCard in e-poštni objekt iz dokumentov, podpisanih s QR-Code. Podprto je tudi preverjanje šifriranega besedila podpisov QR-Code in iskanje podpisa metapodatkov v dokumentih PDF. Uporabite dodatne iskalne kriterije za digitalne podpise dokumentov Words & Cells.  

          Možnost iskanja je na voljo tudi za podpis metapodatkov za dokumente Word, diapozitive in preglednice, medtem ko je iskanje po polju obrazca na voljo za dokumente PDF.

      # more_feature_loop
      - title: "Konfigurirajte lastnosti e-podpisa"
        content: |
          Za izboljšanje UX končnih uporabnikov GroupDocs.Signature for Java API ponuja veliko lastnosti, ki jih je mogoče konfigurirati precej enostavno. Nastavite lahko možnosti pisave in barve (barva ozadja, barva ospredja, krepko, ležeče, podčrtano, družina pisav, velikost pisave itd.), možnosti ozadja in obrobe (barva ozadja, prosojnost ozadja, barva obrobe, slog obrobne pomišljaja, debelina obrobe, Preglednost obrob itd.), robovi podpisa (levo, zgoraj, širina, višina, oblazinjenje itd.) in nastavitev območja podpisa slike in poravnave podpisa (vodoravna poravnava, navpična poravnava itd.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature ponuja API-je za podpisovanje dokumentov za druga priljubljena razvojna okolja"

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