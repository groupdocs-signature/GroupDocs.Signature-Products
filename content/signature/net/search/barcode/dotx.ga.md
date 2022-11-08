---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Barcode
fileformat: Dotx
productName: .NET
lang: ga
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Barcode signatures at Dotx with C#

############################# Head ############################
head_title: "Cuardaigh Barcode síniú i gcomhad Dotx i C#"
head_description: "Úsáid .NET chun sínithe Barcode a chuardach i gcomhaid Dotx ag úsáid cúpla líne de chód."

############################# Header ############################
title: "Cuardaigh le haghaidh Barcode sínithe i gcomhad Dotx"
description: "Ceadaíonn API dúchais .NET cuardach a dhéanamh ar Barcode sínithe i gcomhaid Dotx atá sínithe cheana féin. Déan ard-chuardach ríomhshínithe laistigh de do dhoiciméid Dotx ag úsáid cúpla líne cód."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Maidir le GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) soláthraíonn .NET API chun doiciméid a phróiseáil ag baint úsáide as cineálacha sínithe éagsúla ar nós téacsanna, íomhánna, teastais dhigiteacha, barrachóid, QR-cóid, stampaí nó meiteashonraí. Is féidir le húsáideoirí sínithe leictreonacha a chur leis, a scriosadh, a nuashonrú, a fhíorú nó a chuardach laistigh de PDFs, doiciméid MS Word, leabhair oibre MS Excel, cur i láthair MS PowerPoint, comhaid Adobe Photoshop agus formáidí íomhá éagsúla, le tacaíocht bhreise chun airíonna sínithe a shaincheapadh de réir mar is gá.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Conas síniú Barcode a chuardach i Dotx"
    content_left: |
        Déanann [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) é níos fusa d’fhorbróirí .NET cuardach a dhéanamh ar shínithe Barcode i gcomhaid Dotx óna bhfeidhmchláir trí roinnt céimeanna éasca a chur i bhfeidhm.
        
        * Cruthaigh sampla nua den rang Sínithe agus pas a fháil ar chonair an doiciméid foinse mar pharaiméadar cruthaitheoir.
        * Cuir an oibiacht SearchOptions ar bun de réir do riachtanais agus sonraigh roghanna cuardaigh.
        * Glaoigh ar an modh cuardaigh ar shampla rang Sínithe agus cuir SearchOptions chuige.
        * Próiseáil torthaí cuardaigh de réir d'éilimh.

    title_right: "Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Signature for .NET ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.

        * Córais oibriúcháin: Microsoft Windows, Linux, MacOS
        * Timpeallachtaí forbartha: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Íoslódáil an leagan is déanaí de GroupDocs.Signature for .NET ó [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Dotx file
        string filePath = "input.dotx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                BarcodeSearchOptions options = new BarcodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Barcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Barcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Barcode signatures in Dotx document
                List<BarcodeSignature> signatures = signature.Search<BarcodeSignature>(options);

                // process signatures which were found                
                foreach (BarcodeSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Cuardaigh le haghaidh Barcode sínithe leictreonacha Live Demo"
    content: |
       Cuardaigh an doiciméad le haghaidh sínithe leictreonacha éagsúla ar chomhaid Dotx faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cuardaigh sínithe Barcode eile ag úsáid C#"
    content: |
        "Cuardach sínithe leictreonacha i ndoiciméid éagsúla. Faigh sínithe ón gceann de na formáidí comhaid coitianta mar a thaispeántar thíos."
    format: 
           
       
back_to_top:
    enable: true
---