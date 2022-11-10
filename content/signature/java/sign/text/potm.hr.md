---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Potm
productName: Java
lang: hr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Potm for Java

############################# Head ############################
head_title: "Stvorite tekstualne elektroničke potpise u datoteku Potm s Java"
head_description: "Stavite e-potpis Text na datoteku Potm za Java pomoću nekoliko redaka koda. Koristite GroupDocs Document Signature API za potpisivanje desetaka formata datoteka."

############################# Header ############################
title: "Potpišite Potm datoteke s Text potpisima u Java"
description: "Kako dodati Text potpis s nekoliko redaka Java koda"
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
    title: "O GroupDocs.Signature for Java API-ju"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) je popularan API za e-potpisivanje digitalnih dokumenata. Dostupni su potpisi kao što su tekstovi, slike, digitalni certifikati, crtični kodovi, QR kodovi, pečati ili metapodaci. Potpisi se mogu staviti na PDF-ove, MS Word dokumente, MS Excel radne knjige, MS PowerPoint prezentacije, Adobe Photoshop datoteke i razne formate slika. Korisnici mogu potpisati svoj dokument i ažurirati, pretraživati, verificirati, brisati ili pregledavati e-potpise koji su stavljeni na te dokumente. Štoviše, pruža se mnogo mogućnosti za prilagodbu potpisa.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Koraci za potpisivanje Potm s Text u Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) pruža mogućnost brzog i jednostavnog potpisivanja Potm dokumenata s Text potpisima.
        
        * Stvorite instancu klase potpisa koja daje Potm datoteku koja bi se trebala potpisati kao put ili memorijski tok
        * Instancirajte klasu SignOptions i postavite sve tražene podatke.
        * Pozovite metodu Signature.Sign() prosljeđujući izlaznu datoteku Potm ili memorijski tok

    title_right: " Zahtjevi sustava"
    content_right: |
        GroupDocs.Signature for Java podržani su na svim glavnim platformama i operativnim sustavima. Prije izvršavanja koda u nastavku, provjerite imate li sljedeće preduvjete instalirane na vašem sustavu.

        * Operativni sustavi: Microsoft Windows, Linux, MacOS
        * Razvojna okruženja: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Preuzmite najnoviji GroupDocs.Signature for Java od [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Potm file
        String filePath = "input.potm";
        // Set up output file
        String outputFilePath = "output.potm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Potm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Potpisivanje Potm dokumenata s Text Live Demo"
    content: |
       Potpišite datoteku Potm raznim potpisima upravo sada tako da posjetite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web mjesto. Besplatan online demo čeka na vas.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Drugi podržani potpisi Text za Java"
    content: |
        "Također možete potpisati Potm drugim vrstama potpisa. Pogledajte popis u nastavku."
    format: 
       
       
back_to_top:
    enable: true
---