---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Pptx
productName: Java
lang: hr
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pptx for Java

############################# Head ############################
head_title: "Dodavanje digitalnih elektroničkih potpisa u datoteku Pptx s Java"
head_description: "Stavite digitalni potpis na datoteku Pptx za Java pomoću nekoliko redaka koda. Koristite GroupDocs Document Signature API za potpisivanje desetaka formata datoteka."

############################# Header ############################
title: "eSign Pptx datoteke s Digital potpisima u Java"
description: "Kako dodati Digital potpis s nekoliko redaka Java koda"
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
    title: "O GroupDocs.Signature for Java API-ju za digitalne potpise"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) je popularan API za izradu dokumenata s digitalnim elektroničkim potpisima, s digitalnim certifikatima. Za digitalne potpise API koristi PFX datoteke certifikata za izradu dokumenata s privatnim i javnim ključevima zaštićenim lozinkom. Digitalni potpisi mogu se koristiti za certificiranje poslovnih dokumenata s eSign PDF određenom stranicom, certificiranje cijelih Microsoft Office dokumenata kao što su Words, Excel, Powerpoint datoteke i Open Office dokumenti. Korisnici mogu jednostavno manipulirati potpisima poput uređivanja, uklanjanja ili prilagođavanja. API pruža način pretraživanja i provjere potpisa. Štoviše, pruža se mnogo mogućnosti za prilagodbu potpisa.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Koraci za potpisivanje Pptx s Digital u Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) pruža mogućnost brzog i jednostavnog potpisivanja Pptx dokumenata s Digital potpisima.
        
        * Stvorite instancu klase potpisa koja daje Pptx datoteku koja bi se trebala potpisati kao put ili memorijski tok
        * Instancirajte klasu SignOptions i postavite sve tražene podatke.
        * Pozovite metodu Signature.Sign() prosljeđujući izlaznu datoteku Pptx ili memorijski tok

    title_right: " Zahtjevi sustava"
    content_right: |
        GroupDocs.Signature for Java podržani su na svim glavnim platformama i operativnim sustavima. Prije izvršavanja koda u nastavku, provjerite imate li sljedeće preduvjete instalirane na vašem sustavu.

        * Operativni sustavi: Microsoft Windows, Linux, MacOS
        * Razvojna okruženja: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Preuzmite najnoviji GroupDocs.Signature for Java od [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pptx file
        String filePath = "input.pptx";
        // Set up output file
        String outputFilePath = "output.pptx";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Pptx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Potpisivanje Pptx dokumenata s Digital Live Demo"
    content: |
       Potpišite datoteku Pptx raznim potpisima upravo sada tako da posjetite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web mjesto. Besplatan online demo čeka na vas.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Drugi podržani potpisi Digital za Java"
    content: |
        "Također možete potpisati Pptx drugim vrstama potpisa. Pogledajte popis u nastavku."
    format: 
       
       
back_to_top:
    enable: true
---