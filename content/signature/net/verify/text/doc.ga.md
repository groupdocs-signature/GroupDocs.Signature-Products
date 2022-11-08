---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Text
fileformat: Doc
productName: .NET
lang: ga
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Doc for C#

############################# Head ############################
head_title: "Fíorú Text sínithe do chomhaid Doc trí C#"
head_description: "Ná húsáid ach cúpla líne de chód .NET chun doiciméid Doc agus a gcuid sínithe Text a fhíorú."

############################# Header ############################
title: "Text fíorú sínithe le haghaidh comhad Doc"
description: "Soláthraíonn API do .NET deis chun Text sínithe ag Doc doiciméid a fhíorú. Seans go ndéanfar ríomhshínithe laistigh de do dhoiciméid Doc a fhíorú go tapa agus go héasca."
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
    title: "Faigh amach gnéithe nua API GroupDocs.Signature for .NET"
    content: |
        Soláthraíonn [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API raon leathan bealaí chun go leor formáidí doiciméad a phróiseáil trí úsáid a bhaint as sínithe leictreonacha. Tacaítear le go leor cineálacha sínithe digiteacha mar théacsanna, íomhánna, deimhnithe digiteacha, barrachóid, cóid QR, stampaí nó meiteashonraí. Is féidir le custaiméirí sínithe digiteacha a chur leis, a bhaint, a chur in eagar, a bhailíochtú nó a chuardach ag comhaid PDF, doiciméid MS Word, leabhair oibre MS Excel, láithreoireachtaí MS PowerPoint, comhaid Adobe Photoshop agus formáidí éagsúla íomhá. Tá líon iontach gnéithe agus socruithe breise ar fáil.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Conas Text sínithe i do dhoiciméad Doc a bhailíochtú"
    content_left: |
        Áiríonn [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) gnéithe úsáideacha amhail fíorú Text sínithe atá curtha ag Doc doiciméad. Bain úsáid as an deis seo gan cód breise a chur i bhfeidhm.
        
        * Ar an gcéad dul síos, aicme Sínithe meandrach ag soláthar mar chonair paraiméadar cruthaitheoir chuig doiciméad atá ceaptha a fhíorú.
        * Ar an dara dul síos, cruthaigh réad VerifyOptions nua agus socraigh na hairíonna riachtanacha go léir.
        * Ar deireadh, agairt oibiacht Signature Fíoraigh modh a rith VerifyOptions mar shampla.
        * Ansin próiseáil na torthaí fíoraithe.

    title_right: "Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Signature for .NET ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.

        * Córais oibriúcháin: Microsoft Windows, Linux, MacOS
        * Timpeallachtaí forbartha: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Íoslódáil an leagan is déanaí de GroupDocs.Signature for .NET ó [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                TextVerifyOptions options = new TextVerifyOptions()
                {
                    // Process all pages 
                    AllPages = true,
                    // set up text match type
                    MatchType = TextMatchType.Exact,
                    // specify text pattern to search
                    Text = "Very important signature",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ag síniú le Text sínithe Live Demo"
    content: |
       Cuir sínithe leictreonacha éagsúla le comhad Doc faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Fíoraigh Text sínithe eile ag úsáid C#"
    content: |
        "Sínithe leictreonacha a chuirtear i ndoiciméid éagsúla a fhíorú. Seiceáil cáilíocht na sínithe sna formáidí comhaid coitianta mar a léirítear thíos."
    format: 
       
       
back_to_top:
    enable: true
---