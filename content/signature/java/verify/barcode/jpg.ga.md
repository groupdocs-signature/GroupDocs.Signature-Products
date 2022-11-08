---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Barcode
fileformat: Jpg
productName: Java
lang: ga
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Barcode signature on Jpg for Java

############################# Head ############################
head_title: "Fíorú Barcode sínithe do chomhaid Jpg trí Java"
head_description: "Ná húsáid ach cúpla líne de chód Java chun doiciméid Jpg agus a gcuid sínithe Barcode a fhíorú."

############################# Header ############################
title: "Barcode fíorú sínithe le haghaidh comhad Jpg"
description: "Soláthraíonn API do Java deis chun Barcode sínithe ag Jpg doiciméid a fhíorú. Seans go ndéanfar ríomhshínithe laistigh de do dhoiciméid Jpg a fhíorú go tapa agus go héasca."
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
    title: "Faigh amach gnéithe nua API GroupDocs.Signature for Java"
    content: |
        Soláthraíonn [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API raon leathan bealaí chun go leor formáidí doiciméad a phróiseáil trí úsáid a bhaint as sínithe leictreonacha. Tacaítear le go leor cineálacha sínithe digiteacha mar théacsanna, íomhánna, deimhnithe digiteacha, barrachóid, cóid QR, stampaí nó meiteashonraí. Is féidir le custaiméirí sínithe digiteacha a chur leis, a bhaint, a chur in eagar, a bhailíochtú nó a chuardach ag comhaid PDF, doiciméid MS Word, leabhair oibre MS Excel, láithreoireachtaí MS PowerPoint, comhaid Adobe Photoshop agus formáidí éagsúla íomhá. Tá líon iontach gnéithe agus socruithe breise ar fáil.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Conas Barcode sínithe i do dhoiciméad Jpg a bhailíochtú"
    content_left: |
        Áiríonn [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gnéithe úsáideacha amhail fíorú Barcode sínithe atá curtha ag Jpg doiciméad. Bain úsáid as an deis seo gan cód breise a chur i bhfeidhm.
        
        * Ar an gcéad dul síos, aicme Sínithe meandrach ag soláthar mar chonair paraiméadar cruthaitheoir chuig doiciméad atá ceaptha a fhíorú.
        * Ar an dara dul síos, cruthaigh réad VerifyOptions nua agus socraigh na hairíonna riachtanacha go léir.
        * Ar deireadh, agairt oibiacht Signature Fíoraigh modh a rith VerifyOptions mar shampla.
        * Ansin próiseáil na torthaí fíoraithe.

    title_right: "Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Signature for Java ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.

        * Córais oibriúcháin: Microsoft Windows, Linux, MacOS
        * Timpeallachtaí forbartha: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Íoslódáil an leagan is déanaí de GroupDocs.Signature for Java ó [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Jpg file
        String filePath = "input.jpg";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        BarcodeVerifyOptions options = new BarcodeVerifyOptions();

        // process only specified page 
        options.setPageNumber(2);
        options.setAllPages(false);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Special signature");
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ag síniú le Barcode sínithe Live Demo"
    content: |
       Cuir sínithe leictreonacha éagsúla le comhad Jpg faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Fíoraigh Barcode sínithe eile ag úsáid Java"
    content: |
        "Sínithe leictreonacha a chuirtear i ndoiciméid éagsúla a fhíorú. Seiceáil cáilíocht na sínithe sna formáidí comhaid coitianta mar a léirítear thíos."
    format: 
       
       
back_to_top:
    enable: true
---