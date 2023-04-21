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
head_title: "Java Digital Signature API, dodajte e-potpis u PDF Word Excel sliku"
head_description: "Java digitalni potpis API. Knjižnica elektroničkih potpisa za digitalno potpisivanje PDF-a, Microsoft Worda, Excel proračunskih tablica, PowerPoint prezentacija i formata slikovnih dokumenata."

############################# Header ############################
title: "Java API za upravljanje digitalnim potpisima"
description: "Upravljajte e-potpisom slika, QR-koda, crtičnog koda, metapodataka, teksta i vrsta pečata u Java aplikacijama za potpisivanje slika i formata datoteka digitalnih dokumenata."
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
              text: "Značajke"

            # button loop
            - link: "#support"
              text: "podrška"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Demo uživo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Cijene"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API pomaže vam u razvoju Java aplikacija s funkcionalnošću elektroničkih potpisa za potpisivanje digitalnih dokumenata podržanih formata bez instaliranja vanjskog softvera. Podržava manipulaciju i upravljanje različitim vrstama e-potpisa kao što su slika, crtični kod, QR-kod, pečat, tekst, optički i metapodaci. Svi vaši elektronički poslovni dokumenti poput Microsoft Office Worda, PowerPoint prezentacija, Excel proračunskih tablica, slika i PDF datoteka mogu se digitalno potpisati prilagođavanjem svojstava potpisa, npr. sjena, dimenzije, poravnanje i više prema vašim zahtjevima. Knjižnica digitalnog potpisa jednostavna je i lagana, sastoji se od jedne DLL datoteke koja se može lako integrirati unutar nove ili postojeće Java aplikacije.  

      Preko GroupDocs.Signature for Java API možete učitati sve registrirane certifikate iz sustava ili locirati postojeće potpise koristeći jednostavno i napredno pretraživanje. Mogućnosti za rad s dokumentima zaštićenim lozinkom, određivanje uobičajenih svojstava potpisa (veličina teksta, neprozirnost, rotacija, provjera, svojstva fonta, opcije boja, broj stranice, širina, vrh, lijevo itd.) i podrška za implementaciju različitih vrsta e-potpisa čine ga pouzdanim Rješenje za upravljanje e-potpisima za digitalne dokumente.  

      GroupDocs.Signature za Javu kompatibilan je sa svim verzijama Jave i podržava popularne operativne sustave (Windows, Linux, MacOS) koji mogu pokretati Java runtime
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Ovo je pregled značajki GroupDocs.Signature za Javu:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Vrste potpisa"
          content: |
            * Potpis teksta
            * Potpis slike
            * Digitalni potpisi
            * Potpis QR koda
            * Potpis crtičnog koda
            * Pečat Potpis
            * Potpis polja obrasca
      
      ## TAB TWO ##
      tab_two:
        description: |
          API za elektroničko potpisivanje Java podržava različite formate datoteka dokumenata kako je navedeno u nastavku. [Podržani formati dokumenata.](https://docs.groupdocs.com/signature/java/supported-document-formats/)

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
                * **Prijenosni**: PDF
                * **Skalabilna vektorska grafika**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Drugi**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature za Javu podržava sljedeće operativne sustave, okvire i upravitelje paketa:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operacijski sustavi"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Podržani okviri"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Razvojna okruženja"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Alat za automatizaciju izrade"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature za Java značajke"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Stvaranje, čitanje, mijenjanje, skrivanje i brisanje e-potpisa iz podržanih formata dokumenata"

      # feature loop
      - icon: "fas fa-eye"
        content: "Pristup dokumentu koji treba potpisati iz streama, relativnog puta ili apsolutnog puta"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Primijenite tekstualni potpis na dokumente, proračunske tablice, prezentacije, slike i PDF datoteke"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Dodajte tekstualni potpis kao komentar, naljepnicu, sliku u PDF datoteke i konfigurirajte stil i boju"

      # feature loop
      - icon: "fas fa-code"
        content: "Potpišite PDF dokument, slikovnu datoteku i dobijte izlaz u različitim formatima datoteka"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Digitalno potpišite slike tekstualnim potpisom kao vodenim žigom i dodajte prozirnost, rotaciju u e-potpis"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Pretražujte certifikate i potpisujte Microsoft Word, Excel i PDF dokumente digitalnim certifikatima"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Potpišite formate dokumenata za obradu teksta izvornim tekstualnim vodenim žigovima"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Koristite QR-kod, crtični kod za potpisivanje riječi, slajdova, ćelija, PDF i slikovnih datoteka"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Konfigurirajte i primijenite pečatne potpise kako biste osigurali podržane formate datoteka"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Postavite i dodijelite slikovne potpise dokumentima, proračunskim tablicama, prezentacijama, slikama i PDF datotekama"

      # feature loop
      - icon: "fas fa-columns"
        content: "Konfigurirajte svojstva potpisa, npr. izgled i dojam, margine, poravnanje itd."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Primjena digitalnog potpisa na dokument zaštićen lozinkom"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Izvršite provjeru teksta PDF dokumenata pomoću Rukovatelja potpisom"

      # feature loop
      - icon: "fas fa-print"
        content: "Digitalna provjera Word, Cell, PDF dokumenata s .CER i .PFX spremnicima certifikata"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Odredite različite vrste mjernih jedinica (npr. milimetri, pikseli itd.) za PDF tekstualne potpise"

      # feature loop
      - icon: "fas fa-lock"
        content: "Dobivanje informacija o dokumentu putem datoteke ili URL-a - Dodajte potpise polja obrasca u PDF dokumente"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Dodajte objekt prilagođenih podataka, ugrađenu VCard, e-poštu, EPC, MeCard ili objekt događaja u QR kod"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Primijenite različite stilove kista na potpise, npr. gradijent, radijalni, čvrsti i teksturni kist"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Potpišite dokument koji se nalazi na FTP ili Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Postavite poravnanje teksta unutar oblika za dokumente, slajdove, slike i PDF datoteke"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Pretraživanje, provjera i digitalni potpis PowerPoint prezentacijskih dokumenata"

      # feature loop
      - icon: "fas fa-cube"
        content: "Postavite potpis koristeći piksele u ćelijskim dokumentima i pozicioniranje teksta za potpise pečata"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Implementirajte potpis pravokutnog pečata sa zaobljenim kutovima"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Proširite potpise crtičnog koda i QR koda sadržajem slikovnih podataka"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Dodajte šifrirane potpise metapodataka dok radite s opcijama potpisivanja i pretraživanja"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Ugradite prilagođene objekte u potpise metapodataka unutar programa Word, Excel i prezentacija"

    more_feature:
      # more_feature_loop
      - title: "Jednostavno konfigurirajte i primijenite e-potpise"
        content: |
          GroupDocs.Signature for Java API omogućuje konfiguriranje i dodavanje e-potpisa podržanim formatima dokumenata. Slijedi primjer koda koji pokazuje koliko je jednostavno primijeniti tekstualni potpis na PDF datoteku:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // postavite poziciju potpisa
          options.setLeft(100);
          options.setTop(100);
          
          // postavite pravokutnik potpisa
          options.setWidth(100);
          options.setHeight(30);

          // postavite boju teksta i font
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // potpisati dokument u datoteku
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Podržane vrste kodiranja crtičnog koda za e-potpis"
        content: |
          Pomoću API-ja GroupDocs.Signature za Java možete primijeniti potpise crtičnog koda i QR koda na podržane formate datoteka. GroupDocs.Signature za Javu podržava veliki raspon vrsta kodiranja crtičnog koda kako bi zadovoljio većinu zahtjeva. Podržane vrste kodiranja crtičnog koda uključuju Code 11, Code 128, Code 16K/32, Databar kodove, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard i Code39 Prošireno.

          Slično GroupDocs.Signature za Java API omogućuje vam korištenje vrsta QR kodova, kao što su QR, Aztec i Data Matrix. Podržane vrste kodiranja QR-koda uključuju Aztec, DataMatrix, GS1 DataMatrix i GS1 QR.

      # more_feature_loop
      - title: "Pretražite potpise i potvrde"
        content: |
          Putem API-ja GroupDocs.Signature za Java možete pretraživati ​​potpise QR-kodova i crtičnih kodova u bilo kojem dokumentu, prezentaciji, proračunskoj tablici, slici, kao i PDF datoteci, te dohvatiti rezultate pretraživanja. Također možete pretraživati ​​prilagođeni podatkovni objekt iz dokumenata potpisanih potpisom QR-koda kao i pretraživati ​​standardnu ​​VCard i objekt e-pošte iz dokumenata potpisanih QR-kodom. Također je podržana provjera šifriranog teksta QR-Code potpisa kao i traženje potpisa metapodataka u PDF dokumentima. Primijenite dodatne kriterije pretraživanja za digitalne potpise Words & Cells dokumenata.  

          Opcija pretraživanja dostupna je i za potpis metapodataka za Word dokumente, slajdove i proračunske tablice, dok je pretraživanje polja obrasca dostupno za PDF dokumente.

      # more_feature_loop
      - title: "Konfigurirajte svojstva e-potpisa"
        content: |
          Kako bi se poboljšao korisnički doživljaj krajnjih korisnika GroupDocs.Signature za Java API pruža mnogo svojstava koja se mogu konfigurirati prilično jednostavno. Možete postaviti opcije fonta i boje (boja pozadine, boja prednjeg plana, podebljano, kurziv, podcrtano, obitelj fontova, veličina fonta itd.), opcije pozadine i obruba (boja pozadine, prozirnost pozadine, boja obruba, stil obrubne crtice, debljina obruba, Prozirnost obruba itd.), margine potpisa (lijevo, vrh, širina, visina, ispuna itd.) i postavljanje područja potpisa slike i poravnanja potpisa (horizontalno poravnanje, okomito poravnanje itd.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature nudi API-je za potpisivanje dokumenata za druga popularna razvojna okruženja"

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