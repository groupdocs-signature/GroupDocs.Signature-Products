---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: Aztec
fileformat: Docx
productName: .NET
lang: zh
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on Docx for C#

############################# Head ############################
head_title: "在 C# 中带有 Aztec QR 码的 eSign Docx 文档"
head_description: "创建 Aztec 二维码并使用 .NET 和一小段 C# 代码将其放在 Docx 文件中。使用 GroupDocs 文档签名 API 使用 QR 码对您的业务文档和文件进行电子签名。"

############################# Header ############################
title: "在 C# 中为 Docx 文档生成 Aztec 二维码签名"
description: "使用 Aztec 二维码对您的 Docx 文档和合同进行电子签名。快速轻松地生成二维码签名。"
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
    title: "关于 GroupDocs.Signature for .NET 二维码签名 API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) 是一个成熟的 API，用于为文档创建和生成二维码签名。用户可以生成二维码签名，提供文本下载或作为图像在社交媒体上分享。可以使用 API 或简单地通过移动相机扫描签名的文档！通过添加二维码签名以电子方式签署您的商业合同和官方文件并对其进行操作。任何二维码签名都将包含唯一的自定义信息，以识别签名者或授权文档。此外，二维码内容可以通过个人密钥以编程方式进行加密和解密。这开启了许多在公共文档中共享敏感数据的能力。签名后，用户可以更新、验证、删除、预览或搜索 PDF、MS Word 文档、MS Excel 工作簿、MS PowerPoint 演示文稿、Adobe Photoshop 文件和各种图像格式中的二维码。 QR码可以额外定制。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "在 C# 中使用 Qrcode 签署 Docx 的步骤"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) 提供使用 Qrcode 签名快速轻松地签署 Docx 文档的能力。
        
        * 创建 Signature 类的实例，提供 Docx 文件应该作为路径或内存流进行签名
        * 实例化 SignOptions 类并设置所有需要的数据。
        * 调用 Signature.Sign() 方法传递输出 Docx 文件或内存流

    title_right: " 系统要求"
    content_right: |
        所有主要平台和操作系统都支持 GroupDocs.Signature for .NET。在执行以下代码之前，请确保您的系统上安装了以下先决条件。

        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * 从 [Nuget](https://www.nuget.org/packages/groupdocs.signature) 获取最新的 GroupDocs.Signature for .NET
         
    code: |
        ```csharp    
                
        // Set up input Docx file
        string filePath = "input.docx";
        // Set up output file
        string outputFilePath = "output.docx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined QrCode text
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // setup QrCode encoding type
                    EncodeType = QrCodeTypes.Aztec,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50
                };

                // sign Docx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "使用 Qrcode 现场演示签署 Docx 文档"
    content: |
       访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站，立即使用各种签名为 Docx 文件签名。免费在线演示等着你。

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Aztec QrCode"
          content: |
            Aztec Code 是一种二维 (2-D) 通用矩阵符号，其设计精度高于其他二维符号。一个阿兹特克代码符号最多可以编码 3,832 个数字； 3,067 个字母字符；或 1,914 字节的数据。
          characterset: |
             所有 256 个 ASCII 字符。
          textcapacity: |
             最多 3,832 个数字，或 3,067 个字母字符，或 1,914 个字节的数据。
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAK0AAACtCAYAAADCr/9DAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAALEoAACxKAXd6dE0AAAp7SURBVHhe7ZJBjuA6DsX6/pf+s+KiAc6D2pFcSUEEuCMsO9Gf/5blY+zSLp9jl3b5HLu0y+fYpV0+xy7t8jl2aZfPsUu7fI5d2uVz7NIun2OXdvkcu7TL59ilXT7HLu3yOXZpl8+xS7t8jl3a5XPs0i6fY5d2+Ry7tMvnuLq0f/78aTdhPb4Jux8mrK+YsL7iTa5Os8c+NWE9vgm7Hyasr5iwvuJNrk6zxz41YT2+CbsfJqyvmLC+4k2uTrPHPjVhPb4Jux8mrK+YsL7iTa5Os8c+NWE9vgm7Hyasr5iwvuJNrk6zxz41YT2+CbsfJqyvmLC+4k2uTrPHPjVhPb4Jux8mrK+YsL7iTV7z9+xD4AQ2BxPWf82E9ZiwHruZ2YgD7LE4gc3BhPVfM2E9JqzHbmY24gB7LE5gczBh/ddMWI8J67GbmY04wB6LE9gcTFj/NRPWY8J67GZmIw6wx+IENgcT1n/NhPWYsB67mdmIA+yxOIHNwYT1XzNhPSasx25mNuIAeyxOYHMwYf3XTFiPCeuxm5mN+D/Yg/AUO+upp9hZFRPW45uw+2E3V19uD8JT7KynnmJnVUxYj2/C7ofdXH25PQhPsbOeeoqdVTFhPb4Jux92c/Xl9iA8xc566il2VsWE9fgm7H7YzdWX24PwFDvrqafYWRUT1uObsPthN1dfbg/CU+ysp55iZ1VMWI9vwu6H3Vx9uT0IT7GznnqKnVUxYT2+CbsfdtN+ol36jSasn3QCm4MJ6yveZJdWsH7SCWwOJqyveJNdWsH6SSewOZiwvuJNdmkF6yedwOZgwvqKN9mlFayfdAKbgwnrK95kl1awftIJbA4mrK94k11awfpJJ7A5mLC+4k3uTjvEPtJTE9Zjwnq8jd0BJ7A52M39r3mAfYinJqzHhPV4G7sDTmBzsJv7X/MA+xBPTViPCevxNnYHnMDmYDf3v+YB9iGemrAeE9bjbewOOIHNwW7uf80D7EM8NWE9JqzH29gdcAKbg93c/5oH2Id4asJ6TFiPt7E74AQ2B7u5/zUPsA/x1IT1mLAeb2N3wAlsDnbTfqJdGhPWY8L6dcaE9djNLu1aNmE9drNLu5ZNWI/d7NKuZRPWYze7tGvZhPXYzS7tWjZhPXazS7uWTViP3fSfGLAH4QQ2B38D9q6nJqzHm+zSfhh711MT1uNNdmk/jL3rqQnr8Sa7tB/G3vXUhPV4k13aD2PvemrCerzJLu2HsXc9NWE93mSX9sPYu56asB5v0j7NHvTUU+wsTFj/Uyasx4T1mLC+YjftJ9qln3qKnYUJ63/KhPWYsB4T1lfspv1Eu/RTT7GzMGH9T5mwHhPWY8L6it20n2iXfuopdhYmrP8pE9ZjwnpMWF+xm/YT7dJPPcXOwoT1P2XCekxYjwnrK3bTfqJd+qmn2FmYsP6nTFiPCesxYX3FbtpPtEs/9RQ7CxPW/5QJ6zFhPSasr9hN/4mH2GMrJqzHhPU4gc3BhPUVE9ZjwnrsZuYvHGCPrZiwHhPW4wQ2BxPWV0xYjwnrsZuZv3CAPbZiwnpMWI8T2BxMWF8xYT0mrMduZv7CAfbYignrMWE9TmBzMGF9xYT1mLAeu5n5CwfYYysmrMeE9TiBzcGE9RUT1mPCeuxm5i8cYI+tmLAeE9bjBDYHE9ZXTFiPCeuxm5m/cIA9tmLCekxYjxPYHExYXzFhPSasx25m/sIB9tiKCesxYT0mrMeE9ZiwvuIENge7mXnBAfbYignrMWE9JqzHhPWYsL7iBDYHu5l5wQH22IoJ6zFhPSasx4T1mLC+4gQ2B7uZecEB9tiKCesxYT0mrMeE9ZiwvuIENge7mXnBAfbYignrMWE9JqzHhPWYsL7iBDYHu5l5wQH22IoJ6zFhPSasx4T1mLC+4gQ2B7uZecEB9tiKCesxYT0mrMeE9ZiwvuIENge7aT/RLo0J6zFhfcWE9TiBzcGE9RUT1mPCeuym/US7NCasx4T1FRPW4wQ2BxPWV0xYjwnrsZv2E+3SmLAeE9ZXTFiPE9gcTFhfMWE9JqzHbtpPtEtjwnpMWF8xYT1OYHMwYX3FhPWYsB67aT/RLo0J6zFhfcWE9TiBzcGE9RUT1mPCeuym/US7NCasx4T1FRPW4wQ2BxPWV0xYjwnrsZv2E+3SmLAeE9ZXTFiPE9gcTFhfMWE9JqzHbtpPtEtPmrAeE9b/lAnrJ30Lu7SC9T9lwvpJ38IurWD9T5mwftK3sEsrWP9TJqyf9C3s0grW/5QJ6yd9C7u0gvU/ZcL6Sd/CLq1g/U+ZsH7St3D1JvYhMGH9U38D9q6KCesxYT12c/Xv2YMwYf1TfwP2rooJ6zFhPXZz9e/ZgzBh/VN/A/auignrMWE9dnP179mDMGH9U38D9q6KCesxYT12c/Xv2YMwYf1TfwP2rooJ6zFhPXZz9e/ZgzBh/VN/A/auignrMWE9dnP179mDMGH9U38D9q6KCesxYT1285q/Z4+tmLB+zSasr9jNLu36lwnrK3azS7v+ZcL6it3s0q5/mbC+Yje7tOtfJqyv2M0u7fqXCesrdrNLu/5lwvqK3VxdWnvQU29jd8CE9RUnsDmYsB5vcnWaPfapt7E7YML6ihPYHExYjze5Os0e+9Tb2B0wYX3FCWwOJqzHm1ydZo996m3sDpiwvuIENgcT1uNNrk6zxz71NnYHTFhfcQKbgwnr8SZXp9ljn3obuwMmrK84gc3BhPV4k6vT7LFPvY3dARPWV5zA5mDCerzJ/b9+gH2kSRPW4yl2VsUJbA6+hV1aMWE9nmJnVZzA5uBb2KUVE9bjKXZWxQlsDr6FXVoxYT2eYmdVnMDm4FvYpRUT1uMpdlbFCWwOvoVdWjFhPZ5iZ1WcwObgW9ilFRPW4yl2VsUJbA6+hfab2GMxYT2eYmdVPMXOqpiwHhPW4wQ2B7tpP9EujQnr8RQ7q+IpdlbFhPWYsB4nsDnYTfuJdmlMWI+n2FkVT7GzKiasx4T1OIHNwW7aT7RLY8J6PMXOqniKnVUxYT0mrMcJbA52036iXRoT1uMpdlbFU+ysignrMWE9TmBzsJv2E+3SmLAeT7GzKp5iZ1VMWI8J63ECm4PdtJ9ol8aE9XiKnVXxFDurYsJ6TFiPE9gc7Kb9RLs0nmJnVXwTdr+KCesrJqzHt9B+E3ssnmJnVXwTdr+KCesrJqzHt9B+E3ssnmJnVXwTdr+KCesrJqzHt9B+E3ssnmJnVXwTdr+KCesrJqzHt9B+E3ssnmJnVXwTdr+KCesrJqzHt9B+E3ssnmJnVXwTdr+KCesrJqzHt9B+E3ssnmJnVXwTdr+KCesrJqzHt9B+E3ssvgm7X8UJbE7F29gd8Ca7tP/oBDan4m3sDniTXdp/dAKbU/E2dge8yS7tPzqBzal4G7sD3mSX9h+dwOZUvI3dAW+yS/uPTmBzKt7G7oA32aX9RyewORVvY3fAm7xrk5alwC7t8jl2aZfPsUu7fI5d2uVz7NIun2OXdvkcu7TL59ilXT7HLu3yOXZpl8+xS7t8jl3a5XPs0i6fY5d2+Ry7tMvn2KVdPscu7fI5dmmXz7FLu3yM//77H+JY77gkOjOBAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# 的其他支持的 Qrcode 签名"
    content: |
        "您还可以使用其他签名类型对 Docx 进行签名。请参阅下面的列表。"
    format: 
        
       
back_to_top:
    enable: true
---