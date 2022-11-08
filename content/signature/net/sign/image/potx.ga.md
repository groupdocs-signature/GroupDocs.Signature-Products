---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Potx
productName: .NET
lang: ga
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Potx for C#

############################# Head ############################
head_title: "Ag cur Image sínithe le comhad Potx le C#"
head_description: "Cuir Image Síniú ar Potx comhad le haghaidh .NET ag baint úsáide as cúpla líne de chód. Úsáid an GroupDocs Document Signature API chun mórán formáidí comhaid a shíniú."

############################# Header ############################
title: "Sínigh Potx comhad le sínithe Image in C#"
description: "Conas Image Síniú a chur leis le cúpla líne de chód .NET"
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
    title: "Maidir le GroupDocs.Signature for .NET API sínithe íomhánna"
    content: |
        Is API coitianta é [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) le haghaidh ríomhshíniú doiciméad digiteach. Tá sínithe amhail téacsanna, íomhánna, teastais dhigiteacha, barrachóid, cóid QR, stampaí nó meiteashonraí ar fáil. D’fhéadfaí sínithe a chur ar PDF, doiciméid MS Word, leabhair oibre MS Excel, láithreoireachtaí MS PowerPoint, comhaid Adobe Photoshop agus formáidí éagsúla íomhá. Is féidir le custaiméirí a ndoiciméad a shíniú agus ríomhshínithe a cuireadh ar na doiciméid sin a nuashonrú, a chuardach, a fhíorú, a scriosadh nó a réamhamharc. Thairis sin, soláthraítear go leor cumais le haghaidh saincheapadh sínithe.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Céimeanna chun Potx a shíniú le Image in C#"
    content_left: |
        Soláthraíonn [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) cumas chun doiciméid Potx a shíniú le sínithe Image go tapa agus go héasca.
        
        * Cruthaigh sampla d'aicme Sínithe ag soláthar Potx comhad atá ceaptha a shíniú mar chonair nó mar shruth cuimhne
        * Cuir rang SignOptions ar bun agus socraigh na sonraí go léir a éilítear.
        * Iarr ar an modh Signature.Sign() aschuir {{ Fileformat}} comhad nó sruth cuimhne a rith

    title_right: " Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Signature for .NET ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.

        * Córais oibriúcháin: Microsoft Windows, Linux, MacOS
        * Timpeallachtaí forbartha: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Faigh an GroupDocs.Signature for .NET is déanaí ó [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Potx file
        string filePath = "input.potx";
        // Set up output file
        string outputFilePath = "output.potx";
        // Provide image file
        string imageFilePath = "image.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
            //Provide sign options
            ImageSignOptions options = new ImageSignOptions(imageFilePath)
            {
                // set signature position
                Left = 50,
                Top = 200
            };

            // sign Potx document
            SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ag síniú Potx doiciméad le {{ Signaturetype}} Taispeántas Beo"
    content: |
       Sínigh Potx comhad le sínithe éagsúla faoi láthair trí chuairt a thabhairt ar an suíomh Gréasáin [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Saor in aisce taispeána ar líne ag fanacht leat.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Sínithe Image eile a dtacaítear leo le haghaidh C#"
    content: |
        "Is féidir leat Potx a shíniú le cineálacha sínithe eile freisin. Féach ar an liosta thíos le do thoil."
    format: 
       
       
back_to_top:
    enable: true
---