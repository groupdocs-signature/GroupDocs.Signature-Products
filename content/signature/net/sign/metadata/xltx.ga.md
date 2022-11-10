---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Xltx
productName: .NET
lang: ga
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Xltx for C#

############################# Head ############################
head_title: "Cuir sínithe leictreonacha Meiteashonraí i gceangal le doiciméid Xltx trí C#"
head_description: "Úsáid Meiteashonraí mar shínithe leictreonacha folaithe i do dhoiciméid Xltx ag baint úsáide as cúpla líne de chód C#. Bain úsáid as an GroupDocs Document Signature API chun do dhoiciméid ghnó agus do chomhaid a ríomhshíniú le faisnéis Meiteashonraí."

############################# Header ############################
title: "Tá sínithe leictreonacha meiteashonraí do dhoiciméad Xltx trí .NET simplí agus éasca le húsáid!"
description: "eSigh do dhoiciméid agus do chonarthaí Xltx le hiontrálacha Meiteashonraí folaithe. Gin Meiteashonraí do PDFs, doiciméid MS Word, leabhair oibre MS Excel, cur i láthair MS PowerPoint agus formáidí íomhá éagsúla gan aon fhadhbanna agus códú breise."
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
    title: "Maidir le GroupDocs.Signature for .NET API sínithe meiteashonraí"
    content: |
        Is API coitianta é [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) le haghaidh ríomhshíniú doiciméad digiteach. Tá sínithe amhail téacsanna, íomhánna, teastais dhigiteacha, barrachóid, cóid QR, stampaí nó meiteashonraí ar fáil. D’fhéadfaí sínithe a chur ar PDF, doiciméid MS Word, leabhair oibre MS Excel, láithreoireachtaí MS PowerPoint, comhaid Adobe Photoshop agus formáidí éagsúla íomhá. Is féidir le custaiméirí a ndoiciméad a shíniú agus ríomhshínithe a cuireadh ar na doiciméid sin a nuashonrú, a chuardach, a fhíorú, a scriosadh nó a réamhamharc. Thairis sin, soláthraítear go leor cumais le haghaidh saincheapadh sínithe.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Céimeanna chun Xltx a shíniú le Metadata in C#"
    content_left: |
        Soláthraíonn [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) cumas chun doiciméid Xltx a shíniú le sínithe Metadata go tapa agus go héasca.
        
        * Cruthaigh sampla d'aicme Sínithe ag soláthar Xltx comhad atá ceaptha a shíniú mar chonair nó mar shruth cuimhne
        * Cuir rang SignOptions ar bun agus socraigh na sonraí go léir a éilítear.
        * Iarr ar an modh Signature.Sign() aschuir Xltx comhad nó sruth cuimhne a rith

    title_right: " Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Signature for .NET ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.

        * Córais oibriúcháin: Microsoft Windows, Linux, MacOS
        * Timpeallachtaí forbartha: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Faigh an GroupDocs.Signature for .NET is déanaí ó [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Xltx file
        string filePath = "input.xltx";
        // Set up output file
        string outputFilePath = "output.xltx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Xltx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ag síniú Xltx doiciméad le Metadata Taispeántas Beo"
    content: |
       Sínigh Xltx comhad le sínithe éagsúla faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Saor in aisce taispeána ar líne ag fanacht leat.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Sínithe Metadata eile a dtacaítear leo le haghaidh C#"
    content: |
        "Is féidir leat Xltx a shíniú le cineálacha sínithe eile freisin. Féach ar an liosta thíos le do thoil."
    format: 
       
       
back_to_top:
    enable: true
---