



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:06
draft: false
lang: ko
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "JPEG용 바코드 생성하기 C# API 사용"
head_description: "C#를 사용하여 바코드 서명을 생성하고 JPEG 문서를 몇 줄의 코드로 안전하게 보호하세요. 다양한 파일 형식에 대한 서명에 GroupDocs.Signature을 활용하세요."

############################# Header ############################
title: "JPEG 문서의 바코드 생성하기" 
description: "GroupDocs.Signature for .NET를 사용하여 비즈니스 문서 내 어디에나 바코드를 배치하세요. 저희 API는 바코드 서명에 대한 광범위한 커스터마이징 옵션을 제공합니다."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 다운로드"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET 개요"
    link: "/signature/net/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/)는 텍스트, 이미지, 바코드, 디지털 인증서 및 도장을 포함한 다양한 서명 유형을 지원하는 정교한 문서 서명 솔루션입니다. PDF, MS Office, 이미지, ZIP 파일 등 60개 이상의 파일 형식과 호환되는 이 도구는 서명 적용뿐만 아니라 필요에 따라 검색, 검증, 수정 또는 제거할 수 있게 합니다.

############################# Steps ############################
steps:
    enable: true
    title: "JPEG 파일에 바코드를 생성하고 삽입하기 위한 단계"
    content: |
      [GroupDocs.Signature](/signature/net/)는 여러 인기 형식에서 바코드를 생성하고 JPEG 페이지에 배치할 수 있습니다. 60개 이상의 바코드 유형을 지원하며, .NET 애플리케이션은 저희 라이브러리를 통합하여 바코드 서명 기능을 손쉽게 추가할 수 있습니다.
      
      1. JPEG 파일 또는 스트림을 처리하도록 제공하세요.
      2. BarcodeSignOptions 인스턴스에 바코드 텍스트를 전달하세요.
      3. 위치, 크기 등의 바코드 옵션을 조정하세요.
      4. 새로 추가된 바코드와 함께 파일을 저장하세요.
   
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
        // 문서 경로로 새 Signature 객체 인스턴스화
        using (Signature signature = new Signature("input.jpeg"))
        {
            // BarcodeSignOptions를 사용하여 문서에 바코드 추가
            BarcodeSignOptions options = new BarcodeSignOptions("Business data")
            {
                // 바코드 유형 및 추가 속성 설정
                EncodeType = BarcodeTypes.Code128,
                Left = 50,
                Top = 150
            };

            // 서명된 파일 저장
            SignResult result = signature.Sign("output.jpeg", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "고급 서명 기능으로 문서를 강화하고 보호하세요"
  description: "GroupDocs.Signature for .NET 라이브러리는 널리 사용되는 파일 형식 전반에 걸쳐 포괄적인 문서 서명 및 처리 기능을 제공하도록 설계되었습니다. 다양한 유형의 서명을 추가, 조정, 검증 또는 제거할 수 있습니다."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "GroupDocs.Signature의 주요 기능"
  features:
    # feature loop
    - title: "다양한 문서 서명"
      content: "텍스트, 이미지, 바코드, QR 코드 또는 도장을 사용하여 지원되는 문서 내 어느 페이지에서나 효율적으로 서명하세요. 또한 이미지의 EXIF 데이터와 같은 숨겨진 메타데이터를 삽입하거나, 디지털 인증서를 이용해 문서 콘텐츠를 무단 수정으로부터 보호할 수 있습니다."

    # feature loop
    - title: "포괄적인 서명 검색 및 검증"
      content: "저희 도구는 서명된 문서 작업을 위한 강력한 기능을 제공합니다. 서명을 검증하여 문서의 무결성을 확인하고, 검색 기능을 통해 문서 내 모든 서명의 포괄적인 목록을 쉽게 검색할 수 있습니다."

    # feature loop
    - title: "서명을 손쉽게 수정"
      content: "이전에 적용된 거의 모든 서명은 수정이 가능합니다. 필요에 맞게 텍스트를 업데이트하고, 위치를 조정하거나 색상을 변경하세요."

    # feature loop
    - title: "효율적인 서명 삭제"
      content: "저희 접근 방식은 서명에 대한 CRUD 작업을 완벽하게 지원하여 원치 않거나 구식의 서명을 문서에서 신속하게 제거할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "바코드 서명 생성하기"
      content: |
        이 예제는 JPEG 문서 페이지에 사용자 정의 바코드를 삽입하는 방법을 보여줍니다.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          using (Signature signature = new Signature("input.jpeg"))
          {
              // 원하는 텍스트로 서명 옵션 설정
              BarcodeSignOptions options = new BarcodeSignOptions("Accepted")
              {
                  EncodeType = BarcodeTypes.Code39FullASCII,

                  // 페이지에서 바코드의 상대적인 위치 결정
                  VerticalAlignment = Domain.VerticalAlignment.Top,
                  HorizontalAlignment = Domain.HorizontalAlignment.Left,

                  // 페이지 가장자리에서 바코드 여백 정의
                  Margin = new Padding() { Top = 180, Right = 20 },

                  // 막대의 색상 지정
                  ForeColor = Color.Red,

                  // 메시지 글씨체 스타일 선택
                  Font = new SignatureFont { Size = 12, FamilyName = "Arial" },

                  // 메시지 위치 표시
                  CodeTextAlignment = CodeTextAlignment.Above
              };

              // 문서 서명 및 저장
              SignResult result = signature.Sign("output.jpeg", options);
          }
          ```
        platform: "net"
        copy_title: "복사"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "클릭하여 복사"
          copy_done: "복사됨"
        top_links:
          #  loop
          - title: "결과 다운로드"
            icon: "download"
            link: "/examples/signature/formats/signature_barcode.jpeg"
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
    title: "주요 기능 알아보기"
    exclude: "barcode"
    description: "저희는 인상적인 서명 옵션과 작업을 제공합니다."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/net/esign/jpeg/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/net/text/jpeg/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/net/image/jpeg/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/net/barcode/jpeg/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/net/qrcode/jpeg/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/net/stamp/jpeg/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/net/search/pdf/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/net/verify/pdf/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/net/modify/pdf/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/net/delete/pdf/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 형식의 문서 서명"
    exclude: "JPEG"
    description: "저희 .NET API는 60개 이상의 다양한 형식의 서명을 지원합니다. 문서 내에서 페이지의 어떤 위치에도 다양한 유형의 서명을 손쉽게 배치하세요."
    items: 
          
        # format loop 1
        - name: "PDF에 바코드 추가"
          format: "PDF"
          link: "/signature/net/barcode/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에 바코드 추가"
          format: "DOCX"
          link: "/signature/net/barcode/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "JPEG에 바코드 추가"
          format: "JPEG"
          link: "/signature/net/barcode/jpeg/"
          description: "JPEG 이미지"
          
        # format loop 4
        - name: "PPTX에 바코드 추가"
          format: "PPTX"
          link: "/signature/net/barcode/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 5
        - name: "XLSX에 바코드 추가"
          format: "XLSX"
          link: "/signature/net/barcode/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---