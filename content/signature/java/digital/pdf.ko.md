



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:16
draft: false
lang: ko
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java로 PDF 파일에 디지털 전자 서명 추가하기"
head_description: "Java를 사용하여 PDF 파일에 디지털 서명을 몇 줄의 코드로 추가하세요. GroupDocs.Signature for Java을 사용하여 다양한 파일 형식에 서명할 수 있습니다."

############################# Header ############################
title: "PDF를 디지털 서명으로 보호하기" 
description: "GroupDocs.Signature for Java의 기능을 활용하여 디지털 인증서를 사용하여 비즈니스 문서의 내용을 보호하세요. 문서를 표시하고 안전하게 보호할 수 있는 다양한 방법을 제공합니다."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료로 다운로드"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java에 대하여"
    link: "/signature/java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/)는 다양한 유형의 문서 처리를 지원하는 포괄적인 서명 솔루션입니다. PDF, MS Office, 이미지, ZIP 파일 및 기타 인기 있는 비즈니스 형식을 포함하여 60개 이상의 형식으로 파일에 텍스트, 이미지, 디지털 인증서 및 스탬프를 추가할 수 있습니다. 또한 서명된 문서는 편리한 방법으로 검색, 검증, 수정 또는 자동으로 삭제할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "Java에서 디지털 인증서를 사용한 PDF 보호를 위한 단계"
    content: |
      [GroupDocs.Signature](/signature/java/)는 Java 개발자가 디지털 서명을 사용하여 PDF 문서의 변화를 방지할 수 있게 합니다. 중요한 데이터를 보호할 수 있는 기능을 비즈니스 애플리케이션에 사용하세요.
      
      1. Signature 클래스 생성자에 PDF 문서를 전달합니다.
      2. 문서를 보호하기 위해 디지털 인증서와 비밀번호를 사용합니다.
      3. 선택적으로 문서 페이지에 디지털 서명의 시각적 표현을 추가합니다.
      4. 문서에 서명하여 향후 변경을 방지합니다.
   
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
        // 디지털 서명을 위해 문서와 함께 Signature 사용
        Signature signature = new Signature("input.pdf");

        // 디지털 인증서와 비밀번호 제공
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // 필요시 시각적 표현 설정
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);

        // 문서를 디지털 인증서로 보호
        SignResult result = signature.sign("output.pdf", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "서명으로 문서 내용 강화를 또는 보호하기"
  description: "GroupDocs.Signature for Java 라이브러리는 모든 인기 있는 파일 형식에 서명할 수 있습니다. 비즈니스 프로세스를 간소화하기 위해 다양한 유형의 서명을 자동으로 추가, 수정, 검증 또는 삭제하십시오."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "GroupDocs.Signature의 기능"
  features:
    # feature loop
    - title: "문서에 서명 추가"
      content: "텍스트, 이미지, 바코드, QR 코드 또는 스탬프 서명을 지원하는 문서의 모든 페이지에 정밀하게 추가할 수 있습니다. EXIF와 같은 숨겨진 메타데이터를 이미지와 대부분의 파일 형식에 추가하거나 수정할 수 있습니다. 디지털 서명을 사용하여 문서 내용을 무단 변경으로부터 보호하세요."

    # feature loop
    - title: "서명 검색 및 검증"
      content: "서명 후 문서를 다양한 방식으로 처리할 수 있습니다. 서명된 문서가 제대로 처리되었는지 확인하기 위해 검증하세요. 더 많은 제어가 필요하면 검색을 통해 모든 서명의 목록을 가져올 수 있습니다."

    # feature loop
    - title: "서명 수정"
      content: "대부분의 유형의 서명은 추가 수정을 지원합니다. 텍스트 수정, 위치, 색상, 크기 등을 변경할 수 있습니다."

    # feature loop
    - title: "불필요한 서명 제거"
      content: "우리 솔루션은 서명에 대한 전체 CRUD 작업을 지원합니다. 필요시 문서에서 디지털 인증서를 포함한 여러 유형의 서명을 삭제할 수 있습니다."
      
  code_samples:
    # code sample loop
    - title: "디지털 서명으로 문서 보호하기"
      content: |
        디지털 서명을 사용하여 문서의 변화를 방지하는 방법을 배우세요.
        {{< landing/code title="Java">}}
        ```java {style=abap}
        // 서명을 위한 문서 제공
        Signature signature = new Signature("input.pdf");

        // 유효한 비밀번호가 있는 디지털 인증서 사용
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // 추가 텍스트 데이터 지정
        options.setReason("Security issue");
        options.setContact("John Smith");
        options.setLocation("Office D.W.");

        // 이미지와 다른 옵션을 사용하여 시각적 표현 설정
        options.setImageFilePath("image.png");

        options.setAllPages(true);
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        Padding padding = new Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);

        // 보호된 문서를 다른 위치에 저장
        SignResult result = signature.sign("output.pdf", options);
        ```
        {{< /landing/code >}}


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
    title: "우리의 포괄적인 기능 세트 살펴보기"
    exclude: "digital"
    description: "우리 플랫폼이 제공하는 방대한 기능성과 서명 지원을 자랑스럽게 생각합니다."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/java/esign/pdf/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/java/text/pdf/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/java/image/pdf/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/java/barcode/pdf/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/java/qrcode/pdf/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/java/stamp/pdf/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다른 형식의 문서 서명"
    exclude: "PDF"
    description: "Java API는 60개 이상의 형식을 처리할 수 있도록 해줍니다. 페이지에 다양한 서명을 생성하고 추가하며, 디지털 인증서로 내용을 봉인하고, 문서 내의 기존 서명을 관리하고 편집하세요."
    items: 
          
        # format loop 1
        - name: "PDF 보호"
          format: "PDF"
          link: "/signature/java/digital/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX 보호"
          format: "DOCX"
          link: "/signature/java/digital/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "PPTX 보호"
          format: "PPTX"
          link: "/signature/java/digital/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX 보호"
          format: "XLSX"
          link: "/signature/java/digital/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---