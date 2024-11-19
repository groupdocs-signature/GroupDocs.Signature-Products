



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:30
draft: false
lang: ko
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScript로 JPEG에 전자 서명하기"
head_description: "JavaScript API의 기능을 활용하여 PDF, Word 문서, Excel 시트, 프레젠테이션 및 이미지 형식을 포함한 JPEG 파일을 디지털 서명하고 보호합니다."

############################# Header ############################
title: "JPEG 파일을 전자적으로 서명하기" 
description: "GroupDocs.Signature for Node.js via Java를 사용하여 PDF, Word, Excel, 프레젠테이션 및 이미지 형식과 같은 문서에 다양한 디지털 서명을 삽입하여 데이터 무결성과 규정 준수를 보장합니다."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "지금 무료로 다운로드"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java API 개요"
    link: "/signature/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)는 전자 서명을 추가하기 위한 강력한 도구 세트를 제공합니다. 직관적인 API를 통해 외부 소프트웨어 없이도 다양한 파일 형식에서 서명을 원활하게 추가, 검색, 검증, 수정 및 삭제할 수 있습니다. PDF, Word 문서, Excel 스프레드시트, PowerPoint 슬라이드 및 다양한 이미지 형식의 서명을 부드럽게 지원합니다.

############################# Steps ############################
steps:
    enable: true
    title: "JavaScript를 사용하여 JPEG에 서명하는 단계"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)는 JPEG 파일에 사용자 지정 서명을 추가하는 과정을 간소화합니다. Node.js via Java 개발자는 애플리케이션에 서명 기능을 원활하게 통합할 수 있습니다.
      
      1. Signature 인스턴스에 JPEG 문서를 로드합니다.
      2. SignOptions를 구성하여 서명 속성을 정의합니다.
      3. 필요에 따라 크기, 색상 및 내용을 조정합니다.
      4. 서명된 문서를 지정된 위치에 저장합니다.
   
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

        // Signature 인스턴스로 문서를 가져옵니다.
        const signature = new signatureLib.Signature('input.jpeg');

        // QrCodeSignOptions 객체를 생성합니다.
        const options = new signatureLib.QrCodeSignOptions('QR code text');

        // 필요한 모든 옵션을 지정합니다.
        options.setLeft(100);
        options.setTop(100);
        options.setForeColor(new Color(255, 0, 0));

        // 서명된 문서를 로컬 디스크에 저장합니다.
        signature.sign('output.jpeg', options);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "고급 디지털 서명 기능"
  description: "우리의 고급 API는 다양한 문서의 전자 서명 자동화, 검증, 수정 및 관리를 용이하게 하여 비즈니스 운영을 간소화합니다."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "디지털 서명 기능"
  features:
    # feature loop
    - title: "오피스 파일에 대한 디지털 서명"
      content: "문서의 모든 페이지나 위치에 디지털 서명을 간편하게 추가할 수 있습니다. 보안 및 문서 무결성을 향상시키기 위해 디지털 인증서, 메타데이터, 바코드 또는 시각적 요소와 같은 옵션으로 서명을 사용자 정의하세요."

    # feature loop
    - title: "포괄적인 서명 관리"
      content: "문서에 서명이 완료된 후, 서명을 쉽게 관리할 수 있습니다. 모든 서명의 전체 목록을 조회하여 필요에 따라 업데이트하거나 제거할 수 있습니다."

    # feature loop
    - title: "문서 보안 강화"
      content: "디지털 인증서를 사용하여 문서 변조를 방지하세요. 메타데이터를 삽입 또는 추출하여 추적 가능성과 감사 기능을 강화하여 문서의 규정 준수 및 진위를 보장합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "문서에 이미지 서명을 적용하는 방법"
      content: |
        이 가이드는 문서의 지정된 페이지에 이미지 서명을 부착하는 과정을 자세히 설명합니다.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
        
          // 소스 문서를 입력 매개변수로 제공합니다.
          const signature = new signatureLib.Signature('input.jpeg');

          // 서명 구성 옵션에서 이미지 파일 경로를 지정합니다.
          const options = new signatureLib.ImageSignOptions('image.jpg');

          // 서명을 위한 크기를 설정하고 대상 페이지를 지정합니다.
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setHeight(150);
          options.setWidth(200);
          options.setMargin(new signatureLib.Padding(50));
          options.setAllPages(true);

          // 문서에 서명 적용을 구현합니다.
          signature.sign('output.jpeg', options);

          ```
        platform: "nodejs-java"
        copy_title: "복사"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "클릭하여 복사"
          copy_done: "복사됨"
        top_links:
          #  loop
          - title: "결과 다운로드"
            icon: "download"
            link: "/examples/signature/formats/signature_esign.jpeg"
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
    title: "광범위한 기능 살펴보기"
    exclude: "esign"
    description: "우리는 다양한 서명 유형과 기능이 풍부한 작업을 제공합니다."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 파일 형식에 디지털 서명하기"
    exclude: "JPEG"
    description: "Node.js via Java API는 60개 이상의 파일 형식에 디지털 서명을 적용할 수 있어 비즈니스에 중요한 문서를 보호하는 데 매우 유연성을 제공합니다."
    items: 
          
        # format loop 1
        - name: "e-서명 PDF"
          format: "PDF"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "e-서명 DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/esign/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "e-서명 JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "JPEG 이미지"
          
        # format loop 4
        - name: "e-서명 PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/esign/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 5
        - name: "e-서명 XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---