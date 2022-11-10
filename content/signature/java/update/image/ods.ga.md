---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Ods
productName: Java
lang: ga
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Ods for Java

############################# Head ############################
head_title: "Nuashonraigh Image sínithe atá curtha i gcomhad Ods le Java"
head_description: "Úsáid cód Java atá simplí agus éasca le tuiscint le haghaidh nuashonruithe sínithe Image i ndoiciméid sínithe Ods."

############################# Header ############################
title: "Cuir in eagar agus nuashonraigh Image sínithe atá curtha ag comhaid Ods"
description: "Soláthraíonn API le haghaidh Java feidhmiúlacht le haghaidh sínithe Image nuashonraithe ag Ods doiciméad. Nuashonraigh ríomhshínithe taobh istigh de do dhoiciméid Ods le cúpla líne de chód Java go tapa agus go héasca."
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
    title: "Faigh amach faoi ghnéithe API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) Tá rogha leathan bealaí le próiseáil i bhformáidí doiciméid éilimh trí úsáid a bhaint as sínithe leictreonacha i bhfeidhmiúlacht API. Tacaítear le speictream leathan ríomhshínithe amhail téacsanna, íomhánna, deimhnithe digiteacha, barrachóid, cóid QR, stampaí nó meiteashonraí. Is féidir le custaiméirí sínithe digiteacha a chur leis, a bhaint, a chur in eagar, a bhailíochtú nó a chuardach ag comhaid PDF, doiciméid MS Word, leabhair oibre MS Excel, láithreoireachtaí MS PowerPoint, comhaid Adobe Photoshop agus formáidí éagsúla íomhá. Tá go leor gnéithe agus socruithe úsáideacha ar fáil.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Conas Image sínithe a athrú i do dhoiciméad Ods"
    content_left: |
        Cuimsíonn [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gnéithe úsáideacha amhail nuashonrú ar Image sínithe a cuireadh i ndoiciméid Ods. Is féidir gnéithe sínithe a athrú gan cód breise.
        
        * Ar dtús, cruthaigh réad Síniú ag dul mar chonair paraiméadar cruthaitheoir chuig doiciméad atá le nuashonrú.
        * Ansin, cuir réad sínithe cuí ar an toirt ar an toirt agus socraigh a aitheantóir agus a airíonna nach mór a athrú.
        * Ar deireadh, cuir glaoch ar an modh Nuashonraithe Signature chun réad sínithe ar leith a rith.
        * Próiseáil na torthaí a nuashonrú le d'fhógra.

    title_right: "Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Signature for Java ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.

        * Córais oibriúcháin: Microsoft Windows, Linux, MacOS
        * Timpeallachtaí forbartha: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Íoslódáil an leagan is déanaí de GroupDocs.Signature for Java ó [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ods file
        String filePath = "input.ods";
        // Set up output file
        String outputFilePath = "output.ods";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to update
        // set up particular signature id
        ImageSignature signatureToUpdate = new ImageSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(170);
        // specify signature height
        signatureToUpdate.setHeight(250);
        // set left position
        signatureToUpdate.setLeft(10);
        // set top position
        signatureToUpdate.setTop(10);

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Na sínithe Image ar leathanaigh na doiciméid a nuashonrú - Taispeántas Beo"
    content: |
       Cuir sínithe leictreonacha éagsúla den doiciméad Ods in eagar faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Nuashonraigh sínithe Image éagsúla trí Java"
    content: |
        "Sínithe digiteacha a chur in eagar a chuirtear i bhformáidí éagsúla doiciméad. Nuashonraigh sonraí sínithe gan cód breise."
    format: 
       
       
back_to_top:
    enable: true
---