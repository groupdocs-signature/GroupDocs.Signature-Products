



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:19
draft: false
lang: ko
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Python를 사용하여 DOCX에 디지털 서명 생성하기"
head_description: "Python를 사용하여 DOCX 문서에 디지털 서명을 추가하는 데 필요한 몇 줄의 코드로 가능합니다. 다양한 파일 형식을 서명하기 위해 GroupDocs.Signature for Python via .NET을(를) 사용하세요."

############################# Header ############################
title: "DOCX에 디지털 서명하기" 
description: "GroupDocs.Signature for Python via .NET을(를) 통해 디지털 인증서를 적용하여 문서의 보안성과 진위를 보장하세요. 우리의 솔루션은 강력한 도구를 사용하여 문서를 서명하고 보호할 수 있습니다."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 체험하기"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Python via .NET란?"
    link: "/signature/python-net/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/)는 다양한 문서 처리 작업을 지원하는 종합 서명 도구입니다. 텍스트, 이미지, 디지털 인증서 및 스탬프를 60개 이상의 파일 형식—PDF, MS Office 파일, 이미지 및 ZIP—에 추가할 수 있습니다. GroupDocs.Signature for Python via .NET을(를) 사용하면 필요할 때마다 서명을 검색, 확인, 업데이트 또는 제거할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "Python에서 DOCX를 디지털 인증서로 보호하는 방법"
    content: |
      [GroupDocs.Signature](/signature/python-net/)는 Python via .NET 개발자가 DOCX 파일에 디지털 서명을 추가하여 보호할 수 있도록 돕습니다. 강력한 문서 보호 기능으로 비즈니스 애플리케이션을 강화하세요.
      
      1. Signature 클래스로 DOCX 파일을 로드합니다.
      2. 파일을 보호하기 위해 디지털 인증서와 해당 비밀번호를 적용합니다.
      3. 문서 페이지에 디지털 서명의 시각적 표시를 추가할 수 있습니다.
      4. 무단 변경을 방지하기 위해 문서에 서명하세요.
   
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

            # 문서를 디지털 서명하기 위해 Signature를 사용하세요
            with sg.Signature('input.docx') as signature:

                # 디지털 인증서와 해당 비밀번호 입력하기
                options = sg.DigitalSignOptions("certificate.pfx")
                options.Password = "1234567890"

                # 서명의 모양을 구성할 수 있습니다
                options.PageNumber = 1
                options.Left = 50
                options.Top = 50

                # 디지털 인증서로 문서를 마무리하세요
                result = signature.Sign("output.docx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "디지털 서명으로 문서를 향상하고 보호하기"
  description: "GroupDocs.Signature for Python via .NET 라이브러리는 모든 주요 파일 형식에 서명하기 위해 설계되었습니다. 다양한 유형의 서명을 추가, 검증, 업데이트 또는 제거하여 작업 흐름을 간소화하세요."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "GroupDocs.Signature의 핵심 기능"
  features:
    # feature loop
    - title: "문서에 서명 추가"
      content: "지원되는 문서의 정확한 위치에 텍스트, 이미지, 바코드, QR 코드 또는 스탬프 서명을 삽입하세요. 문서의 무결성을 보장하기 위해 EXIF와 같은 숨겨진 메타데이터를 관리할 수도 있습니다."

    # feature loop
    - title: "서명 검증 및 검색"
      content: "서명이 완료된 후, 문서의 정상 동작을 확인할 수 있습니다. 강력한 검색 기능을 통해 파일 내 모든 서명을 검색하고 관리하세요."

    # feature loop
    - title: "기존 서명 수정"
      content: "대부분의 서명은 완전히 커스터마이즈 가능합니다. 필요에 맞게 텍스트를 편집하고, 요소를 이동하고, 색상을 변경하며, 크기를 조절할 수 있습니다."

    # feature loop
    - title: "불필요한 서명 제거"
      content: "우리의 솔루션은 서명 관리 기능을 완벽하게 지원하여 필요에 따라 문서에서 서명, 디지털 인증서를 삭제할 수 있습니다."
      
  code_samples:
    # code sample loop
    - title: "디지털 서명으로 문서 보호하기"
      content: |
        무단 수정 방지를 위해 디지털 서명을 적용하여 문서를 보호하는 방법을 알아보세요.
        {{< landing/code title="C#">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # 서명할 문서를 로드합니다
            with sg.Signature('input.docx') as signature:

                # 유효한 디지털 인증서와 해당 비밀번호를 사용합니다
                options = sg.DigitalSignOptions("certificate.pfx")
                options.Password = "1234567890"

                # 필요 시 추가적인 텍스트 정보를 추가합니다
                options.Reason = "Security issue"
                options.Contact = "John Smith"
                options.Location = "Office D.W."

                # 서명의 시각적 표현을 위한 이미지 또는 기타 옵션을 포함합니다
                options.ImageFilePath = "image.png"
                options.AllPages = True
                options.VerticalAlignment = sg.VerticalAlignment.Center
                options.HorizontalAlignment = sg.HorizontalAlignment.Left
                options.Width = 60
                options.Height = 80

                options.Margin = sg.Padding()
                options.Margin.Bottom = 10
                options.Margin.Right = 10

                # 서명된 문서를 안전한 위치에 저장합니다
                result = signature.Sign("output.docx", options)
        ```
        {{< /landing/code >}}


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
    title: "핵심 기능 탐색하기"
    exclude: "digital"
    description: "우리는 강력한 문서 작업 및 다양한 서명 옵션을 제공합니다."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/python-net/esign/docx/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/python-net/text/docx/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/python-net/image/docx/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/python-net/barcode/docx/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/docx/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/python-net/digital/docx/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/python-net/stamp/docx/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/python-net/search/docx/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/python-net/verify/docx/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/python-net/modify/docx/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/python-net/delete/docx/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 형식의 문서 서명"
    exclude: "DOCX"
    description: "Python via .NET API를 사용하면 60개 이상의 다양한 형식을 처리하고, 서명을 추가하고, 보안을 위해 디지털 인증서를 적용하며, 여러 페이지에서 서명을 관리할 수 있습니다."
    items: 
          
        # format loop 1
        - name: "PDF 보호"
          format: "PDF"
          link: "/signature/python-net/digital/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX 보호"
          format: "DOCX"
          link: "/signature/python-net/digital/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "PPTX 보호"
          format: "PPTX"
          link: "/signature/python-net/digital/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX 보호"
          format: "XLSX"
          link: "/signature/python-net/digital/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---