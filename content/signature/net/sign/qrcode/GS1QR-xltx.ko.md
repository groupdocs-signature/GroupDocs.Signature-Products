---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: G S1 Q R
fileformat: Xltx
productName: .NET
lang: ko
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on Xltx for C#

############################# Head ############################
head_title: "C#의 G S1 Q R QR 코드로 Xltx 문서에 전자 서명"
head_description: "짧은 C# 코드와 함께 .NET을(를) 사용하여 G S1 Q R QR 코드를 생성하고 Xltx 파일에 넣습니다. GroupDocs 문서 서명 API를 사용하여 QR 코드로 비즈니스 문서 및 파일에 전자 서명하십시오."

############################# Header ############################
title: "C#에서 Xltx 문서에 대한 G S1 Q R QR 코드 서명 생성"
description: "G S1 Q R QR 코드로 Xltx 문서 및 계약에 전자 서명합니다. QR 코드 서명을 빠르고 쉽게 생성합니다."
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
    title: "GroupDocs.Signature for .NET API 정보"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)은 QR 코드를 사용한 디지털 문서 전자 서명을 위한 성숙한 API입니다. 사용자는 요청된 텍스트를 제공하는 QR 코드 서명을 생성하여 다운로드하거나 이미지로 소셜 미디어에 공유할 수 있습니다. 서명된 문서는 API 또는 모바일 카메라를 통해 간단히 스캔할 수 있습니다! QR 코드 서명을 추가하여 비즈니스 계약 및 공식 문서에 전자 서명하고 조작하십시오. 모든 QR 코드 서명에는 서명자를 식별하거나 문서를 승인하는 고유한 사용자 지정 정보가 포함됩니다. 또한 QR 코드 콘텐츠는 프로그래밍 방식으로 개인 키로 암호화 및 해독할 수 있습니다. 이는 공개 문서 내에서 민감한 데이터를 공유할 수 있는 많은 기능을 제공합니다. 서명 후 사용자는 PDF, MS Word 문서, MS Excel 통합 문서, MS PowerPoint 프레젠테이션, Adobe Photoshop 파일 및 다양한 이미지 형식 내에서 QR 코드를 업데이트, 확인, 삭제, 미리보기 또는 검색할 수 있습니다. QR 코드는 추가로 사용자 정의할 수 있습니다.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C#에서 Qrcode으로 Xltx에 서명하는 단계"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)은 Qrcode 서명으로 Xltx 문서에 빠르고 쉽게 서명할 수 있는 기능을 제공합니다.
        
        * 경로 또는 메모리 스트림으로 서명해야 하는 Xltx 파일을 제공하는 Signature 클래스의 인스턴스 생성
        * SignOptions 클래스를 인스턴스화하고 필요한 모든 데이터를 설정합니다.
        * 출력 Xltx 파일 또는 메모리 스트림을 전달하는 Signature.Sign() 메서드를 호출합니다.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET을(를) 사용한 문서 서명은 몇 가지 간단한 단계로 수행할 수 있습니다. 당사의 API는 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 전제 조건이 설치되어 있는지 확인하십시오.

        * 운영 체제: Microsoft Windows, Linux, MacOS
        * 개발 환경: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature)에서 최신 GroupDocs.Signature for .NET 가져오기
         
    code: |
        ```csharp    
                
        // Set up input Xltx file
        string filePath = "input.xltx";
        // Set up output file
        string outputFilePath = "output.xltx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined QrCode text
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // setup QrCode encoding type
                    EncodeType = QrCodeTypes.G S1 Q R,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50
                };

                // sign Xltx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Qrcode 라이브 데모로 Xltx 문서 서명"
    content: |
       지금 바로 [GroupDocs.Signature 앱](https://products.groupdocs.app/signature/family) 웹사이트에서 다양한 서명으로 Xltx 파일에 서명하세요. 무료 온라인 데모가 여러분을 기다리고 있습니다.

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About G S1 Q R QrCode"
          content: |
            GS1 QR 코드는 GS1 사양을 준수하는 QR 코드의 변형입니다. 로트 번호, 제품 ID 및 수량과 같은 확장된 포장 정보를 공유하기 위해 특별히 설계되었습니다.
          characterset: |
             대문자 및 소문자 및 특수 문자 $%*+-./: 모두 올바른 애플리케이션 식별자 포함
          textcapacity: |
             최대 7089자의 숫자, 4296자의 영숫자
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "C#에 대해 지원되는 기타 Qrcode 서명"
    content: |
        "다른 서명 유형으로 Xltx에 서명할 수도 있습니다. 아래 목록을 참조하십시오."
    format: 
        
       
back_to_top:
    enable: true
---