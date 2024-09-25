---
############################# Static ############################
layout: "landing"
date: 2024-09-25T13:59:03
draft: false

lang: ko
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

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
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"  

############################# Head ############################
head_title: "{index-content-python-net.head_title}"
head_description: "{index-content-python-net.head_description}"

############################# Header ############################
title: "{index-content-python-net.title}"
description: "{index-content-python-net.description}"
words:
  for: "~을 위한"

actions:
  main: "{index-content-python-net.actions_main}"
  main_link: "https://pypi.org/project/groupdocs-signature-net/"
  alt: "라이선스"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Signature 기능을 무료로 사용해 보거나 라이센스를 요청하세요"

release:
  title: "버전 {0} 출시됨"
  notes: "새로운 소식 보기"
  downloads: "다운로드"

code:
  title: "{index-content-python-net.code_title}"
  more: "더 많은 예시"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
  install: "pip install groupdocs-signature-net"
  content: |
    ```python {style=abap}   
    import groupdocs.signature as sg

    def run():

        # PDF 문서 선택
        with sg.Signature('sample.pdf') as signature:

            # 텍스트 제공
            options = sg.TextSignOptions("John Smith")
    
            # 색상 설정
            options.ForeColor = sg.Color.Red
    
            # 문서에 서명하고 파일에 저장
            signature.Sign('signed.pdf', options)
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature 개요"
  description: "{index-content-python-net.overview_description}"
  features:
    # feature loop
    - title: "{index-content-python-net.overview_feature_1.title}"
      content: "{index-content-python-net.overview_feature_1.description}"

    # feature loop
    - title: "{index-content-python-net.overview_feature_2.title}"
      content: "{index-content-python-net.overview_feature_2.description}"

    # feature loop
    - title: "{index-content-python-net.overview_feature_3.title}"
      content: "{index-content-python-net.overview_feature_3.description}"

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: "{index-content-python-net.platforms_description}"
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
    {index-content-python-net.formats_description}
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
  title: "{index-content-python-net.features.title}"
  description: "{index-content-python-net.features.description}"

  items:
    # feature loop
    - icon: "sign"
      title: "{index-content-python-net.features.feature_1.title}"
      content: "{index-content-python-net.features.feature_1.content}"

    # feature loop
    - icon: "custom"
      title: "{index-content-python-net.features.feature_2.title}"
      content: "{index-content-python-net.features.feature_2.content}"

    # feature loop
    - icon: "password"
      title: "{index-content-python-net.features.feature_3.title}"
      content: "{index-content-python-net.features.feature_3.content}"

    # feature loop
    - icon: "protect"
      title: "{index-content-python-net.features.feature_4.title}"
      content: "{index-content-python-net.features.feature_4.content}"

    # feature loop
    - icon: "convert"
      title: "{index-content-python-net.features.feature_5.title}"
      content: "{index-content-python-net.features.feature_5.content}"

    # feature loop
    - icon: "preview"
      title: "{index-content-python-net.features.feature_6.title}"
      content: "{index-content-python-net.features.feature_6.content}"

    # feature loop
    - icon: "search"
      title: "{index-content-python-net.features.feature_7.title}"
      content: "{index-content-python-net.features.feature_7.content}"

    # feature loop
    - icon: "validate"
      title: "{index-content-python-net.features.feature_8.title}"
      content: "{index-content-python-net.features.feature_8.content}"

    # feature loop
    - icon: "update"
      title: "{index-content-python-net.features.feature_9.title}"
      content: "{index-content-python-net.features.feature_9.content}"

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: "{index-content-python-net.code_samples_description}"
  items:
    # code sample loop
    - title: "{index-content-python-net.code_title_sample_1}"
      content: |
        {index-content-python-net.code_samples_sample_1_content_1} {index-content-python-net.code_samples_sample_1_content_2}
        {{< landing/code title="QR 코드를 PDF에 넣는 방법.">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # 서명할 문서를 로드하세요.
            with sg.Signature('file_to_sign.pdf') as signature:

                # 미리 정의된 텍스트로 QR 코드 옵션 만들기
                options = sg.QrCodeSignOptions('The document is approved by John Smith')
        
                # QR 코드 인코딩 유형 및 페이지에서의 위치 구성
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 100
                options.Top = 100
            
                # 문서에 서명하고 결과 파일로 저장
                signature.Sign('file_with_QR.pdf', options)
        ```
        {{< /landing/code >}}

    # code sample loop
    - title: "{index-content-python-net.code_title_sample_2}"
      content: |
        {index-content-python-net.code_samples_sample_2_content_1} {index-content-python-net.code_samples_sample_2_content_2}
        {{< landing/code title="문서 무결성을 보장하는 방법은 다음과 같습니다.">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # 디지털 서명할 문서를 로드합니다.
            with sg.Signature('file_to_sign.docx') as signature:
        
                # 디지털 서명 옵션을 지정하고 인증서 파일의 경로를 제공하세요.
                options = sg.DigitalSignOptions('certificate.pfx')

                # 인증서 비밀번호 설정
                options.Password = '1234567890'

                # 문서에 서명하고 원하는 경로에 저장하세요.
                signature.Sign('digitally_signed.docx', options)
        ```
        {{< /landing/code >}}

---
