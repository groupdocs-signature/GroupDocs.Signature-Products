---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Zip
productName: Java
lang: hr
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Zip with Java

############################# Head ############################
head_title: "Potražite Digital potpise u datoteci Zip u Java"
head_description: "Upotrijebite Java za traženje potpisa Digital u datotekama Zip pomoću nekoliko redaka koda."

############################# Header ############################
title: "Potražite Digital potpise u Zip datoteci"
description: "Izvorni API za Java omogućuje pretraživanje potpisa Digital u već potpisanim Zip datotekama. Izvršite napredno pretraživanje e-potpisa unutar svojih Zip dokumenata pomoću nekoliko redaka koda."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "O GroupDocs.Signature for Java API-ju"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) pruža Java API za obradu dokumenata koji koriste različite vrste potpisa kao što su tekstovi, slike, digitalni certifikati, crtični kodovi, QR kodovi, pečati ili metapodaci. Korisnici mogu dodavati, brisati, ažurirati, verificirati ili pretraživati ​​elektroničke potpise unutar PDF-ova, MS Word dokumenata, MS Excel radnih knjiga, MS PowerPoint prezentacija, Adobe Photoshop datoteka i raznih formata slika, uz dodatnu podršku za prilagođavanje svojstava potpisa prema potrebi.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kako tražiti Digital potpise u Zip"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) programerima proizvoda Java olakšava traženje potpisa Digital u datotekama Zip iz njihovih aplikacija implementacijom nekoliko jednostavnih koraka.
        
        * Stvorite novu instancu klase Signature i proslijedite putanju izvornog dokumenta kao parametar konstruktora.
        * Instancirajte SearchOptions objekt prema svojim zahtjevima i odredite opcije pretraživanja.
        * Pozovite metodu Search instance klase Signature i proslijedite joj SearchOptions.
        * Obradite rezultate pretraživanja u skladu s vašim zahtjevima.

    title_right: "Zahtjevi sustava"
    content_right: |
        GroupDocs.Signature for Java podržani su na svim glavnim platformama i operativnim sustavima. Prije izvršavanja koda u nastavku, provjerite imate li sljedeće preduvjete instalirane na vašem sustavu.

        * Operativni sustavi: Microsoft Windows, Linux, MacOS
        * Razvojna okruženja: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Preuzmite najnoviju verziju GroupDocs.Signature for Java s [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Zip file
        String filePath = "input.zip";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        DigitalSearchOptions options = new DigitalSearchOptions();

        // specify special search criteria
        options.setComments("Approved");
        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2021, 3, 5));
        options.setSignDateTimeTo(new Date(2022, 7, 16));
        
        // search for Digital signatures in Zip document
        List<DigitalSignature> signatures = signature.search(DigitalSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Potražite Digital elektroničke potpise Demo uživo"
    content: |
       Potražite u dokumentu različite elektroničke potpise za Zip datoteke upravo sada tako da posjetite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web mjesto.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Potražite druge Digital potpise koristeći Java"
    content: |
        "Pretraživanje elektroničkih potpisa u raznim dokumentima. Pronađite potpise jednog od popularnih formata datoteka kao što je prikazano u nastavku."
    format: 
           
       
back_to_top:
    enable: true
---