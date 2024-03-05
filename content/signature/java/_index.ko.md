---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:00
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: ko
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET, Java, Cloud API 및 온라인 문서 서명 앱"
head_description: ".NET, Java 및 클라우드 기반 애플리케이션을 위한 올인원 문서 전자 서명 솔루션을 받으세요. 간단한 드래그 앤 드롭 기능을 사용하여 일반적인 문서 형식에 온라인으로 서명"

############################# Header ############################
title: "문서에 서명<br>자바 API를 통해"
description: "프로그래머와 최종 사용자를 위한 유연한 API 및 앱 기반 솔루션을 사용하여 모든 플랫폼에서 디지털 문서 및 이미지에 서명하십시오."
words:
  for: "~을 위한"

actions:
  main: "무료 메이븐 다운로드"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "라이선스"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Signature 기능을 무료로 사용해 보거나 라이센스를 요청하세요"

release:
  title: "버전 {0} 출시됨"
  notes: "새로운 소식 보기"
  downloads: "다운로드"

code:
  title: "Java로 PDF 파일 서명"
  more: "더 많은 예시"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // PDF 문서 선택
    Signature signature = new Signature("sample.pdf");
    
    // 텍스트 제공
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // 문서에 서명하고 파일에 저장
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature 개요"
  description: "Java 애플리케이션에서 문서 서명 및 관련 작업을 수행하기 위한 API"
  features:
    # feature loop
    - title: "Java의 디지털 서명이 포함된 향상된 비즈니스 문서"
      content: "신속하고 사용자 정의 가능한 서명: Java용 GroupDocs.Signature는 PDF, 이미지 및 Office 문서에 대한 광범위한 디지털 서명 옵션을 제공합니다. 텍스트, 바코드, QR 코드, 디지털 인증서, 사진 또는 숨겨진 메타데이터를 사용할 수 있습니다. 문서 처리가 빠르고 효율적입니다."

    # feature loop
    - title: "서명된 문서 조작"
      content: "고급 문서 처리에는 Java용 GroupDocs.Signature를 사용하여 서명된 문서에 대한 강력한 작업이 포함됩니다. 다양한 유용한 기준을 사용하여 비즈니스 문서에 추가된 서명을 검색하고 확인할 수 있습니다. 또한 문서에 대한 자세한 정보에 액세스하거나 해당 페이지의 미리 보기 이미지를 얻을 수 있습니다."

    # feature loop
    - title: "다양한 출력 선택"
      content: "강력한 서명 옵션을 사용하면 Java용 GroupDocs.Signature로 서명된 문서의 출력을 사용자 정의할 수 있습니다. 모든 문서 페이지에 서명을 정확하게 배치하고 다양한 방법으로 모양을 구성할 수 있습니다. Java API는 서명된 비즈니스 문서를 다양한 지원 형식으로 저장할 수 있도록 지원하며 암호로 문서를 보호하는 옵션을 제공합니다."

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: "Java용 GroupDocs.Signature는 다음 운영 체제, 프레임워크 및 패키지 관리자를 지원합니다."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "지원되는 파일 형식"
  description: |
    Java용 GroupDocs.Signature는 다음 [파일 형식](https://docs.groupdocs.com/signature/java/supported-document-formats/)을 사용한 작업을 지원합니다.
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office 형식
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### 이미지 및 기타 형식
        * **가지고 다닐 수 있는:** PDF
        * **이미지:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **기타 사무실 형식:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### 기타 형식
        * **편물:** HTML, MHTML
        * **아카이브:** ZIP, TAR, 7Z
        * **인증서:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature 기능"
  description: "디지털 서명으로 PDF, Office 문서 및 이미지에 서명"

  items:
    # feature loop
    - icon: "sign"
      title: "서명 추가"
      content: "모든 페이지의 원하는 위치에 디지털 서명을 정확하게 배치하여 지원되는 다양한 서명 유형을 사용하여 문서에 서명합니다."

    # feature loop
    - icon: "custom"
      title: "결과 맞춤설정"
      content: "원하는 결과를 얻으려면 색상, 글꼴, 테두리, 회전 및 기타 기능을 조정하여 서명 모양을 사용자 정의하세요."

    # feature loop
    - icon: "password"
      title: "비밀번호로 문서를 보호하세요"
      content: "지원되는 다양한 문서 유형의 경우 서명된 문서를 비밀번호로 보호할 수 있습니다."

    # feature loop
    - icon: "protect"
      title: "무단 변경 방지"
      content: "디지털 인증서로 서명된 중요한 비즈니스 문서를 무단 수정으로부터 보호하세요."

    # feature loop
    - icon: "convert"
      title: "원하는 형식으로 결과 얻기"
      content: "지원되는 모든 형식으로 서명된 결과 파일을 쉽게 얻을 수 있습니다. MS Word 문서를 PDF로 쉽게 변환할 수도 있습니다."

    # feature loop
    - icon: "preview"
      title: "문서 미리보기"
      content: "향후 처리를 위해 문서의 모든 페이지를 이미지로 저장하세요."

    # feature loop
    - icon: "search"
      title: "서명 검색 중"
      content: "특정 문서에 이전에 추가된 서명에 대한 정보를 얻을 수 있습니다."

    # feature loop
    - icon: "validate"
      title: "문서 유효성 검사"
      content: "서명된 문서의 서명이 올바른지 확인합니다."

    # feature loop
    - icon: "update"
      title: "서명 관리"
      content: "문서 페이지에 서명이 배치되면 필요에 따라 삭제, 이동 또는 업데이트할 수 있습니다."

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: "Java 작업을 위한 일반적인 GroupDocs.Signature의 일부 사용 사례"
  items:
    # code sample loop
    - title: "QR 코드로 PDF 문서 강화"
      content: |
        PDF 문서의 특정 페이지에 [QR 코드](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/)를 추가하여 비즈니스 프로세스를 향상시키는 것이 중요할 수 있습니다. Java용 GroupDocs.Signature를 사용하여 QR 코드를 추가하는 방법에 대한 예가 있습니다.
        {{< landing/code title="QR 코드로 PDF 문서 강화">}}
        ```java {style=abap}
        // 서명할 문서를 로드하세요.
        Signature signature = new Signature("file_to_sign.pdf");
        
        // 미리 정의된 텍스트로 QR 코드 옵션 만들기
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // QR 코드 인코딩 유형 및 페이지에서의 위치 구성
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // 문서에 서명하고 결과 파일로 저장
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "디지털 서명을 사용하여 DOCX 보호"
      content: |
        디지털 인증서로 저장된 개인 또는 회사 서명을 사용하여 [문서를 보호](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/)할 수 있습니다. 인증서로 보호된 문서는 서명을 무효화하지 않고는 변경할 수 없습니다.
        {{< landing/code title="디지털 서명을 사용하여 DOCX 보호">}}
        ```java {style=abap}   
        // 디지털 서명할 문서를 로드합니다.
        Signature signature = new Signature("file_to_sign.docx");
        
        // 디지털 서명 옵션을 지정하고 인증서 파일의 경로를 제공하세요.
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // 인증서 비밀번호 설정
        options.setPassword("1234567890");

        // 문서에 서명하고 원하는 경로에 저장하세요.
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---
