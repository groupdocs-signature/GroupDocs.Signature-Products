---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Xls
productName: Java
lang: ga
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Xls for Java

############################# Head ############################
head_title: "Nuashonraigh Text sínithe atá curtha i gcomhad Xls le Java"
head_description: "Úsáid cód Java atá simplí agus éasca le tuiscint le haghaidh nuashonruithe sínithe Text i ndoiciméid sínithe Xls."

############################# Header ############################
title: "Cuir in eagar agus nuashonraigh Text sínithe atá curtha ag comhaid Xls"
description: "Soláthraíonn API le haghaidh Java feidhmiúlacht le haghaidh sínithe Text nuashonraithe ag Xls doiciméad. Nuashonraigh ríomhshínithe taobh istigh de do dhoiciméid Xls le cúpla líne de chód Java go tapa agus go héasca."
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
    title_left: "Conas Text sínithe a athrú i do dhoiciméad Xls"
    content_left: |
        Cuimsíonn [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) gnéithe úsáideacha amhail nuashonrú ar Text sínithe a cuireadh i ndoiciméid Xls. Is féidir gnéithe sínithe a athrú gan cód breise.
        
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
                
        // Set up input Xls file
        String filePath = "input.xls";
        // Set up output file
        String outputFilePath = "output.xls";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to update
        // set up particular signature id
        TextSignature signatureToUpdate = new TextSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(130);
        // specify signature height
        signatureToUpdate.setHeight(20);
        // set left position
        signatureToUpdate.setLeft(40);
        // set top position
        signatureToUpdate.setTop(50);
        // set up new text
        signatureToUpdate.setText("Mr. John Smith");

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
    title: "Na sínithe Text ar leathanaigh na doiciméid a nuashonrú - Taispeántas Beo"
    content: |
       Cuir sínithe leictreonacha éagsúla den doiciméad Xls in eagar faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Nuashonraigh sínithe Text éagsúla trí Java"
    content: |
        "Sínithe digiteacha a chur in eagar a chuirtear i bhformáidí éagsúla doiciméad. Nuashonraigh sonraí sínithe gan cód breise."
    format: 
       
       
back_to_top:
    enable: true
---