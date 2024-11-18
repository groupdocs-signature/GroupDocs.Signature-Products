



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:12
draft: false
lang: ko
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java로 DOCX에서 디지털 서명 검색"
head_description: "GroupDocs.Signature for Java API를 사용하여 DOCX 파일 내에서 서명을 검색합니다. PDF, Word, Excel, 프레젠테이션 및 이미지에서 서명을 찾으세요."

############################# Header ############################
title: "DOCX에서 디지털 서명 검색" 
description: "GroupDocs.Signature for Java를 사용하여 PDF, Word, Excel, 프레젠테이션 또는 이미지 파일에 포함된 전자 서명의 전체 목록을 가져오세요."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 다운로드"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java 소개"
    link: "/signature/java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/)는 문서 서명을 위한 강력한 기능을 제공합니다. PDF, MS Office 문서, 이미지, ZIP 파일 및 기타 일반 비즈니스 형식을 포함하여 60개 이상의 형식으로 텍스트, 이미지, 바코드, 디지털 인증서 및 스탬프를 추가할 수 있습니다. 또한 언제든지 서명을 검색, 검증, 수정 또는 삭제할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "Java를 사용한 DOCX 서명 검색 단계"
    content: |
      [GroupDocs.Signature](/signature/java/)는 DOCX 파일 내에서 모든 디지털 서명을 검색할 수 있는 강력한 엔진을 제공합니다. Java 개발자는 우리 솔루션을 통해 애플리케이션을 향상할 수 있습니다.
      
      1. 서명을 검색할 DOCX 파일 경로를 제공합니다.
      2. SearchOptions를 사용하여 검색 결과를 다듬습니다.
      3. 결과를 얻기 위해 Search 메서드를 실행합니다.
      4. 발견된 서명의 목록을 분석합니다.
   
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

        // Signature의 인스턴스를 문서 경로로 생성
        final Signature signature = new Signature("input.docx");

        // 모든 페이지를 포함하기 위해 TextSearchOptions를 인스턴스화
        TextSearchOptions options = new TextSearchOptions();
        options.setAllPages(true);

        // 문서 내에서 문자 서명을 검색
        List<TextSignature> signatures = signature.search(TextSignature.class, options);
        System.out.print("\nSource document contains following text signature(s).");

        // 추가 분석을 위해 발견된 서명을 목록화
        for (TextSignature textSignature : signatures) {
            System.out.print("Found Text signature at page " + textSignature.getPageNumber() 
                + " with type [" + textSignature.getSignatureImplementation() + "] and 
                text '" + textSignature.getText() + "'.");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "종합 문서 서명 솔루션"
  description: "모든 주요 문서 형식과 호환되는 우리의 문서 서명 솔루션을 자랑스럽게 소개합니다. 문서를 향상하거나 콘텐츠를 보호하기 위해 다양한 서명을 추가하세요."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "서명 검색"
  features:
    # feature loop
    - title: "비즈니스 문서 서명"
      content: "문서의 모든 페이지에서 원하는 위치에 디지털 서명을 삽입하세요. 텍스트, 이미지, 바코드, 메타데이터, 스탬프 또는 디지털 인증서와 같은 다양한 서명 유형을 사용할 수 있습니다."

    # feature loop
    - title: "서명 관리"
      content: "서명 후 문서는 추가 처리가 필요할 수 있습니다. 사용 가능한 모든 서명을 검색하고 필요에 따라 업데이트하거나 삭제하세요."

    # feature loop
    - title: "문서 콘텐츠 보호"
      content: "문서에 포함된 숨겨진 메타데이터를 관리하세요. 새 메타데이터를 추가하거나 기존 항목을 제거할 수 있습니다. 기업의 디지털 인증서를 사용하여 문서의 내용을 무단 변경으로부터 보호하세요."
      
  code_samples_ext:
    # code sample ext loop
    - title: "이미지 서명 검색"
      content: |
        이 예제는 특정 문서에서 이미지 서명을 찾는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 소스 문서를 생성자 매개변수로 전달
          final Signature signature = new Signature("input.docx");

          // 텍스트 유형의 모든 서명을 검색
          List<ImageSignature> signatures = signature.search(ImageSignature.class, SignatureType.Image);
          System.out.print("\nSource document contains following image signature(s).");

          // 발견된 서명의 속성으로 결과 표시
          for (ImageSignature imageSignature : signatures)
          {
              System.out.print("Image signature found at page "+imageSignature.getPageNumber()+
                    " with size "+imageSignature.getSize()+". Created "+imageSignature.getCreatedOn()+
                    ", modified "+imageSignature.getModifiedOn());
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
    title: "지원되는 작업"
    exclude: "search"
    description: "우리 제품은 문서를 서명하고 서명 후 서명을 관리할 수 있는 유연한 API를 제공합니다."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/java/esign/docx/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/java/text/docx/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/java/image/docx/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/java/barcode/docx/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/java/qrcode/docx/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/java/stamp/docx/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/java/search/docx/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/java/verify/docx/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/java/modify/docx/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/java/delete/docx/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 파일 형식에서 서명 검색"
    exclude: "DOCX"
    description: "GroupDocs.Signature for Java API는 서명된 파일에서 서명 목록을 검색할 수 있도록 합니다. 추가 처리를 위해 인기 있는 파일 형식에서 서명을 추출하세요."
    items: 
          
        # format loop 1
        - name: "PDF에서 서명 검색"
          format: "PDF"
          link: "/signature/java/search/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에서 서명 찾기"
          format: "DOCX"
          link: "/signature/java/search/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "PPTX에서 서명 찾기"
          format: "PPTX"
          link: "/signature/java/search/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX에서 서명 검색"
          format: "XLSX"
          link: "/signature/java/search/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---