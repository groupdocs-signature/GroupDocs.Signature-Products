



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:33
draft: false
lang: ko
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "XLSX 전자 서명 검색을 위한 Python"
head_description: "GroupDocs.Signature for Python via .NET API를 활용하여 PDF, Word, Excel, 프레젠테이션 및 이미지와 같은 형식에 내장된 전자 서명을 검색하세요."

############################# Header ############################
title: "XLSX 디지털 서명 검색" 
description: "GroupDocs.Signature for Python via .NET의 힘으로 PDF, Word, Excel, 프레젠테이션 및 이미지를 포함한 여러 형식에서 전자 서명의 전체 목록을 추출할 수 있습니다."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "지금 다운로드"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Python via .NET의 잠재력을 발휘하세요"
    link: "/signature/python-net/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/)는 디지털 문서 서명 및 관리에 대한 고급 기능을 제공합니다. PDF, Office 문서, 이미지 및 ZIP 파일을 포함한 60개 이상의 파일 형식을 지원하며, 텍스트, 이미지, 바코드, QR 코드, 디지털 인증서 및 스탬프와 같은 서명을 추가, 검색, 검증, 수정 또는 제거할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "Python를 사용하여 XLSX에서 서명을 검색하는 방법"
    content: |
      [GroupDocs.Signature](/signature/python-net/)는 XLSX 파일에서 디지털 서명을 감지하기 위한 강력한 엔진을 제공합니다. Python via .NET 개발자는 이 기능을 사용하여 자신의 앱을 쉽게 강화할 수 있습니다.
      
      1. 서명을 검색할 XLSX 파일 경로를 제공합니다.
      2. SearchOptions를 사용하여 검색 기준을 조정합니다.
      3. 결과를 검색하기 위해 Search 메서드를 호출합니다.
      4. 확인된 서명의 목록을 검토합니다.
   
    code:
      platform: "python-net"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "샘플 서명"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "클릭하여 복사"
        copy_done: "복사됨"
      links:
        #  loop
        - title: "더 많은 예제"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "문서"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Signature 객체를 문서의 파일 경로로 초기화합니다
            with sg.Signature('input.xlsx') as signature:

                # TextSearchOptions의 인스턴스를 생성하여 모든 페이지를 검색합니다
                options = sg.TextSearchOptions()
                options.AllPages = True

                # 문서에서 텍스트 기반 서명을 찾기 위해 검색을 실행합니다
                signatures = signature.Search(options)
                print("\nSource document contains following text signature(s).")

                # 상세 검토를 위해 발견된 서명의 목록을 컴파일합니다
                for textSignature in signatures:
                    print("\nFound Text signature at page ", textSignature.PageNumber)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "종합 문서 서명 플랫폼"
  description: "다양한 파일 형식에 걸쳐 여러 서명 유형으로 문서를 보호하는 강력하고 기능이 풍부한 서명 솔루션을 경험하세요."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "서명 검색 및 관리"
  features:
    # feature loop
    - title: "비즈니스 문서에 서명 및 보호"
      content: "문서의 어디에나 전자 서명을 추가하세요. GroupDocs.Signature는 텍스트, 이미지, 바코드, 메타데이터, 스탬프 및 디지털 인증서를 포함한 다양한 서명 유형을 지원하여 문서의 진위성과 보안을 보장합니다."

    # feature loop
    - title: "종합적인 서명 관리"
      content: "문서에 서명한 후, 검색 기능을 사용하여 모든 내장된 서명을 찾을 수 있습니다. 필요에 따라 서명을 수정하거나 제거할 수 있어 문서의 무결성을 완전히 제어할 수 있습니다."

    # feature loop
    - title: "문서 무결성 보장"
      content: "문서 내의 숨겨진 메타데이터를 관리하기 위한 고급 도구를 사용하세요. 메타데이터를 추가하거나 제거하고, 디지털 인증서를 적용하여 문서가 무단 변경으로부터 보호되도록 하여 그 진정성을 확보합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "이미지 서명 검색"
      content: |
        이 예시는 특정 문서 내에서 이미지 서명을 찾는 방법을 보여줍니다.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # 소스 문서를 생성자에 전달합니다
              with sg.Signature('input.xlsx') as signature:

                    # 텍스트 기반 서명을 검색합니다
                    signatures = signature.Search(sg.SignatureType.Image)
                    print("\nSource document contains following image signature(s).")

                    # 확인된 서명의 상세 속성을 표시합니다
                    for imageSignature in signatures:
                        print("\nFound image signature at page ", imageSignature.PageNumber)
          ```
        platform: "python-net"
        copy_title: "복사"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "클릭하여 복사"
          copy_done: "복사됨"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "문서"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Signature의 기능을 무료로 시도하거나 라이센스를 요청하세요."
  items:
    #  loop
    - title: "PyPi 다운로드"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "라이센스 구매"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "핵심 기능"
    exclude: "search"
    description: "저희 API는 사용자가 문서에 서명하고 서명을 검색, 검증 및 편집과 같은 후속 작업을 수행할 수 있는 폭넓은 유연성을 제공합니다."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/python-net/esign/xlsx/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/python-net/text/xlsx/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/python-net/image/xlsx/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/python-net/barcode/xlsx/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/python-net/digital/xlsx/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/python-net/stamp/xlsx/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/python-net/search/xlsx/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/python-net/verify/xlsx/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/python-net/modify/xlsx/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/python-net/delete/xlsx/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 파일 형식에서 서명 추출"
    exclude: "XLSX"
    description: "GroupDocs.Signature for Python via .NET API는 다양한 문서 형식에서 서명을 추출하고 관리할 수 있도록 합니다. 주요 파일 유형에서 내장된 서명을 쉽게 검색하여 추가 분석 또는 처리를 수행할 수 있습니다."
    items: 
          
        # format loop 1
        - name: "PDF에서 서명 검색"
          format: "PDF"
          link: "/signature/python-net/search/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에서 서명 찾기"
          format: "DOCX"
          link: "/signature/python-net/search/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "PPTX에서 서명 찾기"
          format: "PPTX"
          link: "/signature/python-net/search/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX에서 서명 검색"
          format: "XLSX"
          link: "/signature/python-net/search/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---