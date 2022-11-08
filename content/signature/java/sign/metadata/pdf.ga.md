---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Pdf
productName: Java
lang: ga
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Pdf for Java

############################# Head ############################
head_title: "Cuir sínithe leictreonacha Meiteashonraí i gceangal le doiciméid Pdf trí Java"
head_description: "Úsáid Meiteashonraí mar shínithe leictreonacha folaithe i do dhoiciméid Pdf ag baint úsáide as cúpla líne de chód Java. Bain úsáid as an GroupDocs Document Signature API chun do dhoiciméid ghnó agus do chomhaid a ríomhshíniú le faisnéis Meiteashonraí."

############################# Header ############################
title: "Tá sínithe leictreonacha meiteashonraí do dhoiciméad Pdf trí Java simplí agus éasca le húsáid!"
description: "eSigh do dhoiciméid agus do chonarthaí Pdf le hiontrálacha Meiteashonraí folaithe. Gin Meiteashonraí do PDFs, doiciméid MS Word, leabhair oibre MS Excel, cur i láthair MS PowerPoint agus formáidí íomhá éagsúla gan aon fhadhbanna agus códú breise."
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
    title: "Maidir le GroupDocs.Signature for Java API sínithe meiteashonraí"
    content: |
        Is API coitianta é [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) le haghaidh ríomhshíniú doiciméad digiteach. Tá sínithe amhail téacsanna, íomhánna, teastais dhigiteacha, barrachóid, cóid QR, stampaí nó meiteashonraí ar fáil. D’fhéadfaí sínithe a chur ar PDF, doiciméid MS Word, leabhair oibre MS Excel, láithreoireachtaí MS PowerPoint, comhaid Adobe Photoshop agus formáidí éagsúla íomhá. Is féidir le custaiméirí a ndoiciméad a shíniú agus ríomhshínithe a cuireadh ar na doiciméid sin a nuashonrú, a chuardach, a fhíorú, a scriosadh nó a réamhamharc. Thairis sin, soláthraítear go leor cumais le haghaidh saincheapadh sínithe.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Céimeanna chun Pdf a shíniú le Metadata in Java"
    content_left: |
        Soláthraíonn [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) cumas chun doiciméid Pdf a shíniú le sínithe Metadata go tapa agus go héasca.
        
        * Cruthaigh sampla d'aicme Sínithe ag soláthar Pdf comhad atá ceaptha a shíniú mar chonair nó mar shruth cuimhne
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
                
        // Set up input Pdf file
        String filePath = "input.pdf";
        // Set up output file
        String outputFilePath = "output.pdf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        PdfMetadataSignature mdSign_Author = new PdfMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        PdfMetadataSignature mdSign_DocData = new PdfMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        PdfMetadataSignature mdSign_DocId = new PdfMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Pdf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ag síniú Pdf doiciméad le {{ Signaturetype}} Taispeántas Beo"
    content: |
       Sínigh Pdf comhad le sínithe éagsúla faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Saor in aisce taispeána ar líne ag fanacht leat.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Sínithe Metadata eile a dtacaítear leo le haghaidh Java"
    content: |
        "Is féidir leat Pdf a shíniú le cineálacha sínithe eile freisin. Féach ar an liosta thíos le do thoil."
    format: 
       
       
back_to_top:
    enable: true
---