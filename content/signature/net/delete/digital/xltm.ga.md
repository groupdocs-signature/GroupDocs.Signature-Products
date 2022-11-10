---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Xltm
productName: .NET
lang: ga
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xltm for C#

############################# Head ############################
head_title: "Scrios Digital sínithe ó chomhaid Xltm trí C#"
head_description: "Seans go ndéanfaí scriosadh sínithe Digital ar leith ó dhoiciméid shínithe Xltm le cód gearr .NET."

############################# Header ############################
title: "Bain Digital sínithe a chuirtear i gcomhaid Xltm"
description: "Scrios Digital sínithe éagsúla ó Xltm doiciméid. Teastaíonn cód simplí C# chun sínithe Digital a bhaint."
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
    title: "Faigh faisnéis faoi ghnéithe API GroupDocs.Signature for .NET"
    content: |
        Soláthraíonn [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API go leor bealaí chun do dhoiciméid a phróiseáil le sínithe leictreonacha. Tá sínithe digiteacha amhail téacsanna, íomhánna, teastais dhigiteacha, barrachóid, cóid QR, stampaí nó meiteashonraí ar fáil. Féadfaidh custaiméirí sínithe digiteacha a chur leis, a scriosadh, a nuashonrú, a fhíorú nó a chuardach ag PDFs, doiciméid MS Word, leabhair oibre MS Excel, láithreoireachtaí MS PowerPoint, comhaid Adobe Photoshop agus formáidí éagsúla íomhá. Soláthraítear líon mór gnéithe agus socruithe úsáideacha.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Conas Digital sínithe a bhaint de do dhoiciméad Xltm"
    content_left: |
        Soláthraíonn [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) gné úsáideach chun Xltm doiciméad de Digital sínithe a ghlanadh le cúpla líne de chód.
        
        * Ar an gcéad dul síos, cuir an réad Síniú ar an toirt ag dul chuig do dhoiciméad mar pharaiméadar cruthaitheoir.
        * Ansin, cruthaigh réad sínithe cuí agus socraigh a aitheantóir uathúil.
        * Tar éis sin, agairt modh Scrios réad sínithe a rith a chaithfear a scriosadh.
        * Ar deireadh, torthaí oibríochta próisis.

    title_right: "Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Signature for .NET ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.

        * Córais oibriúcháin: Microsoft Windows, Linux, MacOS
        * Timpeallachtaí forbartha: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Íoslódáil an leagan is déanaí de GroupDocs.Signature for .NET ó [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xltm file
        string filePath = "input.xltm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "a01e1940-997a-444b-89af-9309a2d559a5";

                // provide signature features to delete
                // set up particular signature id
                DigitalSignature signatureToDelete = new DigitalSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ag síniú le Digital sínithe Live Demo"
    content: |
       Cuir sínithe leictreonacha éagsúla le comhad Xltm faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Scrios do Digital sínithe le C#"
    content: |
        "Scriosadh ríomhshínithe a cuireadh le formáidí éagsúla doiciméad. Bain sínithe go tapa gan cód breise."
    format: 
       
       
back_to_top:
    enable: true
---