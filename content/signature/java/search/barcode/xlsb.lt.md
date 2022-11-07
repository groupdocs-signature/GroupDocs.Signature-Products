---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Barcode
fileformat: Xlsb
productName: Java
lang: lt
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Barcode signatures at Xlsb with Java

############################# Head ############################
head_title: "Ieškokite Barcode parašų Xlsb faile Java"
head_description: "Naudokite Java, norėdami ieškoti Barcode parašų Xlsb failuose naudodami kelias kodo eilutes."

############################# Header ############################
title: "Ieškokite Barcode parašų Xlsb faile"
description: "Java savoji API leidžia ieškoti Barcode parašų jau pasirašytuose Xlsb failuose. Atlikite išplėstinę el. parašo paiešką savo Xlsb dokumentuose naudodami kelias kodo eilutes."
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
    title_left: "Kaip ieškoti Barcode parašų Xlsb"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) leidžia Java kūrėjams lengviau ieškoti Barcode parašų Xlsb failuose iš savo programų, atlikdami kelis paprastus veiksmus.
        
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
        
        // Set up input Xlsb file
        String filePath = "input.xlsb";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        BarcodeSearchOptions options = new BarcodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Barcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Barcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Barcode signatures in Xlsb document
        List<BarcodeSignature> signatures = signature.search(BarcodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ieškokite Barcode elektroninių parašų tiesioginės demonstracijos"
    content: |
       Dabar ieškokite dokumente įvairių elektroninių parašų prie Xlsb failų, apsilankę [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) svetainėje.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Ieškokite kitų Barcode parašų naudodami Java"
    content: |
        "Elektroninių parašų paieška įvairiuose dokumentuose. Raskite parašus iš vieno iš populiarių failų formatų, kaip parodyta toliau."
    format: 
           
       
back_to_top:
    enable: true
---