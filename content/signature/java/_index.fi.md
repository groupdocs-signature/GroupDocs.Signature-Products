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
head_title: "Java Digital Signature API, lisää eAllekirjoitus PDF Word Excel -kuvaan"
head_description: "Java digitaalisen allekirjoituksen API. Sähköinen allekirjoituskirjasto PDF-, Microsoft Word-, Excel-laskentataulukoiden, PowerPoint-esitysten ja kuvadokumenttimuotojen digitaaliseen allekirjoittamiseen."

############################# Header ############################
title: "Java-sovellusliittymä digitaalisten allekirjoitusten hallintaan"
description: "Hallitse kuvien sähköistä allekirjoitusta, QR-koodia, viivakoodia, metatietoja, teksti- ja leimatyyppejä Java-sovelluksissa kuvien ja digitaalisten asiakirjatiedostomuotojen allekirjoittamista varten."
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
              text: "Yleiskatsaus"

            # button loop
            - link: "#features"
              text: "ominaisuudet"

            # button loop
            - link: "#support"
              text: "Tuki"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Live-demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Hinnoittelu"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API auttaa sinua kehittämään Java-sovelluksia, joissa on sähköinen allekirjoitustoiminto tuettujen muotojen digitaalisten asiakirjojen allekirjoittamiseen ilman ulkoisten ohjelmistojen asentamista. Se tukee erityyppisten sähköisten allekirjoitusten, kuten kuvan, viivakoodin, QR-koodin, leiman, tekstin, optisten ja metatietojen, käsittelyä ja hallintaa. Kaikki sähköiset yritysasiakirjasi, kuten Microsoft Office Word, PowerPoint-esitykset, Excel-laskentataulukot, kuvat ja PDF-tiedostot, voidaan allekirjoittaa digitaalisesti mukauttamalla allekirjoitusominaisuuksia esim. varjo, mitat, kohdistus ja paljon muuta tarpeidesi mukaan. Digitaalinen allekirjoituskirjasto on yksinkertainen ja kevyt, ja se koostuu yhdestä DLL-tiedostosta, joka voidaan integroida helposti uuteen tai olemassa olevaan Java-sovellukseen.  

      GroupDocs.Signature for Java API:n kautta voit ladata kaikki rekisteröidyt varmenteet järjestelmästä tai paikantaa olemassa olevat allekirjoitukset yksinkertaisen ja tarkennetun haun avulla. Mahdollisuudet työskennellä salasanalla suojattujen asiakirjojen kanssa, määrittämällä yleiset allekirjoitusominaisuudet (tekstin koko, peittävyys, kierto, vahvistus, fontin ominaisuudet, värivaihtoehdot, sivunumero, leveys, yläreuna, vasen jne.) ja tuki erilaisten eAllekirjoitustyyppien käyttöönotolle tekevät siitä luotettavan Sähköisten allekirjoitusten hallintaratkaisu digitaalisille asiakirjoille.  

      GroupDocs.Signature for Java on yhteensopiva kaikkien Java-versioiden kanssa ja tukee suosittuja käyttöjärjestelmiä (Windows, Linux, MacOS), jotka pystyvät ajamaan Java-ajonaikaa
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Tämä on yleiskatsaus Java:n GroupDocs.Signature-ominaisuuksiin:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Allekirjoitustyypit"
          content: |
            * Teksti allekirjoitus
            * Kuvan allekirjoitus
            * Digitaaliset allekirjoitukset
            * QR-koodin allekirjoitus
            * Viivakoodin allekirjoitus
            * Leima Allekirjoitus
            * Lomakekentän allekirjoitus
      
      ## TAB TWO ##
      tab_two:
        description: |
          Java sähköisen allekirjoituksen API tukee useita alla lueteltuja asiakirjatiedostomuotoja. [Tuetut asiakirjamuodot.](https://docs.groupdocs.com/signature/java/supported-document-formats/)

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
                * **Kuvat**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Metatiedostot**: EMF, WMF, CMX
                * **Kannettava**: PDF
                * **Skaalautuva vektorigrafiikka**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **muut**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for Java tukee seuraavia käyttöjärjestelmiä, kehyksiä ja paketinhallintaohjelmia:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Käyttöjärjestelmät"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Tuetut puitteet"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Kehitysympäristöt"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Rakenna automaatiotyökalu"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature Java-ominaisuuksille"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Luo, lue, muokkaa, piilota ja poista sähköisiä allekirjoituksia tuetuista asiakirjamuodoista"

      # feature loop
      - icon: "fas fa-eye"
        content: "Pääsy allekirjoitettuun asiakirjaan virrasta, suhteellisesta polusta tai absoluuttisesta polusta"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Käytä tekstiallekirjoitusta asiakirjoihin, laskentataulukoihin, esityksiin, kuviin ja PDF-tiedostoihin"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Lisää tekstiallekirjoitus huomautukseksi, tarraksi, kuvaksi PDF-tiedostoihin ja määritä myös tyyli ja väri"

      # feature loop
      - icon: "fas fa-code"
        content: "Allekirjoita PDF-dokumentti, kuvatiedosto ja hanki tuloste eri tiedostomuodoissa"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Allekirjoita digitaalisesti kuvat tekstiallekirjoituksella vesileimana ja lisää läpinäkyvyyttä, kiertoa sähköiseen allekirjoitukseen"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Hae sertifikaatteja ja allekirjoita Microsoft Word-, Excel- ja PDF-asiakirjoja digitaalisilla varmenteilla"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Merkitse tekstinkäsittely-asiakirjamuodot alkuperäistekstin vesileimoilla"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Käytä QR-koodia, viivakoodia allekirjoittaaksesi Word-, dioja, soluja, PDF- ja kuvatiedostoja"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Määritä ja käytä leima-allekirjoituksia suojatuissa tuetuissa tiedostomuodoissa"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Määritä ja määritä kuvaallekirjoituksia asiakirjoille, laskentataulukoille, esityksille, kuville ja PDF-tiedostoille"

      # feature loop
      - icon: "fas fa-columns"
        content: "Määritä allekirjoitusominaisuudet, kuten ulkoasu, marginaalit, kohdistus jne."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Käytä digitaalista allekirjoitusta salasanalla suojatussa asiakirjassa"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Suorita PDF-dokumenttien tekstin tarkistus allekirjoitusten käsittelijällä"

      # feature loop
      - icon: "fas fa-print"
        content: "Word-, solu- ja PDF-asiakirjojen digitaalinen todentaminen .CER- ja .PFX-sertifikaattisäiliöillä"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Määritä eri mittayksikkötyypit (esim. millimetrit, pikselit jne.) PDF-tekstiallekirjoituksille"

      # feature loop
      - icon: "fas fa-lock"
        content: "Hanki asiakirjan tiedot tiedoston tai URL-osoitteen kautta - Lisää lomakekentän allekirjoituksia PDF-dokumentteihin"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Lisää mukautettu tietoobjekti, upotettu VCard, sähköposti, EPC, MeCard tai tapahtumaobjekti QR-koodiin"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Käytä eri siveltimen tyylejä allekirjoituksiin, esim. liukuväri-, säteittäis-, kiinteä- ja pintakuviosivellin"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Allekirjoita asiakirja, joka sijaitsee FTP:ssä tai Azure Cloud Storagessa"

      # feature loop
      - icon: "fas fa-heading"
        content: "Aseta tekstin tasaus muodoissa asiakirjoille, dioille, kuville ja PDF-tiedostoille"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Etsi, vahvista ja allekirjoita digitaalisesti PowerPoint-esitysasiakirjoja"

      # feature loop
      - icon: "fas fa-cube"
        content: "Aseta allekirjoitus käyttämällä pikseleitä soluasiakirjoihin ja tekstin sijoittelu leimaallekirjoituksia varten"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Toteuta suorakaideleimaallekirjoitus pyöristetyillä kulmilla"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Laajenna viivakoodi- ja QR-koodiallekirjoituksia kuvatietosisällöllä"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Lisää salattuja metatietojen allekirjoituksia samalla kun työskentelet allekirjoitus- ja hakuvaihtoehtojen kanssa"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Upota mukautettuja objekteja Wordin, Excelin ja esitysten metatieto-allekirjoituksiin"

    more_feature:
      # more_feature_loop
      - title: "Määritä ja käytä sähköisiä allekirjoituksia helposti"
        content: |
          GroupDocs.Signature for Java API mahdollistaa sähköisten allekirjoitusten määrittämisen ja lisäämisen tuettuihin asiakirjamuotoihin. Seuraavassa on koodiesimerkki, joka osoittaa, kuinka helppoa on lisätä tekstiallekirjoitus PDF-tiedostoon:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // aseta allekirjoituspaikka
          options.setLeft(100);
          options.setTop(100);
          
          // aseta allekirjoitussuorakulmio
          options.setWidth(100);
          options.setHeight(30);

          // aseta tekstin väri ja fontti
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // allekirjoittaa asiakirja tiedostoon
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Tuetut viivakoodien koodaustyypit sähköiselle allekirjoitukselle"
        content: |
          GroupDocs.Signature for Java API:n avulla voit käyttää viivakoodi- ja QR-koodiallekirjoituksia tuetuissa tiedostomuodoissa. GroupDocs.Signature for Java tukee valtavaa valikoimaa viivakoodien koodaustyyppejä, jotka täyttävät useimmat vaatimukset. Tuetut viivakoodin koodaustyypit ovat: Code 11, Code 128, Code 16K/32, Databar codes, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard, Code39 Code39 laajennettu.

          Samoin GroupDocs.Signature for Java API antaa sinun käyttää QR-koodityyppejä, kuten QR, Aztec ja Data Matrix. Tuetut QR-koodin koodaustyypit ovat Aztec, DataMatrix, GS1 DataMatrix ja GS1 QR.

      # more_feature_loop
      - title: "Hae allekirjoituksia ja sertifikaatteja"
        content: |
          GroupDocs.Signature for Java API:n avulla voit etsiä QR-koodi- ja viivakoodiallekirjoituksia mistä tahansa dokumentista, esityksestä, laskentataulukosta, kuvasta sekä PDF-tiedostosta ja hakea hakutuloksen. Voit myös etsiä mukautettuja tietoobjekteja QR-koodiallekirjoituksella allekirjoitetuista asiakirjoista sekä etsiä standardista VCard- ja sähköpostiobjektia QR-koodilla allekirjoitetuista asiakirjoista. Tuetaan myös QR-koodiallekirjoitusten salatun tekstin tarkistamista sekä metadata-allekirjoituksen etsimistä PDF-dokumenteista. Käytä lisähakuehtoja Words & Cells -dokumenttien digitaalisille allekirjoituksille.  

          Hakuvaihtoehto on saatavilla myös Word-dokumenttien, diojen ja laskentataulukoiden metatietoallekirjoitukselle, kun taas lomakekenttähaku on käytettävissä PDF-dokumenteille.

      # more_feature_loop
      - title: "Määritä sähköisen allekirjoituksen ominaisuudet"
        content: |
          Parantaakseen loppukäyttäjien käyttökokemusta GroupDocs.Signature for Java API tarjoaa monia ominaisuuksia, jotka voidaan määrittää melko helposti. Voit määrittää fontti- ja väriasetukset (taustaväri, etualan väri, lihavoitu, kursivoitu, alleviivaus, kirjasinperhe, kirjasinkoko jne.), tausta- ja reunusasetukset (taustaväri, taustan läpinäkyvyys, reunuksen väri, reunaviivatyyli, reunuksen paino, Reunuksen läpinäkyvyys jne.), Allekirjoitusmarginaalit (vasen, Ylä, Leveys, Korkeus, Padding jne.) ja Määritä kuvan allekirjoitusalue ja allekirjoituksen kohdistus (vaakasuuntainen kohdistus, pystysuuntainen kohdistus jne.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature tarjoaa dokumenttien allekirjoitussovellusliittymiä muihin suosittuihin kehitysympäristöihin"

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