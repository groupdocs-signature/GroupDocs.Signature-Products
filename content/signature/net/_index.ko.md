---
############################# Static ############################
layout: "landing"
date: 2023-10-23T14:58:09
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
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, Cloud API 및 온라인 문서 서명 앱"
head_description: ".NET, Java 및 클라우드 기반 애플리케이션을 위한 올인원 문서 전자 서명 솔루션을 받으세요. 간단한 드래그 앤 드롭 기능을 사용하여 일반적인 문서 형식에 온라인으로 서명"

############################# Header ############################
title: "문서에 서명<br>.NET API를 통해"
description: "프로그래머와 최종 사용자를 위한 유연한 API 및 앱 기반 솔루션을 사용하여 모든 플랫폼에서 디지털 문서 및 이미지에 서명하십시오."
words:
  for: "~을 위한"

actions:
  main: "무료 NuGet 다운로드"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "라이선스"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Signature 기능을 무료로 사용해 보거나 라이센스를 요청하세요"

release:
  title: "버전 {0} 출시됨"
  notes: "새로운 소식 보기"
  downloads: "다운로드"

code:
  title: "C#에서 PDF 파일 서명"
  more: "더 많은 예시"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // PDF 문서 선택
    using (Signature signature = new Signature("sample.pdf"))
    {
        // 텍스트 제공
        var options = new TextSignOptions("John Smith")
        {
            // 색상 설정
            ForeColor = Color.Red
        };
        // 문서에 서명하고 파일에 저장
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature 개요"
  description: ".NET 애플리케이션에서 문서 서명 및 관련 작업을 수행하기 위한 API"
  features:
    # feature loop
    - title: "C#에서 비즈니스 문서에 서명 추가"
      content: "문서 서명: .NET용 GroupDocs.Signature를 사용하면 텍스트, 이미지, 바코드, 디지털 인증서 등 다양한 유형의 서명을 PDF 및 Office 문서에 추가할 수 있습니다. 이 API를 사용하면 숨겨진 메타데이터를 포함하여 거의 모든 데이터 유형으로 문서에 서명할 수 있습니다."

    # feature loop
    - title: "서명된 문서 처리"
      content: "추가 처리: GroupDocs.Signature를 사용하여 서명된 문서에 대해 강력한 작업을 수행할 수 있습니다. 여기에는 비즈니스 문서 내의 기존 서명을 검색하고 특정 기준을 사용하여 이를 확인하는 것이 포함됩니다. 또한 이 .NET API를 통해 문서 정보 및 미리보기 페이지를 검색할 수 있습니다."

    # feature loop
    - title: "결과 맞춤설정"
      content: ".NET용 GroupDocs.Signature는 광범위한 사용자 정의 옵션을 제공합니다. 문서 페이지의 어느 위치에나 서명을 정확하게 배치하고 다양한 설정을 사용하여 서명 모양을 조정할 수 있습니다. 또한 이 API는 처리된 문서를 다양한 지원 형식으로 저장할 수 있도록 지원합니다."

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: ".NET용 GroupDocs.Signature는 다음 운영 체제, 프레임워크 및 패키지 관리자를 지원합니다."
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
    .NET용 GroupDocs.Signature는 다음 [파일 형식](https://docs.groupdocs.com/signature/net/supported-document-formats/)을 사용한 작업을 지원합니다.
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
  description: "PDF, Office 문서 및 이미지에 신속하고 정확하게 서명"

  items:
    # feature loop
    - icon: "sign"
      title: "문서 서명"
      content: "비즈니스 문서의 지정된 위치에 하나 이상의 지원되는 서명 유형을 정확하게 추가하세요."

    # feature loop
    - icon: "custom"
      title: "서명 사용자 정의"
      content: "색상, 글꼴, 테두리, 회전 등의 기능을 활용하여 서명의 모양을 구성합니다."

    # feature loop
    - icon: "password"
      title: "문서 비밀번호 보호"
      content: "서명 후 비밀번호를 설정하여 특정 문서 유형을 보호하세요."

    # feature loop
    - icon: "protect"
      title: "변경으로부터 보호"
      content: "디지털 인증서로 서명을 추가한 후 중요한 비즈니스 문서가 변경되는 것을 방지하세요."

    # feature loop
    - icon: "convert"
      title: "서명된 파일을 다른 형식으로 변환"
      content: "Word 문서를 PDF로 저장하는 등 서명된 파일을 원하는 형식으로 변환합니다."

    # feature loop
    - icon: "preview"
      title: "페이지 미리보기 추출"
      content: "향후 처리를 위해 서명된 문서의 페이지를 개별 이미지로 추출합니다."

    # feature loop
    - icon: "search"
      title: "문서에서 서명 검색"
      content: "특정 문서에 이전에 추가된 서명에 대한 정보를 검색합니다."

    # feature loop
    - icon: "validate"
      title: "서명된 문서 유효성 검사"
      content: "유효성 검사 기능을 사용하여 문서의 올바른 서명을 확인하세요."

    # feature loop
    - icon: "update"
      title: "서명 업데이트 또는 삭제"
      content: "페이지에서 특정 서명의 위치를 ​​쉽게 변경하고, 텍스트를 수정하고, 문제 없이 삭제할 수 있습니다."

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: ".NET 작업을 위한 일반적인 GroupDocs.Signature의 일부 사용 사례"
  items:
    # code sample loop
    - title: "PDF에 QR 코드 추가"
      content: |
        PDF 문서의 특정 페이지에 [QR 코드](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/)를 추가하면 비즈니스 프로세스를 향상할 수 있습니다. 다음은 GroupDocs.Signature를 사용하여 QR 코드를 추가하는 방법의 예입니다.
        {{< landing/code title="QR 코드를 PDF에 넣는 방법.">}}
        ```csharp {style=abap}
        // 서명할 문서를 로드하세요.
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // 미리 정의된 텍스트로 QR 코드 옵션 만들기
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // QR 코드 인코딩 유형 및 페이지에서의 위치 구성
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // 문서에 서명하고 결과 파일로 저장
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "디지털 인증서를 사용하여 DOCX 문서 보호"
      content: |
        디지털 인증서로 저장된 개인 또는 회사 서명을 사용하여 [문서를 보호](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/)할 수 있습니다. 이러한 보호된 문서는 서명을 무효화하지 않고는 수정할 수 없습니다.
        {{< landing/code title="문서 무결성을 보장하는 방법은 다음과 같습니다.">}}
        ```csharp {style=abap}   
        // 디지털 서명할 문서를 로드합니다.
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // 디지털 서명 옵션을 지정하고 인증서 파일의 경로를 제공하세요.
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // 인증서 비밀번호 설정
                Password = "1234567890"
            };
            // 문서에 서명하고 원하는 경로에 저장하세요.
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
