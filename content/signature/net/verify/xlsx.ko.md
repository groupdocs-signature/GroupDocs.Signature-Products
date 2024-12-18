



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:36
draft: false
lang: ko
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "XLSX 디지털 서명 검증 using C#"
head_description: "GroupDocs.Signature for .NET를 활용하여 XLSX 파일에 포함된 서명의 진위를 인증하세요. PDF, Word, Excel, 프레젠테이션, 이미지 및 ZIP 형식의 서명을 검증할 수 있습니다."

############################# Header ############################
title: "XLSX 디지털 서명 검증" 
description: "PDF, Word, Excel, 프레젠테이션, 이미지 또는 ZIP 파일과 같은 여러 형식의 모든 지원되는 전자 서명을 효율적으로 확인할 수 있습니다. GroupDocs.Signature for .NET의 종합적인 기능을 통해 가능합니다."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 버전 다운로드"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET의 주요 응용 프로그램"
    link: "/signature/net/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/)는 문서 서명 관리에 대한 완전한 CRUD 기능을 지원합니다. PDFs, MS Office 파일, 이미지 및 ZIP 아카이브를 포함하여 60가지 이상의 다양한 형식에 서명할 수 있으며, 텍스트, 이미지, 바코드, 디지털 인증서, 메타데이터 및 스탬프와 같은 다양한 서명 유형을 사용할 수 있습니다. 서명 추가 외에도 서명을 검색, 검증, 업데이트 또는 제거할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "C#를 사용한 XLSX의 서명 검증 가이드"
    content: |
      [GroupDocs.Signature](/signature/net/)는 XLSX 문서 내 특정 서명의 존재를 인증할 수 있습니다. .NET 개발자는 우리 솔루션이 제공하는 기능을 통합하여 애플리케이션을 손쉽게 향상시킬 수 있습니다.
      
      1. Signature 인스턴스에 XLSX 파일을 로드합니다.
      2. 원하는 검증 결과를 달성하기 위해 VerifyOptions를 인스턴스화하고 구성합니다.
      3. 검증 프로세스를 시작합니다.
      4. 검증 결과를 검토하고 해석합니다.
   
    code:
      platform: "net"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "샘플 서명"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "클릭하여 복사"
        copy_done: "복사됨"
      links:
        #  loop
        - title: "더 많은 예제"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "문서"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // 문서와 함께 Signature 인스턴스를 초기화합니다.
        using (Signature signature = new Signature("input.xlsx"))
        {
            // 특정 텍스트를 포함한 서명을 인증하기 위해 TextVerifyOptions를 설정합니다.
            TextVerifyOptions options = new TextVerifyOptions()
            {
                Text = "signature",
                MatchType = TextMatchType.Contains
            };

            // 문서의 서명 검증을 수행합니다.
            VerificationResult result = signature.Verify(options);

            // 검증 결과를 분석하고 해석합니다.
            if(result.IsValid)
            {
                Console.WriteLine($"\nDocument was verified successfully!");
                foreach (TextSignature item in result.Succeeded)
                {
                    Console.WriteLine($"\nValid signature is found with text: {item.Text}");
                }
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "고급 문서 서명"
  description: "GroupDocs.Signature는 널리 사용되는 형식에서 문서 서명 및 인증 프로세스를 간소화하려는 포괄적인 솔루션입니다. 7가지 서명 유형과 전체 CRUD 작업을 제공하여 문서 콘텐츠의 포괄적인 보호 및 관리를 보장합니다."
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "서명 검증 기능"
  features:
    # feature loop
    - title: "기업 문서 서명 간소화"
      content: "문서의 원하는 섹션에 맞춤형 디지털 서명을 매끄럽게 적용할 수 있습니다. 텍스트, 이미지, 바코드, 메타데이터, 스탬프 및 디지털 인증서 서명을 지원하는 GroupDocs.Signature for .NET는 귀하의 문서가 기업 표준에 부합하도록 보장합니다."

    # feature loop
    - title: "전체 서명 생애주기 관리"
      content: "문서 내 서명의 전체 생애주기를 쉽게 관리할 수 있습니다. 필요할 때마다 서명에 접근하고, 검증하고, 업데이트하거나 제거하여 문서가 최신 상태이도록 합니다."

    # feature loop
    - title: "문서 내용 무결성 보호"
      content: "무단 변경을 방지하는 디지털 인증서를 삽입하여 민감한 문서를 보호합니다. 또한, 중요한 정보를 보호하고 내용 무결성을 보장하기 위해 숨겨진 메타데이터를 추가할 수 있습니다."

    # feature loop
    - title: "맞춤형 기본 서명"
      content: "PDF 스탬프 및 Word 워터마크와 같은 문서별 서명 유형을 활용하세요. 이러한 맞춤형 서명은 브랜딩, 워터마킹 또는 규정 준수를 위한 최적의 선택이며, 전문적인 느낌을 제공하여 기업 문서의 품질을 높입니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "바코드 서명 검증"
      content: |
        이 예제는 문서 내 바코드 서명을 인증하는 절차를 설명합니다.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          using (Signature signature = new Signature("input.xlsx"))
          {
              // 특정 텍스트 기준에 맞춰 바코드를 검증하기 위한 옵션을 구성합니다.
              BarcodeVerifyOptions options = new BarcodeVerifyOptions()
              {
                    Text = "12345",
                    MatchType = TextMatchType.StartsWith
              };

              // 문서에 포함된 서명을 인증합니다.
              VerificationResult result = signature.Verify(options);

              // 인증 프로세스의 결과를 제시합니다.
              if (result.IsValid)
              {
                  Console.WriteLine($"\nDocument was verified successfully!");
                  foreach (BarcodeSignature item in result.Succeeded)
                  {
                      Console.WriteLine($"\nValid signature is found with text: {item.Text} 
                            and type: {item.EncodeType.TypeName}.");
                  }
              }
          }
          ```
        platform: "net"
        copy_title: "복사"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "클릭하여 복사"
          copy_done: "복사됨"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "문서"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Signature의 기능을 무료로 시도하거나 라이센스를 요청하세요."
  items:
    #  loop
    - title: "Nuget 다운로드"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "라이센스 구매"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "포괄적인 작업 및 서명 유형"
    exclude: "verify"
    description: "GroupDocs.Signature와 함께 제공되는 방대한 기능 및 서명 관리 작업을 탐색하여 문서의 서명 프로세스를 완벽하게 제어하세요."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/net/esign/xlsx/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/net/text/xlsx/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/net/image/xlsx/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/net/barcode/xlsx/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/net/qrcode/xlsx/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/net/digital/xlsx/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/net/stamp/xlsx/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/net/search/xlsx/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/net/verify/xlsx/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/net/modify/xlsx/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/net/delete/xlsx/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "형식 간 서명 검증"
    exclude: "XLSX"
    description: "GroupDocs.Signature for .NET를 사용하여 다양한 문서 형식에서 서명을 효율적으로 검증할 수 있습니다. 문서의 무결성과 규정 준수를 보장하기 위해 맞춤형 검증 매개변수를 설정하세요."
    items: 
          
        # format loop 1
        - name: "PDF 서명 검증"
          format: "PDF"
          link: "/signature/net/verify/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX 서명 검증"
          format: "DOCX"
          link: "/signature/net/verify/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "PPTX 서명 검증"
          format: "PPTX"
          link: "/signature/net/verify/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX 서명 유효성 검사"
          format: "XLSX"
          link: "/signature/net/verify/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---