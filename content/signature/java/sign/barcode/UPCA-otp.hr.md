---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: UPCA
fileformat: Otp
productName: Java
lang: hr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Otp for Java

############################# Head ############################
head_title: "eSign Otp dokument s UPCA crtičnim kodom u Java"
head_description: "Stvorite UPCA potpis crtičnog koda i stavite ga na Otp dokument s Java pomoću nekoliko redaka koda. Koristite GroupDocs Document Signature API za potpisivanje različitih formata datoteka."

############################# Header ############################
title: "Generirajte UPCA potpis crtičnog koda za Otp dokument u Java"
description: "ePotpišite svoje Otp poslovne dokumente pomoću UPCA crtičnog koda. Brzo i jednostavno generirajte potpis crtičnog koda s nekoliko redaka koda za postavljanje opcija potpisivanja."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "O API-ju za potpise crtičnog koda GroupDocs.Signature for Java."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) je brz i jednostavan API za upravljanje e-potpisivanjem digitalnih dokumenata pomoću vrsta crtičnog koda kao što su UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 i mnogi drugi. Kupci mogu jednostavno kreirati crtične kodove sa potrebnim tekstom i staviti ih u PDF, Microsoft Office Words dokumente, Microsoft Office Excel radne knjige, MS PowerPoint prezentacije, Adobe Photoshop datoteke i razne formate slika. Crtični kodovi postavljeni u dokumente mogu se ažurirati, pretraživati, verificirati, brisati ili pregledavati. Štoviše, podržana je prilagodba crtičnih kodova.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Koraci za potpisivanje Otp s Barcode u Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) pruža mogućnost brzog i jednostavnog potpisivanja Otp dokumenata s Barcode potpisima.
        
        * Stvorite instancu klase potpisa koja daje Otp datoteku koja bi se trebala potpisati kao put ili memorijski tok
        * Instancirajte klasu SignOptions i postavite sve tražene podatke.
        * Pozovite metodu Signature.Sign() prosljeđujući izlaznu datoteku Otp ili memorijski tok

    title_right: " Zahtjevi sustava"
    content_right: |
        GroupDocs.Signature for Java podržani su na svim glavnim platformama i operativnim sustavima. Prije izvršavanja koda u nastavku, provjerite imate li sljedeće preduvjete instalirane na vašem sustavu.

        * Operativni sustavi: Microsoft Windows, Linux, MacOS
        * Razvojna okruženja: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Preuzmite najnoviji GroupDocs.Signature for Java od [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Otp file
        String filePath = "input.otp";
        // Set up output file
        String outputFilePath = "output.otp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.UPCA);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Otp document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Potpisivanje Otp dokumenata s Barcode Live Demo"
    content: |
       Potpišite datoteku Otp raznim potpisima upravo sada tako da posjetite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web mjesto. Besplatan online demo čeka na vas.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About UPCA Barcode"
          content: |
            Univerzalni kod proizvoda simbol je crtičnog koda koji se širom svijeta široko koristi za praćenje trgovačkih jedinica u trgovinama.
          characterset: |
             Brojčane znamenke (0-9).
          textcapacity: |
             Točno 11 znamenki + 1 kontrolna znamenka.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAGwAAABjCAYAAAB+MOUYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAARpSURBVHhe7ZFBimBRCMT6/pfuUYaAi6pe58MLSJCAG39+H5/iPexjvId9jPewj/Ee9jHewz7Ge9jH+PNhPz//M4bdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXh5K3sM+xnvYx3gP+xjvYR/jPexT/P7+A4FOQDtpBhIBAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Drugi podržani potpisi Barcode za Java"
    content: |
        "Također možete potpisati Otp drugim vrstama potpisa. Pogledajte popis u nastavku."
    format: 
        
       
back_to_top:
    enable: true
---