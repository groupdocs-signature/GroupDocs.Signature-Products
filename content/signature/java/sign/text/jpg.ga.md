---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Jpg
productName: Java
lang: ga
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Jpg for Java

############################# Head ############################
head_title: "Cruthaigh sínithe leictreonacha Téacs chun Jpg a chomhdú le Java"
head_description: "Cuir Text eSignature ar Jpg comhad le haghaidh Java ag baint úsáide as cúpla líne de chód. Úsáid an GroupDocs Document Signature API chun mórán formáidí comhaid a shíniú."

############################# Header ############################
title: "Sínigh Jpg comhad le sínithe Text in Java"
description: "Conas Text Síniú a chur leis le cúpla líne de chód Java"
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
    title: "Maidir le GroupDocs.Signature for Java API"
    content: |
        Is API coitianta é [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) le haghaidh ríomhshíniú doiciméad digiteach. Tá sínithe amhail téacsanna, íomhánna, teastais dhigiteacha, barrachóid, cóid QR, stampaí nó meiteashonraí ar fáil. D’fhéadfaí sínithe a chur ar PDF, doiciméid MS Word, leabhair oibre MS Excel, láithreoireachtaí MS PowerPoint, comhaid Adobe Photoshop agus formáidí éagsúla íomhá. Is féidir le custaiméirí a ndoiciméad a shíniú agus ríomhshínithe a cuireadh ar na doiciméid sin a nuashonrú, a chuardach, a fhíorú, a scriosadh nó a réamhamharc. Thairis sin, soláthraítear go leor cumais le haghaidh saincheapadh sínithe.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Céimeanna chun Jpg a shíniú le Text in Java"
    content_left: |
        Soláthraíonn [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) cumas chun doiciméid Jpg a shíniú le sínithe Text go tapa agus go héasca.
        
        * Cruthaigh sampla d'aicme Sínithe ag soláthar Jpg comhad atá ceaptha a shíniú mar chonair nó mar shruth cuimhne
        * Cuir rang SignOptions ar bun agus socraigh na sonraí go léir a éilítear.
        * Iarr ar an modh Signature.Sign() aschuir {{ Fileformat}} comhad nó sruth cuimhne a rith

    title_right: " Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Signature for Java ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.

        * Córais oibriúcháin: Microsoft Windows, Linux, MacOS
        * Timpeallachtaí forbartha: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Faigh an GroupDocs.Signature for Java is déanaí ó [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Jpg file
        String filePath = "input.jpg";
        // Set up output file
        String outputFilePath = "output.jpg";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Jpg document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ag síniú Jpg doiciméad le {{ Signaturetype}} Taispeántas Beo"
    content: |
       Sínigh Jpg comhad le sínithe éagsúla faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Saor in aisce taispeána ar líne ag fanacht leat.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Sínithe Text eile a dtacaítear leo le haghaidh Java"
    content: |
        "Is féidir leat Jpg a shíniú le cineálacha sínithe eile freisin. Féach ar an liosta thíos le do thoil."
    format: 
       
       
back_to_top:
    enable: true
---