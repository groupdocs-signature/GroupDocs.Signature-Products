---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Ppsm
productName: Java
lang: ga
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Ppsm for Java

############################# Head ############################
head_title: "Scrios Qrcode sínithe ó chomhaid Ppsm trí Java"
head_description: "Seans go ndéanfaí scriosadh sínithe Qrcode ar leith ó dhoiciméid shínithe Ppsm le cód gearr Java."

############################# Header ############################
title: "Bain Qrcode sínithe a chuirtear i gcomhaid Ppsm"
description: "Scrios Qrcode sínithe éagsúla ó Ppsm doiciméid. Teastaíonn cód simplí Java chun sínithe Qrcode a bhaint."
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
    title: "Faigh faisnéis faoi ghnéithe API GroupDocs.Signature for Java"
    content: |
        Soláthraíonn [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API go leor bealaí chun do dhoiciméid a phróiseáil le sínithe leictreonacha. Tá sínithe digiteacha amhail téacsanna, íomhánna, teastais dhigiteacha, barrachóid, cóid QR, stampaí nó meiteashonraí ar fáil. Féadfaidh custaiméirí sínithe digiteacha a chur leis, a scriosadh, a nuashonrú, a fhíorú nó a chuardach ag PDFs, doiciméid MS Word, leabhair oibre MS Excel, láithreoireachtaí MS PowerPoint, comhaid Adobe Photoshop agus formáidí éagsúla íomhá. Soláthraítear líon mór gnéithe agus socruithe úsáideacha.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Conas Qrcode sínithe a bhaint de do dhoiciméad Ppsm"
    content_left: |
        Soláthraíonn [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gné úsáideach chun Ppsm doiciméad de Qrcode sínithe a ghlanadh le cúpla líne de chód.
        
        * Ar an gcéad dul síos, cuir an réad Síniú ar an toirt ag dul chuig do dhoiciméad mar pharaiméadar cruthaitheoir.
        * Ansin, cruthaigh réad sínithe cuí agus socraigh a aitheantóir uathúil.
        * Tar éis sin, agairt modh Scrios réad sínithe a rith a chaithfear a scriosadh.
        * Ar deireadh, torthaí oibríochta próisis.

    title_right: "Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Signature for Java ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.

        * Córais oibriúcháin: Microsoft Windows, Linux, MacOS
        * Timpeallachtaí forbartha: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Íoslódáil an leagan is déanaí de GroupDocs.Signature for Java ó [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ppsm file
        String filePath = "input.ppsm";
        // Set up output file
        String outputFilePath = "output.ppsm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to delete
        QrCodeSignature signatureToDelete = new QrCodeSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ag síniú le Qrcode sínithe Live Demo"
    content: |
       Cuir sínithe leictreonacha éagsúla le comhad Ppsm faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Scrios do Qrcode sínithe le Java"
    content: |
        "Scriosadh ríomhshínithe a cuireadh le formáidí éagsúla doiciméad. Bain sínithe go tapa gan cód breise."
    format: 
       
       
back_to_top:
    enable: true
---