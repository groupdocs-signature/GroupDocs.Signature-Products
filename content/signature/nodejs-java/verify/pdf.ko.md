



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:16
draft: false
lang: ko
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "PDF에서 JavaScript를 사용하여 디지털 서명 검증"
head_description: "GroupDocs.Signature for Node.js via Java를 사용하면 PDF 문서 내 서명의 진위를 효율적으로 검증할 수 있습니다. PDF, Word, Excel, 프레젠테이션, 이미지, ZIP 파일 등에서 서명을 원활하게 확인하세요."

############################# Header ############################
title: "PDF에서 디지털 서명 검증" 
description: "PDF, Word, Excel, 프레젠테이션, 이미지, ZIP을 포함한 다양한 문서 형식에서 모든 지원되는 전자 서명의 정확성과 유효성을 보장하십시오. GroupDocs.Signature for Node.js via Java를 사용하여 서명을 검증하세요."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 버전 다운로드"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java의 응용 프로그램"
    link: "/signature/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)는 60개 이상의 파일 형식에서 서명할 수 있는 포괄적인 문서 서명 관리 기능을 제공합니다. 텍스트, 이미지, 바코드, 디지털 인증서, 메타데이터, 스탬프 등을 지원하는 GroupDocs.Signature for Node.js via Java는 PDF, MS Office 문서, 이미지, ZIP 아카이브 등에서 서명을 검색, 검증, 업데이트 또는 제거할 수 있도록 돕습니다.

############################# Steps ############################
steps:
    enable: true
    title: "JavaScript를 사용하여 PDF에서 서명을 검증하는 방법"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)는 PDF 문서에서 특정 서명의 존재를 인증할 수 있습니다. Node.js via Java 개발자는 당사의 검증 기능을 통합하여 애플리케이션을 향상시킬 수 있습니다.
      
      1. Signature 인스턴스에 PDF 문서를 로드합니다.
      2. 원하는 검증 결과를 얻기 위해 VerifyOptions를 생성하고 구성합니다.
      3. 검증 프로세스를 시작합니다.
      4. 검증 결과를 검토하고 평가합니다.
   
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

        // Signature 객체를 문서와 함께 인스턴스화합니다.
        const signature = new signatureLib.Signature('input.pdf');

        // 지정된 텍스트를 포함하여 서명을 검증하기 위해 TextVerifyOptions를 설정합니다.
        const options = new signatureLib.TextVerifyOptions();
        options.setText('signature');
        options.setMatchType(signatureLib.TextMatchType.Contains);

        // 문서 서명의 검증 프로세스를 실행합니다.
        const result = signature.verify(options);

        // 검증 결과를 해석하고 평가합니다.
        if (result.isValid()) {
            console.log('\nDocument was verified successfully!');
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "최첨단 문서 서명 기술"
  description: "GroupDocs.Signature는 다양한 오피스 형식에서 서명을 검증하고 관리할 수 있는 올인원 솔루션을 제공합니다. 7가지 서명 유형과 완벽한 CRUD 작업을 지원하며, 원활한 문서 관리와 콘텐츠 보안을 보장합니다."
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "서명 검증 기능"
  features:
    # feature loop
    - title: "기업 문서에 서명하기"
      content: "텍스트 기반, 이미지, 바코드, 메타데이터, 스탬프 또는 디지털 인증서와 같은 디지털 서명을 문서에 안전하고 맞춤화된 방식으로 적용하십시오. GroupDocs.Signature for Node.js via Java는 원활하고 전문적인 기업 문서 서명을 보장합니다."

    # feature loop
    - title: "서명 생애주기 운영"
      content: "문서 서명에 대한 완전한 제어권을 확보하십시오. 파일의 모든 서명을 나열하고, 그 진위를 검증하며, 필요에 따라 업데이트하거나 전체적으로 제거하여 적절한 문서 처리를 보장합니다."

    # feature loop
    - title: "문서 무결성 보장"
      content: "디지털 인증서를 활용하여 문서의 무단 변경으로부터 보호하십시오. 메타데이터를 사용하여 문서 내용을 안전하게 보호하고 추적하여 변조되지 않고 기밀 유지됩니다."

    # feature loop
    - title: "맞춤형 네이티브 서명"
      content: "PDF의 스티커나 Word 문서의 워터마크와 같은 맞춤형 네이티브 서명을 추가하십시오. 이러한 맞춤형 옵션은 전문적이고 안전한 문서 처리를 가능하게 하여 기업 환경에 적합합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "바코드 서명 검증 프로세스"
      content: |
        이 예제는 문서 내에 내장된 바코드 서명을 인증하는 방법론을 설명합니다.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 바코드 서명이 포함된 문서를 제출합니다.
          const signature = new signatureLib.Signature('input.pdf');

          // 지정된 텍스트에 따라 바코드를 검증하기 위해 매개변수를 구성합니다.
          const options = new signatureLib.BarcodeVerifyOptions();
          options.setText('12345');
          options.setMatchType(signatureLib.TextMatchType.StartsWith);

          // 문서에 이전에 부착된 서명을 인증합니다.
          const result = signature.verify(options);

          // 검증 보고서를 확인합니다.
          if (result.isValid()) {
              console.log('\nDocument was verified successfully!');
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
    title: "포괄적인 기능과 지원되는 서명"
    exclude: "verify"
    description: "GroupDocs.Signature의 고급 기능을 탐색하며 다양한 서명 관리 도구 및 작업을 통해 문서 워크플로를 향상시키십시오."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/nodejs-java/text/pdf/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/nodejs-java/image/pdf/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pdf/"
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
    title: "다양한 형식에 대한 포괄적인 서명 검증"
    exclude: "PDF"
    description: "GroupDocs.Signature for Node.js via Java는 여러 문서 형식에서 서명 검증을 간소화하며 강력한 서명 검증 제어 기능을 제공합니다. 검증 프로세스를 사용자 맞춤화하여 문서가 적절히 서명되었는지 확인하십시오."
    items: 
          
        # format loop 1
        - name: "PDF 서명 검증"
          format: "PDF"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX 서명 검증"
          format: "DOCX"
          link: "/signature/nodejs-java/verify/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "PPTX 서명 검증"
          format: "PPTX"
          link: "/signature/nodejs-java/verify/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX 서명 유효성 검사"
          format: "XLSX"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---