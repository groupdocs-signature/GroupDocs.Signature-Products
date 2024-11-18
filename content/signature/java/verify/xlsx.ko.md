



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:14
draft: false
lang: ko
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "XLSX 전자 서명 검증 - Java"
head_description: "GroupDocs.Signature for Java는 XLSX 파일에 배치된 서명을 검증할 수 있게 합니다. PDF, Word 문서, Excel 시트, 프레젠테이션, 이미지 또는 ZIP 아카이브의 서명을 검증하십시오."

############################# Header ############################
title: "XLSX에 대한 전자 서명 검증" 
description: "GroupDocs.Signature for Java를 사용하여 PDF, Word, Excel, 프레젠테이션, 이미지 또는 ZIP 파일의 모든 지원되는 전자 서명을 검증하십시오."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 버전 다운로드"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java의 적용 분야"
    link: "/signature/java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/)는 문서 서명 및 기타 작업을 위한 전체 CRUD 작업을 지원합니다. PDF, MS Office 파일, 이미지 및 ZIP 아카이브를 포함하여 60개 이상의 문서 형식에 대해 텍스트, 이미지, 바코드, 디지털 인증서, 메타데이터 및 스탬프 서명으로 서명할 수 있습니다. 서명을 검색하고, 검증하고, 수정하거나 삭제하는 추가 작업도 가능합니다.

############################# Steps ############################
steps:
    enable: true
    title: "Java를 사용한 XLSX의 서명 검증 단계"
    content: |
      [GroupDocs.Signature](/signature/java/)는 XLSX 문서 내 특정 서명의 존재를 검증할 수 있습니다. Java 개발자는 우리의 솔루션에서 제공하는 기능을 추가하여 애플리케이션을 강화할 수 있습니다.
      
      1. Signature 인스턴스에 XLSX 파일을 로드합니다.
      2. 원하는 결과를 얻기 위해 VerifyOptions를 인스턴스화하고 구성합니다.
      3. 검증 프로세스를 시작합니다.
      4. 검증 결과를 검토합니다.
   
    code:
      platform: "java"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "샘플 서명"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "클릭하여 복사"
        copy_done: "복사됨"
      links:
        #  loop
        - title: "더 많은 예제"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "문서"
          link: "https://docs.groupdocs.com/signature/java/"

      content: |
        ```java {style=abap}
        // 문서와 함께 Signature 인스턴스를 생성합니다.
        Signature signature = new Signature("input.xlsx");

        // 특정 텍스트를 포함하는 서명을 검증하기 위한 TextVerifyOptions를 생성합니다.
        TextVerifyOptions options = new TextVerifyOptions();
        options.setText("signature");
        options.setMatchType(TextMatchType.Contains);

        // 문서 내 서명을 검증합니다.
        VerificationResult result = signature.verify(options);

        // 검증 결과를 처리합니다.
        if (result.isValid())
        {
            System.out.print("\nDocument was verified successfully!");
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "종합적인 문서 서명 솔루션"
  description: "GroupDocs.Signature는 7종의 서명과 전체 CRUD 작업을 통해 인기 있는 오피스 문서 형식을 강화하여 문서 내용을 안전하게 보호합니다."
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "서명 검증"
  features:
    # feature loop
    - title: "기업 문서 서명"
      content: "모든 문서에 전문적인 디지털 서명을 추가하십시오. 우리의 솔루션은 텍스트, 이미지, 바코드, 메타데이터, 스탬프 및 디지털 인증서와 같은 다양한 유형의 서명을 지원합니다."

    # feature loop
    - title: "서명 CRUD 작업"
      content: "많은 경우, 서명된 문서는 추가 처리가 필요합니다. 문서에 있는 모든 서명의 목록을 가져오고, 이를 검증하며, 속성을 수정하거나 필요 시 제거하십시오."

    # feature loop
    - title: "문서 내용 보호"
      content: "디지털 인증서를 사용하여 기업 문서를 무단 변경으로부터 보호하십시오. 문서 내용을 더욱 보호하기 위해 숨겨진 메타데이터를 포함하십시오."

    # feature loop
    - title: "네이티브 서명"
      content: "PDF 스탬프 또는 Word 워터마크와 같은 문서별 텍스트 서명을 활용하여 기업 공사용으로 맞춤형 전문 문서를 생성하십시오."
      
  code_samples_ext:
    # code sample ext loop
    - title: "바코드 서명 검증"
      content: |
        이 예제는 문서 내 바코드 서명을 검증하는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 바코드 서명이 포함된 문서를 제공합니다.
          final Signature signature = new Signature("input.xlsx");

          // 특정 텍스트에 대한 바코드를 검증하기 위한 옵션을 구성합니다.
          BarcodeVerifyOptions options = new BarcodeVerifyOptions();
          options.setText("12345");
          options.setMatchType(TextMatchType.StartsWith);

          // 문서에 적용된 서명을 검증합니다.
          VerificationResult result = signature.verify(options);

          // 검증 결과를 표시합니다.
          if (result.isValid())
          {
              System.out.print("\nDocument was verified successfully!");
          }
          ```
        platform: "java"
        copy_title: "복사"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "클릭하여 복사"
          copy_done: "복사됨"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "문서"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Signature의 기능을 무료로 시도하거나 라이센스를 요청하세요."
  items:
    #  loop
    - title: "Maven 다운로드"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "라이센스 구매"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "지원되는 작업 및 서명 유형"
    exclude: "verify"
    description: "GroupDocs.Signature가 지원하는 전체 기능 및 서명 작업 범위를 탐색하십시오."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/java/esign/xlsx/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/java/text/xlsx/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/java/image/xlsx/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/java/barcode/xlsx/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/java/qrcode/xlsx/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/java/digital/xlsx/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/java/stamp/xlsx/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/java/search/xlsx/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/java/verify/xlsx/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/java/modify/xlsx/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/java/delete/xlsx/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats #####################
more_formats:
    enable: true
    title: "파일 형식 전반에 걸친 서명 검증"
    exclude: "XLSX"
    description: "GroupDocs.Signature for Java는 문서 내 모든 서명을 검증하는 과정을 간소화합니다. 서명된 문서의 무결성을 보장하기 위해 사용자 정의 검증 매개변수를 설정하십시오."
    items: 
          
        # format loop 1
        - name: "PDF 서명 검증"
          format: "PDF"
          link: "/signature/java/verify/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX 서명 검증"
          format: "DOCX"
          link: "/signature/java/verify/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "PPTX 서명 검증"
          format: "PPTX"
          link: "/signature/java/verify/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX 서명 유효성 검사"
          format: "XLSX"
          link: "/signature/java/verify/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---