---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Doc
productName: Java
lang: ga
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Doc for Java

############################# Head ############################
head_title: "Sínithe leictreonacha digiteacha á gcur le comhad Doc le Java"
head_description: "Cuir Síniú Digiteach ar chomhad Doc le haghaidh Java ag baint úsáide as cúpla líne de chód. Úsáid an GroupDocs Document Signature API chun mórán formáidí comhaid a shíniú."

############################# Header ############################
title: "eSínigh Doc comhaid le {{ Signaturetype}} sínithe in Java"
description: "Conas Digital síniú a chur leis le cúpla líne de chód Java"
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
    title: "Maidir le GroupDocs.Signature for Java API sínithe digiteacha"
    content: |
        Is API coitianta é [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) chun doiciméid a bhfuil sínithe leictreonacha digiteacha orthu a shíniú, agus teastais dhigiteacha orthu. Le haghaidh sínithe digiteacha úsáideann API comhaid teastais PFX chun doiciméad a shíniú le heochracha príobháideacha agus poiblí cosanta ag pasfhocal. Féadfar na sínithe Digiteacha a úsáid chun doiciméid ghnó a dheimhniú le leathanach áirithe eSign PDF, chun doiciméid iomlána Microsoft Office a dheimhniú mar Words, Excel, comhaid Powerpoint, agus doiciméid Open Office. Is féidir le custaiméirí na sínithe a ionramháil go héasca ar nós eagarthóireacht a dhéanamh orthu, iad a bhaint nó a choigeartú. Soláthraíonn an API bealach chun sínithe a chuardach agus a fhíorú. Thairis sin, soláthraítear go leor cumais le haghaidh saincheapadh sínithe.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Céimeanna chun Doc a shíniú le Digital in Java"
    content_left: |
        Soláthraíonn [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) cumas chun doiciméid Doc a shíniú le sínithe Digital go tapa agus go héasca.
        
        * Cruthaigh sampla d'aicme Sínithe ag soláthar Doc comhad atá ceaptha a shíniú mar chonair nó mar shruth cuimhne
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
                
        // Set up input Doc file
        String filePath = "input.doc";
        // Set up output file
        String outputFilePath = "output.doc";
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

        // sign Doc document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ag síniú Doc doiciméad le {{ Signaturetype}} Taispeántas Beo"
    content: |
       Sínigh Doc comhad le sínithe éagsúla faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Saor in aisce taispeána ar líne ag fanacht leat.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Sínithe Digital eile a dtacaítear leo le haghaidh Java"
    content: |
        "Is féidir leat Doc a shíniú le cineálacha sínithe eile freisin. Féach ar an liosta thíos le do thoil."
    format: 
       
       
back_to_top:
    enable: true
---