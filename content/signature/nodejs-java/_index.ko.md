---
############################# Static ############################
layout: "landing"
date: 2024-03-04T17:52:03
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: ko
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
title: "문서에 서명<br>Node.js API 사용"
description: "프로그래머와 최종 사용자를 위한 유연한 API 및 앱 기반 솔루션을 사용하여 모든 플랫폼에서 디지털 문서 및 이미지에 서명하십시오."
words:
  for: "~을 위한"

actions:
  main: "NPM에서 다운로드"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "라이선스"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Signature 기능을 무료로 사용해 보거나 라이센스를 요청하세요"

release:
  title: "버전 {0} 출시됨"
  notes: "새로운 소식 보기"
  downloads: "다운로드"

code:
  title: "Node.js로 PDF에 서명하기"
  more: "더 많은 예시"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```javascript {style=abap}   
    // PDF 문서 선택
    let signature = new Signature("sample.pdf");
    
    // 텍스트 제공
    let options = new TextSignOptions("John Smith");
    
    // 색상 설정
    options.ForeColor = Color.Red;
    
    // 문서에 서명하고 파일에 저장
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature 개요"
  description: "Node.js 애플리케이션에서 사용할 준비가 된 문서 서명 라이브러리"
  features:
    # feature loop
    - title: "Node.js를 사용한 비즈니스 문서용 디지털 서명 솔루션"
      content: "GroupDocs.Signature for Node.js via Java은 PDF, Office 문서 및 이미지에 대한 포괄적인 디지털 서명 옵션 세트를 제공합니다. 텍스트, 바코드, 이미지, 디지털 인증서 및 메타데이터를 사용할 수 있습니다. 간소화된 문서 처리로 효율성이 보장됩니다."

    # feature loop
    - title: "서명된 문서의 고급 조작"
      content: "GroupDocs.Signature을(를) 사용하면 서명된 문서를 처리할 수 있습니다. 다양한 기준을 사용하여 서명을 검색하고 유효성을 검사합니다. 또한, 상세한 문서 정보를 추출하거나 페이지의 미리보기 이미지를 생성합니다."

    # feature loop
    - title: "다양한 출력 형식"
      content: "당사의 솔루션은 서명된 문서의 출력 형식을 광범위하게 제어할 수 있습니다. 모든 페이지에 서명을 정확하게 배치하고 모양을 사용자 정의하세요. 서명된 문서를 지원되는 다양한 형식으로 저장하고 선택적으로 비밀번호로 보안을 설정하세요."

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: "GroupDocs.Signature for Node.js via Java은(는) 다양한 운영 체제로 문서 처리를 수행합니다."
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "지원되는 파일 형식"
  description: |
    GroupDocs.Signature for Node.js via Java은 [인기 있는 파일 형식](https://docs.groupdocs.com/signature/java/supported-document-formats/)에 대한 작업을 용이하게 합니다.
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
  title: "GroupDocs.Signature의 기능"
  description: "디지털 서명으로 PDF, Office 문서 및 이미지에 서명"

  items:
    # feature loop
    - icon: "sign"
      title: "비즈니스 서명"
      content: "문서에 서명하려면 다양한 서명 유형을 사용하십시오. 모든 페이지 위치에 디지털 서명을 정확하게 배치합니다."

    # feature loop
    - icon: "custom"
      title: "시그니처 모양 사용자 정의"
      content: "색상, 글꼴, 테두리, 회전 등을 조정하여 서명의 시각적 측면을 조정하여 원하는 결과를 얻으세요."

    # feature loop
    - icon: "password"
      title: "비밀번호로 보호된 문서"
      content: "지원되는 다양한 문서 형식의 경우 추가 보안을 위해 비밀번호로 서명된 문서를 보호하세요."

    # feature loop
    - icon: "protect"
      title: "무단 수정 방지"
      content: "디지털 인증서로 서명된 중요한 비즈니스 문서를 무단 변경으로부터 보호하세요."

    # feature loop
    - icon: "convert"
      title: "원하는 출력 형식"
      content: "지원되는 모든 형식으로 서명된 문서를 쉽게 얻을 수 있습니다. MS Word 문서를 PDF 형식으로 쉽게 변환하세요."

    # feature loop
    - icon: "preview"
      title: "문서 미리보기"
      content: "향후 필요에 대비해 개별 문서 페이지를 이미지로 저장하세요."

    # feature loop
    - icon: "search"
      title: "서명 검색"
      content: "문서 내에서 이전에 추가된 서명에 대한 정보를 검색합니다."

    # feature loop
    - icon: "validate"
      title: "문서 검증"
      content: "모든 문서에 표시된 서명의 진위 여부를 확인하세요."

    # feature loop
    - icon: "update"
      title: "서명 관리"
      content: "문서 페이지에 있는 서명을 삭제, 재배치 또는 수정합니다."

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: "일반적인 GroupDocs.Signature for Node.js via Java 작업을 보여주는 예시"
  items:
    # code sample loop
    - title: "QR 코드로 PDF 표시"
      content: |
        [바코드](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/)를 특정 PDF 문서 페이지에 통합하면 비즈니스 프로세스를 간소화할 수 있습니다. 이 섹션에서는 GroupDocs.Signature for Node.js via Java을(를) 사용하여 QR 코드를 추가하는 예를 제공합니다.
        {{< landing/code title="QR 코드를 PDF에 넣는 방법.">}}
        ```javascript {style=abap}
        // 서명할 문서를 로드하세요.
        let signature = new Signature("file_to_sign.pdf");
        
        // 미리 정의된 텍스트로 QR 코드 옵션 만들기
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // QR 코드 인코딩 유형 및 페이지에서의 위치 구성
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // 문서에 서명하고 결과 파일로 저장
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "디지털 서명으로 DOCX 보호"
      content: |
        디지털 인증서를 기반으로 한 서명으로 [문서를 보호](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/)하세요. 디지털 서명은 내용 변경으로부터 비즈니스 문서를 보호합니다.
        {{< landing/code title="문서 무결성을 보장하는 방법은 다음과 같습니다.">}}
        ```javascript {style=abap}   
        // 디지털 서명할 문서를 로드합니다.
        let signature = new Signature("file_to_sign.pdf");
        
        // 디지털 서명 옵션을 지정하고 인증서 파일의 경로를 제공하세요.
        let options = new DigitalSignOptions("certificate.pfx");

        // 인증서 비밀번호 설정
        options.Password = "1234567890";

        // 문서에 서명하고 원하는 경로에 저장하세요.
        signature.Sign("digitally_signed.pdf", options);

        ```
        {{< /landing/code >}}

---
