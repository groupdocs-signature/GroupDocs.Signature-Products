



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:28
draft: false
lang: ko
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java 앱으로 XLSX 파일에 전자 서명하기"
head_description: "Java API를 사용하여 XLSX 파일을 처리하고 PDF, Word, Excel, 프레젠테이션 및 이미지와 같은 다양한 서명 유형을 적용하세요."

############################# Header ############################
title: "XLSX를 위한 전자 서명" 
description: "GroupDocs.Signature for Java를 사용하여 PDF, Word, Excel, 프레젠테이션 및 이미지 등 인기 있는 모든 비즈니스 형식에 폭넓은 전자 서명을 추가하세요."
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
    title: "GroupDocs.Signature for Java API에 대해"
    link: "/signature/java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/)는 고급 전자 서명 기능을 제공합니다. 이를 통해 외부 소프트웨어 없이 문서 및 이미지에 다양한 유형의 전자 서명을 추가, 검색, 검증, 수정 및 제거할 수 있습니다. PDF, Word 문서, Excel 스프레드시트, PowerPoint 프레젠테이션 및 인기도 이미지 형식의 전자 서명을 손쉽게 추가하세요.

############################# Steps ############################
steps:
    enable: true
    title: "Java를 사용하여 XLSX에 서명하는 단계"
    content: |
      [GroupDocs.Signature](/signature/java/)는 XLSX 파일에 맞춤 서명을 추가할 수 있게 해줍니다. Java 개발자는 당사의 소프트웨어를 사용하여 애플리케이션에 서명 기능을 통합할 수 있습니다.
      
      1. Signature 인스턴스에 서명할 XLSX 파일을 제공합니다.
      2. SignOptions를 사용하여 서명 세부정보를 정의합니다.
      3. 크기, 색상 및 내용을 포함한 다양한 속성을 사용자 정의합니다.
      4. 서명된 파일을 원하는 위치에 저장합니다.
   
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
        // Signature 인스턴스에 문서를 로드합니다.
        Signature signature = new Signature("input.xlsx");

        // QrCodeSignOptions 개체를 인스턴스화합니다.
        QrCodeSignOptions options = new QrCodeSignOptions("QR code text");

        // 원하는 모든 옵션을 구성합니다.
        options.setLeft(100);
        options.setTop(100);
        options.setForeColor(Color.RED);

        // 추가된 QR 코드가 포함된 파일을 로컬 디스크에 저장합니다.
        signature.sign("output.xlsx", options);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "문서 전자 서명"
  description: "우리의 전자 서명 API는 비즈니스 프로세스를 간소화합니다. 다양한 서명을 프로그래밍적으로 서명하고, 검색하고, 업데이트하고, 삭제하고, 검증하세요."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "전자 서명"
  features:
    # feature loop
    - title: "사무 문서에 전자 서명하기"
      content: "문서의 어떤 페이지에나 전자 서명을 쉽게 배치할 수 있습니다. 텍스트, 이미지, 바코드, 메타데이터 또는 디지털 인증서로 문서 내용을 향상시킵니다."

    # feature loop
    - title: "서명 관리"
      content: "서명 후 문서는 추가로 처리할 수 있습니다. 존재하는 모든 서명의 목록을 검색하고 필요에 따라 수정하거나 삭제할 수 있습니다."

    # feature loop
    - title: "고급 콘텐츠 제어"
      content: "회사 디지털 인증서를 사용하여 무단 변경으로부터 비즈니스 문서를 보호합니다. 모든 문서 유형에서 사용할 수 있는 숨겨진 메타데이터 항목을 추가하거나 추출합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "문서에 이미지 서명 추가하기"
      content: |
        이 예제는 문서의 특정 페이지에 이미지 서명을 배치하는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 소스 문서를 매개변수로 제공합니다.
          Signature signature = new Signature("input.xlsx");

          // 서명 옵션에서 이미지 경로를 지정합니다.
          ImageSignOptions options = new ImageSignOptions("image.jpg");

          // 서명의 크기와 대상 페이지를 설정합니다.
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setHeight(150);
          options.setWidth(200);
          Padding padding = new Padding(50);
          options.setMargin(padding);
          options.setAllPages(true);

          // 문서에 서명을 적용합니다.
          signature.sign("output.xlsx", options);

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
        top_links:
          #  loop
          - title: "결과 다운로드"
            icon: "download"
            link: "/examples/signature/formats/signature_esign.xlsx"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "문서"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################## Actions ############################

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
    title: "주요 기능 탐색"
    exclude: "esign"
    description: "우리는 지원하는 다양한 서명 및 작업을 제공합니다."
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
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "전자 서명으로 인기 파일 형식 서명하기"
    exclude: "XLSX"
    description: "Java용 전자 서명 API는 모든 현대 비즈니스 파일 및 문서 형식의 처리를 지원합니다."
    items: 
          
        # format loop 1
        - name: "e-서명 PDF"
          format: "PDF"
          link: "/signature/java/esign/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "e-서명 DOCX"
          format: "DOCX"
          link: "/signature/java/esign/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "e-서명 JPEG"
          format: "JPEG"
          link: "/signature/java/esign/jpeg/"
          description: "JPEG 이미지"
          
        # format loop 4
        - name: "e-서명 PPTX"
          format: "PPTX"
          link: "/signature/java/esign/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 5
        - name: "e-서명 XLSX"
          format: "XLSX"
          link: "/signature/java/esign/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---