---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Dotx
productName: Java
lang: lt
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Dotx with Java

############################# Head ############################
head_title: "Ieškokite Image parašų Dotx faile Java"
head_description: "Naudokite Java, norėdami ieškoti Image parašų Dotx failuose naudodami kelias kodo eilutes."

############################# Header ############################
title: "Ieškokite Image parašų Dotx faile"
description: "Java savoji API leidžia ieškoti Image parašų jau pasirašytuose Dotx failuose. Atlikite išplėstinę el. parašo paiešką savo Dotx dokumentuose naudodami kelias kodo eilutes."
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
    title: "Apie GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) teikia Java API, skirtą dokumentams apdoroti naudojant įvairius parašo tipus, pvz., tekstus, vaizdus, ​​skaitmeninius sertifikatus, brūkšninius kodus, QR kodus, antspaudus ar metaduomenis. Vartotojai gali pridėti, ištrinti, atnaujinti, tikrinti arba ieškoti elektroninių parašų PDF rinkmenose, MS Word dokumentuose, MS Excel darbaknygėse, MS PowerPoint pristatymuose, Adobe Photoshop failuose ir įvairiuose vaizdo formatuose, su papildoma pagalba prireikus tinkinti parašų ypatybes.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kaip ieškoti Image parašų Dotx"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) leidžia Java kūrėjams lengviau ieškoti Image parašų Dotx failuose iš savo programų, atlikdami kelis paprastus veiksmus.
        
        * Sukurkite naują Signature klasės egzempliorių ir nurodykite šaltinio dokumento kelią kaip konstruktoriaus parametrą.
        * Sukurkite paieškos parinkčių objektą pagal savo reikalavimus ir nurodykite paieškos parinktis.
        * Iškvieskite Signature klasės egzemplioriaus paieškos metodą ir perduokite jam paieškos parinktis.
        * Apdorokite paieškos rezultatus pagal savo poreikius.

    title_right: "Sistemos reikalavimai"
    content_right: |
        GroupDocs.Signature for Java palaikomos visose pagrindinėse platformose ir operacinėse sistemose. Prieš vykdydami toliau pateiktą kodą, įsitikinkite, kad jūsų sistemoje yra įdiegtos šios būtinos sąlygos.

        * Operacinės sistemos: Microsoft Windows, Linux, MacOS
        * Kūrimo aplinkos: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Atsisiųskite naujausią GroupDocs.Signature for Java versiją iš [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dotx file
        String filePath = "input.dotx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        ImageSearchOptions options = new ImageSearchOptions();

        // set minimum size if needed 
        options.setMinContentSize(100);
        // set maximum image size if needed
        options.setMaxContentSize(2000);
        // return images for processing
        options.setReturnContent(true);
        // set up type of returned images
        options.setReturnContentType(FileType.PNG);

        // search for Image signatures in Dotx document
        List<ImageSignature> signatures = signature.search(ImageSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ieškokite Image elektroninių parašų tiesioginės demonstracijos"
    content: |
       Dabar ieškokite dokumente įvairių elektroninių parašų prie Dotx failų, apsilankę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) svetainėje.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Ieškokite kitų Image parašų naudodami Java"
    content: |
        "Elektroninių parašų paieška įvairiuose dokumentuose. Raskite parašus iš vieno iš populiarių failų formatų, kaip parodyta toliau."
    format: 
           
       
back_to_top:
    enable: true
---