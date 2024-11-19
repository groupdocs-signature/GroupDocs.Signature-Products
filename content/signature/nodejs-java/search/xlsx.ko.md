



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:33
draft: false
lang: ko
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScript을(를) 이용한 XLSX 파일에서 전자 서명 검색"
head_description: "GroupDocs.Signature for Node.js via Java API의 강력한 기능을 활용하여 PDF, Word 문서, Excel 스프레드시트, 프레젠테이션 및 이미지 전반에 걸쳐 전자 서명을 감지하고 검색하세요."

############################# Header ############################
title: "XLSX에서 전자 서명 검색" 
description: "GroupDocs.Signature for Node.js via Java에서 제공하는 고급 도구를 사용하여 PDF, Word, Excel, 프레젠테이션 및 이미지 파일에 포함된 모든 서명에 대한 자세한 정보를 발견하고 검색하세요."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 시작하기"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java 개요"
    link: "/signature/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)은 다양한 파일 형식에서 디지털 서명을 관리할 수 있는 견고한 프레임워크를 제공합니다. PDF, Microsoft Office 문서, 이미지 및 ZIP 파일 등 60개 이상의 형식을 지원하는 이 API는 사용자에게 텍스트, 이미지, 바코드, 디지털 인증서 등 다양한 서명 유형을 적용, 탐색, 검증, 업데이트 또는 제거할 수 있는 기능을 제공합니다.

############################# Steps ############################
steps:
    enable: true
    title: "JavaScript을(를) 이용한 XLSX에서 서명 검색 가이드"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)은(는) XLSX 파일 내에서 디지털 서명을 찾기 위한 강력한 도구입니다. Node.js via Java 개발자는 저희 솔루션을 통해 손쉽게 애플리케이션 기능을 확장할 수 있습니다.
      
      1. XLSX 파일 경로를 지정하여 서명 검색을 시작합니다.
      2. SearchOptions를 사용하여 검색 결과를 필터링합니다.
      3. Search 메서드를 실행하여 서명을 찾습니다.
      4. 발견된 서명 목록을 검토합니다.
   
    code:
      platform: "nodejs-java"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "샘플 서명"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "클릭하여 복사"
        copy_done: "복사됨"
      links:
        #  loop
        - title: "더 많은 예제"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "문서"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // 문서 경로를 사용하여 Signature 객체를 인스턴스화합니다.
        const signature = new signatureLib.Signature('input.xlsx');

        // TextSearchOptions를 구성하여 모든 페이지를 포함시킵니다.
        const options = new signatureLib.TextSearchOptions();
        options.setAllPages(true);

        // 문서 내 모든 텍스트 서명을 찾기 위해 검색을 수행합니다.
        const signatures = signature.search(signatureLib.TextSignature.class, options).toArray();
        console.log(`\nSource document contains the following text signature(s).`);

        // 발견된 서명을 집계하여 포괄적으로 분석합니다.
        for (const textSignature of signatures) {
            console.log(`Found Text signature at page ${textSignature.getPageNumber()} 
            with type [${textSignature.getSignatureImplementation()}] and text '${textSignature.getText()}'.`);
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "완전한 서명 관리 솔루션"
  description: "GroupDocs.Signature for Node.js via Java은(는) 인기 문서 형식에서 전자 서명을 추가, 수정, 검색 및 검증할 수 있는 올인원 솔루션을 제공합니다. 고급 문서 서명 기능으로 작업 흐름을 강화하세요."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "서명 감지 기능"
  features:
    # feature loop
    - title: "비즈니스 파일에 디지털 서명하기"
      content: "문서 내의 위치에 텍스트, 이미지, 바코드 및 디지털 인증서와 같은 전자 서명을 추가하세요. GroupDocs.Signature는 PDF, Word, Excel, 이미지 등에서 서명을 지원하여 유연한 문서 관리를 보장합니다."

    # feature loop
    - title: "효율적인 서명 관리"
      content: "서명한 후, 문서 내에 포함된 모든 서명을 쉽게 찾을 수 있습니다. 이 API는 서명을 포괄적으로 검색하고 검색할 수 있는 기능을 제공하며, 서명을 업데이트하거나 제거할 수 있는 기능도 포함되어 있습니다."

    # feature loop
    - title: "문서 보안 및 메타데이터 관리"
      content: "숨겨진 메타데이터를 포함하거나 제거하여 문서의 무결성을 보호하세요. 디지털 인증서를 이용해 문서 내용을 봉인하고 인증하여 무단 변경으로부터 파일을 보호하십시오."
      
  code_samples_ext:
    # code sample ext loop
    - title: "이미지 서명 식별"
      content: |
        이 예제는 특정 문서 내에서 이미지 서명을 감지하는 방법을 설명합니다.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 소스 문서를 생성자에 매개변수로 제공합니다.
          const signature = new signatureLib.Signature('input.xlsx');

          // 텍스트 유형의 서명을 검색합니다.
          const signatures = signature.search(signatureLib.ImageSignature.class, signatureLib.SignatureType.Image).toArray();
          console.log(`\nSource document contains the following image signature(s).`);

          // 발견된 서명의 종합적인 속성과 함께 결과를 표시합니다.
          for (const imageSignature of signatures) {
              console.log(`Found Image signature at page ${imageSignature.getPageNumber()} 
              and size ${imageSignature.getSize()}.`);
          }
          ```
        platform: "nodejs-java"
        copy_title: "복사"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "클릭하여 복사"
          copy_done: "복사됨"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "문서"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Signature의 기능을 무료로 시도하거나 라이센스를 요청하세요."
  items:
    #  loop
    - title: "NPM 다운로드"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "라이센스 구매"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "주요 기능"
    exclude: "search"
    description: "저희 포괄적인 API는 서명부터 후처리 및 검증까지 문서 서명 관리를 간소화하기 위한 다양한 작업을 제공합니다."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 파일 형식에서 서명 찾기"
    exclude: "XLSX"
    description: "GroupDocs.Signature for Node.js via Java API를 사용하면 광범위한 지원 파일 형식에서 전자 서명을 효율적으로 검색하고 검색할 수 있어 문서 작업 흐름 통합이 원활해집니다."
    items: 
          
        # format loop 1
        - name: "PDF에서 서명 검색"
          format: "PDF"
          link: "/signature/nodejs-java/search/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에서 서명 찾기"
          format: "DOCX"
          link: "/signature/nodejs-java/search/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "PPTX에서 서명 찾기"
          format: "PPTX"
          link: "/signature/nodejs-java/search/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX에서 서명 검색"
          format: "XLSX"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---