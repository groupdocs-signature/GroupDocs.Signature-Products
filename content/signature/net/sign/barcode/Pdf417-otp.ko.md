---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pdf417
fileformat: Otp
productName: .NET
lang: ko
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Otp for C#

############################# Head ############################
head_title: "C#의 Pdf417 바코드로 Otp 문서에 전자 서명"
head_description: "Pdf417 Barcode Signature를 생성하고 몇 줄의 코드를 사용하여 .NET를 사용하여 Otp 문서에 넣습니다. 다양한 파일 형식에 서명하려면 GroupDocs 문서 서명 API를 사용하십시오."

############################# Header ############################
title: "C#에서 Otp 문서에 대한 Pdf417 바코드 서명 생성"
description: "Pdf417 바코드로 Otp 비즈니스 문서에 전자 서명하세요. 서명 옵션을 설정하는 몇 줄의 코드로 빠르고 쉽게 바코드 서명을 생성합니다."
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
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)은 UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN, ITF14와 같은 다양한 바코드 유형을 사용하는 디지털 문서 전자 서명에 널리 사용되는 API입니다. 그리고 많은 다른 사람들. 고객은 원하는 텍스트만 제공하는 바코드를 쉽게 생성하여 PDF, MS Word 문서, MS Excel 통합 문서, MS PowerPoint 프레젠테이션, Adobe Photoshop 파일 및 다양한 이미지 형식에 넣을 수 있습니다. 문서에 배치된 바코드는 업데이트, 검색, 확인, 삭제 또는 미리 볼 수 있습니다. 또한 바코드 사용자 정의가 지원됩니다.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C#에서 Barcode으로 Otp에 서명하는 단계"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)은 Barcode 서명으로 Otp 문서에 빠르고 쉽게 서명할 수 있는 기능을 제공합니다.
        
        * 경로 또는 메모리 스트림으로 서명해야 하는 Otp 파일을 제공하는 Signature 클래스의 인스턴스 생성
        * SignOptions 클래스를 인스턴스화하고 필요한 모든 데이터를 설정합니다.
        * 출력 Otp 파일 또는 메모리 스트림을 전달하는 Signature.Sign() 메서드를 호출합니다.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET을(를) 사용한 문서 서명은 몇 가지 간단한 단계로 수행할 수 있습니다. 당사의 API는 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 전제 조건이 설치되어 있는지 확인하십시오.

        * 운영 체제: Microsoft Windows, Linux, MacOS
        * 개발 환경: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature)에서 최신 GroupDocs.Signature for .NET 가져오기
         
    code: |
        ```csharp    
        
        // Set up input Otp file
        string filePath = "input.otp";
        // Set up output file
        string outputFilePath = "output.otp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Pdf417,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Otp document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Barcode 라이브 데모로 Otp 문서 서명"
    content: |
       지금 바로 [GroupDocs.Signature 앱](https://products.groupdocs.app/signature/family) 웹사이트에서 다양한 서명으로 Otp 파일에 서명하세요. 무료 온라인 데모가 여러분을 기다리고 있습니다.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pdf417 Barcode"
          content: |
            PDF417은 운송, 신분증 및 재고 관리와 같은 다양한 애플리케이션에 사용되는 스택형 선형 바코드 형식입니다.
          characterset: |
             모든 256 ASCII 문자.
          textcapacity: |
             최대 800자입니다.
          image: |
             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n5CyNd2mE6YM3C103eeW7u1GcDbbfbpDbg48fhVus6H3LuXJRLf9hK77TGz77Q7qm05whu1ugne3grPZ7tMdcnPg8atwmw29dylPJrrtJ3TdZ2Lbb3dQ33SCM2x3E7y7FZzNdp/ukJsDj1+F22zovUt5MtFtP6HrPhPbfruD+qYTnGG7m+DdreBstvt0h9wcePwq3GZD713Kk4lu+wld95nY9tsd1Ded4Azb3QTvbgVns92nO+TmwONX4TYbeu9Snkx020/ous/Ett/uoL7pBGfY7iZ4dys4m+0+3SE3Bx6/CrfZ0HuX8mSi235C130mtv12B/VNJzjDdjfBu1vB2Wz36Q65OfD4VbjNZrvn7t735MR2750FZ1Pf1N2Ugbt735MT3ZuN4Gy2+3SH3Bx4/CrcZrPdc3fve3Jiu/fOgrOpb+puysDdve/Jie7NRnA22326Q24OPH4VbrPZ7rm79z05sd17Z8HZ1Dd1N2Xg7t735ET3ZiM4m+0+3SE3Bx6/CrfZbPfc3fuenNjuvbPgbOqbupsycHfve3Kie7MRnM12n+6QmwOPX4XbbLZ77u59T05s995ZcDb1Td1NGbi79z050b3ZCM5mu093yM2Bx6/CbTbbPXf3vicntnvvLDib+qbupgzc3fuenOjebARns92nO+TmwONX4Tab17013eYzkXbOE9s9O++nbOh/awfebwVns92nO+TmwONX4Tab17013eYzkXbOE9s9O++nbOh/awfebwVns92nO+TmwONX4Tab17013eYzkXbOE9s9O++nbOh/awfebwVns92nO+TmwONX4Tab17013eYzkXbOE9s9O++nbOh/awfebwVns92nO+TmwONX4Tab17013eYzkXbOE9s9O++nbOh/awfebwVns92nO+TmwONX4Tab17013eYzkXbOE9s9O++nbOh/awfebwVns92nO+TmwONX4TYbeu+coW6r4LylfqsKzqa++WkHaVe/UXtnqNtqYuqhfutGcDbbfbpDbg48fhVus6H3zhnqtgrOW+q3quBs6pufdpB29Ru1d4a6rSamHuq3bgRns92nO+TmwONX4TYbeu+coW6r4LylfqsKzqa++WkHaVe/UXtnqNtqYuqhfutGcDbbfbpDbg48fhVus6H3zhnqtgrOW+q3quBs6pufdpB29Ru1d4a6rSamHuq3bgRns92n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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "C#에 대해 지원되는 기타 Barcode 서명"
    content: |
        "다른 서명 유형으로 Otp에 서명할 수도 있습니다. 아래 목록을 참조하십시오."
    format: 
           
       
back_to_top:
    enable: true
---