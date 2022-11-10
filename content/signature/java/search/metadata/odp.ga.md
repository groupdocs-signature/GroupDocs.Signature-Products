---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Odp
productName: Java
lang: ga
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Odp with Java

############################# Head ############################
head_title: "Cuardaigh Metadata síniú i gcomhad Odp i Java"
head_description: "Úsáid Java chun sínithe Metadata a chuardach i gcomhaid Odp ag úsáid cúpla líne de chód."

############################# Header ############################
title: "Cuardaigh le haghaidh Metadata sínithe i gcomhad Odp"
description: "Ceadaíonn API dúchais Java cuardach a dhéanamh ar Metadata sínithe i gcomhaid Odp atá sínithe cheana féin. Déan ard-chuardach ríomhshínithe laistigh de do dhoiciméid Odp ag úsáid cúpla líne cód."
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
    title: "Maidir le GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) soláthraíonn Java API chun doiciméid a phróiseáil ag baint úsáide as cineálacha sínithe éagsúla ar nós téacsanna, íomhánna, teastais dhigiteacha, barrachóid, QR-cóid, stampaí nó meiteashonraí. Is féidir le húsáideoirí sínithe leictreonacha a chur leis, a scriosadh, a nuashonrú, a fhíorú nó a chuardach laistigh de PDFs, doiciméid MS Word, leabhair oibre MS Excel, cur i láthair MS PowerPoint, comhaid Adobe Photoshop agus formáidí íomhá éagsúla, le tacaíocht bhreise chun airíonna sínithe a shaincheapadh de réir mar is gá.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Conas síniú Metadata a chuardach i Odp"
    content_left: |
        Déanann [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) é níos fusa d’fhorbróirí Java cuardach a dhéanamh ar shínithe Metadata i gcomhaid Odp óna bhfeidhmchláir trí roinnt céimeanna éasca a chur i bhfeidhm.
        
        * Cruthaigh sampla nua den rang Sínithe agus pas a fháil ar chonair an doiciméid foinse mar pharaiméadar cruthaitheoir.
        * Cuir an oibiacht SearchOptions ar bun de réir do riachtanais agus sonraigh roghanna cuardaigh.
        * Glaoigh ar an modh cuardaigh ar shampla rang Sínithe agus cuir SearchOptions chuige.
        * Próiseáil torthaí cuardaigh de réir d'éilimh.

    title_right: "Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Signature for Java ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.

        * Córais oibriúcháin: Microsoft Windows, Linux, MacOS
        * Timpeallachtaí forbartha: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Íoslódáil an leagan is déanaí de GroupDocs.Signature for Java ó [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
        
        // Set up input Odp file
        String filePath = "input.odp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // search for Metadata signatures in Odp document
        List<PresentationMetadataSignature> signatures = signature.search(PresentationMetadataSignature.class, SignatureType.Metadata);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));


        ```

############################# Demos ############################
demos:
    enable: true
    title: "Cuardaigh le haghaidh Metadata sínithe leictreonacha Live Demo"
    content: |
       Cuardaigh an doiciméad le haghaidh sínithe leictreonacha éagsúla ar chomhaid Odp faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cuardaigh sínithe Metadata eile ag úsáid Java"
    content: |
        "Cuardach sínithe leictreonacha i ndoiciméid éagsúla. Faigh sínithe ón gceann de na formáidí comhaid coitianta mar a thaispeántar thíos."
    format: 
           
       
back_to_top:
    enable: true
---