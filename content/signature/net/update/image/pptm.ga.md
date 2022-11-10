---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Pptm
productName: .NET
lang: ga
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Pptm for C#

############################# Head ############################
head_title: "Nuashonraigh Image sínithe atá curtha i gcomhad Pptm le C#"
head_description: "Úsáid cód .NET atá simplí agus éasca le tuiscint le haghaidh nuashonruithe sínithe Image i ndoiciméid sínithe Pptm."

############################# Header ############################
title: "Cuir in eagar agus nuashonraigh Image sínithe atá curtha ag comhaid Pptm"
description: "Soláthraíonn API le haghaidh .NET feidhmiúlacht le haghaidh sínithe Image nuashonraithe ag Pptm doiciméad. Nuashonraigh ríomhshínithe taobh istigh de do dhoiciméid Pptm le cúpla líne de chód C# go tapa agus go héasca."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Faigh amach faoi ghnéithe API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) Tá rogha leathan bealaí le próiseáil i bhformáidí doiciméid éilimh trí úsáid a bhaint as sínithe leictreonacha i bhfeidhmiúlacht API. Tacaítear le speictream leathan ríomhshínithe amhail téacsanna, íomhánna, deimhnithe digiteacha, barrachóid, cóid QR, stampaí nó meiteashonraí. Is féidir le custaiméirí sínithe digiteacha a chur leis, a bhaint, a chur in eagar, a bhailíochtú nó a chuardach ag comhaid PDF, doiciméid MS Word, leabhair oibre MS Excel, láithreoireachtaí MS PowerPoint, comhaid Adobe Photoshop agus formáidí éagsúla íomhá. Tá go leor gnéithe agus socruithe úsáideacha ar fáil.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Conas Image sínithe a athrú i do dhoiciméad Pptm"
    content_left: |
        Cuimsíonn [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) gnéithe úsáideacha amhail nuashonrú ar Image sínithe a cuireadh i ndoiciméid Pptm. Is féidir gnéithe sínithe a athrú gan cód breise.
        
        * Ar dtús, cruthaigh réad Síniú ag dul mar chonair paraiméadar cruthaitheoir chuig doiciméad atá le nuashonrú.
        * Ansin, cuir réad sínithe cuí ar an toirt ar an toirt agus socraigh a aitheantóir agus a airíonna nach mór a athrú.
        * Ar deireadh, cuir glaoch ar an modh Nuashonraithe Signature chun réad sínithe ar leith a rith.
        * Próiseáil na torthaí a nuashonrú le d'fhógra.

    title_right: "Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Signature for .NET ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.

        * Córais oibriúcháin: Microsoft Windows, Linux, MacOS
        * Timpeallachtaí forbartha: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Íoslódáil an leagan is déanaí de GroupDocs.Signature for .NET ó [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pptm file
        string filePath = "input.pptm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                // set up particular signature id
                ImageSignature signatureToUpdate = new ImageSignature(id)
                {
                    // specify signature width
                    Width = 170,
                    // specify signature height
                    Height = 250,
                    // set left position
                    Left = 10,
                    // set top position
                    Top = 10
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Na sínithe Image ar leathanaigh na doiciméid a nuashonrú - Taispeántas Beo"
    content: |
       Cuir sínithe leictreonacha éagsúla den doiciméad Pptm in eagar faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Nuashonraigh sínithe Image éagsúla trí C#"
    content: |
        "Sínithe digiteacha a chur in eagar a chuirtear i bhformáidí éagsúla doiciméad. Nuashonraigh sonraí sínithe gan cód breise."
    format: 
       
       
back_to_top:
    enable: true
---