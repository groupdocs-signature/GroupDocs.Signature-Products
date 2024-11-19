



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:42
draft: false
lang: ko
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "XLSX에서 JavaScript를 사용하여 서명 삭제"
head_description: "GroupDocs.Signature for Node.js via Java를 사용하면 서명된 XLSX 문서에서 디지털 서명, 바코드, 텍스트, 이미지, 메타데이터 서명을 삭제할 수 있습니다."

############################# Header ############################
title: "XLSX에서 서명을 간편하게 제거" 
description: "우리의 포괄적인 솔루션은 단순한 문서 서명을 넘어서, GroupDocs.Signature for Node.js via Java 내에서 다양한 서명을 찾고 삭제할 수 있는 강력한 기능을 제공합니다."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 다운로드 받기"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java를 알아보세요"
    link: "/signature/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)는 텍스트, 이미지, 바코드, 디지털 인증서 및 도장을 포함한 다양한 서명 유형을 지원하도록 설계된 첨단 기업용 디지털 서명 라이브러리입니다. PDF, MS Office 파일, 이미지, ZIP 아카이브 등 60개 이상의 문서 형식과 호환되며, 이 도구는 전자 문서 워크플로우에서 비할 데 없는 유연성을 제공합니다. 이 플랫폼은 원활한 서명 삽입을 지원할 뿐만 아니라 서명을 검색, 검증, 업데이트 및 삭제할 수 있는 강력한 기능을 제공하여 기업 환경에서 디지털 서명 프로세스의 전체 수명 주기를 관리하는 데 기여합니다.

############################# Steps ############################
steps:
    enable: true
    title: "JavaScript를 사용하여 XLSX에서 디지털 서명을 제거하기 위한 가이드라인"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)는 Node.js via Java 개발자가 XLSX 파일에서 전자 서명을 효율적으로 제거할 수 있도록 간단한 단계를 따르는 것을 가능하게 합니다.
      
      1. Signature 클래스의 인스턴스에 XLSX 파일 경로를 제공합니다.
      2. Search 메소드를 활용하여 문서 내 모든 서명을 식별합니다.
      3. 식별된 서명 중 하나 이상을 제거합니다.
      4. 문서 처리 결과를 검토합니다.
   
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

        // Signature 인스턴스에 서명이 포함된 문서를 전달하세요
        const signature = new signatureLib.Signature('input.xlsx');

        // 모든 바코드 서명을 삭제합니다.
        const options = new signatureLib.DigitalSearchOptions();
        const signatures = signature.search(signatureLib.DigitalSignature.class, options);

        // 첫 번째 발견된 디지털 서명을 제거하세요
        if(signatures.size() > 0)
        {
            const digitalSignature = signatures[0];
            const result = signature.delete('output.xlsx', digitalSignature);

            // 삭제 결과를 처리하세요
            if(result)
            {
                console.log(`\n XLSX digital signature deleted successfully`);
            }
        }

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "서명 도구로 문서 보안 강화"
  description: "GroupDocs.Signature for Node.js via Java는 비즈니스 파일 형식의 서명 및 관리를 간소화하도록 특별히 설계되어 서명을 추가, 편집, 검증 또는 삭제할 수 있는 정밀한 기능을 제공합니다."
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "GroupDocs.Signature의 종합적인 기능을 탐색하세요"
  features:
    # feature loop
    - title: "문서 서명"
      content: "지원하는 문서의 모든 페이지에 텍스트, 이미지, 바코드, QR 코드 또는 도장 서명을 쉽게 추가하세요. 이미지의 EXIF와 같은 숨겨진 메타데이터를 활용하거나 디지털 인증서를 통해 무단 수정 방지를 위한 문서 무결성을 확보하세요."

    # feature loop
    - title: "서명 검색 및 검증"
      content: "우리의 도구는 문서 서명의 철저한 검증을 가능하게 하여 그 진정성을 보장합니다. 문서 내 모든 서명을 검색하여 문서 관리 기능을 강화하세요."

    # feature loop
    - title: "기존 서명 편집"
      content: "기존에 추가된 서명을 쉽게 수정하고 텍스트를 조정하거나 위치를 변경하거나 색상을 변경하여 특정 요구 사항을 충족시킬 수 있습니다."

    # feature loop
    - title: "원하지 않는 서명 제거"
      content: "완전한 CRUD 기능을 통해 우리의 솔루션은 문서에서 다양한 서명을 효율적으로 삭제할 수 있는 유연성과 제어를 보장합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "모든 바코드 서명 제거하기"
      content: |
        문서에 삽입된 모든 바코드 서명을 없애는 절차를 알아보세요.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 바코드 서명이 포함된 문서를 제공합니다.
          const signature = new signatureLib.Signature('input.xlsx');

          // 모든 바코드 서명을 삭제합니다.
          const result = await signature.delete('output.xlsx', signatureLib.SignatureType.Barcode);
          if (result.getSucceeded().size() > 0) {

              // 삭제 결과를 검토합니다.
              console.log('Following XLSX barcode signatures were deleted:');
              let number = 1;
              result.getSucceeded().toArray().forEach((o) => {
                    const temp = o;
                    console.log(`Signature #${number++}: Type: ${temp.getSignatureType()}, 
                    Id: ${temp.getSignatureId()}, Text: ${temp.getText()}`);
              });
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
    title: "제공하는 기능 탐색하기"
    exclude: "delete"
    description: "우리 시스템에서 사용할 수 있는 모든 서명 솔루션과 작업 범위를 알아보세요."
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
    title: "다양한 파일 형식에서 서명 삭제"
    exclude: "XLSX"
    description: "GroupDocs.Signature for Node.js via Java 솔루션은 60개 이상의 다양한 파일 형식에서 서명을 제거하는 데 능숙하여 폭넓은 호환성과 기능성을 보장합니다."
    items: 
          
        # format loop 1
        - name: "PDF 서명 삭제"
          format: "PDF"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX 서명 제거"
          format: "DOCX"
          link: "/signature/nodejs-java/delete/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "PPTX 서명 삭제"
          format: "PPTX"
          link: "/signature/nodejs-java/delete/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX 서명 삭제"
          format: "XLSX"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---