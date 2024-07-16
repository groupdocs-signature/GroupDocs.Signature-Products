---
############################# Static ############################
layout: "family"
date:  2024-07-16T12:27:51
draft: false

product: "Signature"
product_tag: "signature"

lang: ko

############################# Head ############################
head_title: "C# .NET, Java, Node.js 디지털 서명 앱"
head_description: "GroupDocs.Signature을(를) 사용하여 .NET, Java 또는 Node.js 애플리케이션의 전자 서명을 통합하세요. 널리 사용되는 비즈니스 문서 형식에 서명하세요."

############################# Header ############################
title: "문서전자서명 솔루션"
description:  |
  프로그래머와 최종 사용자를 위한 유연한 API와 앱 기반 솔루션을 사용하여 모든 플랫폼에서 디지털 문서와 이미지에 서명하세요.

  고급 방법을 사용하여 이전에 추가된 서명을 검색하고 수정합니다.

  디지털 인증서를 사용하여 문서가 변경되지 않도록 보호하고 숨겨진 메타데이터를 제어하세요.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "플랫폼을 선택하세요"
  title: "플랫폼 독립성"
  description: "GroupDocs.Signature 라이브러리는 다음 운영 체제 및 프레임워크를 지원합니다."
  details_link_title: "더 알아보기"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Signature .NET 
      color: "blue"
      tag: "net"
      link: "/signature/net/"
      features_link: "https://docs.groupdocs.com/signature/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.6.2 or higher <br> .NET Core 3.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS <br> Microsoft Azure
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Signature Java
      color: "red"
      tag: "java"
      link: "/signature/java/"
      features_link: "https://docs.groupdocs.com/signature/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 8 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Signature Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/signature/nodejs-java/"
      features_link: "https://docs.groupdocs.com/signature/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> 다른 텍스트 편집기
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Signature 주요 기능"
  description: "당사의 솔루션은 널리 사용되는 문서 및 파일 형식에 다양한 유형의 서명을 추가하도록 설계되었습니다. 귀하의 비즈니스 프로세스를 쉽게 강화하십시오."

  items:
    # items loop
    - icon: "additional"
      title: "서명으로 데이터를 풍부하게 만드세요"
      content: "비즈니스 문서에 텍스트, 이미지, 워터마크 등을 추가하세요."

    # items loop
    - icon: "protect"
      title: "문서 내용 보호"
      content: "디지털 인증서로 문서를 봉인하여 문서 변경을 금지합니다."

    # items loop
    - icon: "search"
      title: "숨겨진 데이터 및 바코드 추가"
      content: "메타데이터를 사용하여 눈에 보이지 않는 정보를 저장하거나 페이지에 사용자 정의 바코드를 삽입하세요."

    # items loop
    - icon: "manipulate"
      title: "서명 조작"
      content: "이전에 추가된 모든 서명을 검색, 업데이트 또는 삭제합니다."

############################# Code samples ############################
code_samples:
  enable: true
  title: "서명을 사용하여 파일을 보호하세요"
  description: "GroupDocs.Signature 코드 예시"
  items:
    # code sample loop
    - title: "QR 코드 생성 및 추가"
      content: |
       GroupDocs.Signature을(를) 사용하면 지원되는 형식의 문서에 QR 코드를 생성하고 추가할 수 있습니다. 서명이 필요한 문서의 경로를 제공하고 QR 코드의 원하는 텍스트 및 시각적 옵션을 설정하세요. 생성된 QR 코드 이미지를 문서 페이지의 어느 영역에나 배치할 수 있습니다.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // 서명할 문서 지정
            using (Signature signature = new Signature("source.docx"))
            {
                // QR 코드 서명 옵션 만들기
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // QR 코드 옵션 설정
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150,
                };

                // 처리된 파일 서명 및 저장
                SignResult result = signature.Sign("result.docx", options);
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // 서명할 문서 지정
            Signature signature = new Signature("source.docx");

            // QR 코드 서명 옵션 만들기
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith");

            // QR 코드 옵션 설정
            options.setEncodeType(QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // 처리된 파일 서명 및 저장
            signature.sign("result.docx", options);
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            const signatureLib = require('@groupdocs/groupdocs.signature')

            // 서명할 문서 지정
            const signature = new signatureLib.Signature('source.docx');

            // QR 코드 서명 옵션 만들기
            const options = new signatureLib.QrCodeSignOptions('JohnSmith');

            // QR 코드 옵션 설정
            options.setEncodeType(signatureLib.QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // 처리된 파일 서명 및 저장
            signature.sign('result.docx', options);
            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "60개 이상의 파일 형식이 지원됩니다"
  description: "GroupDocs.Signature은 거의 모든 널리 사용되는 파일 형식을 지원합니다"

############################# Metrics ###############################
metrics:
  enable: true
  title: "우리 도서관 통계자료"
  description: "주요 제품 측정항목을 검사하여 당사의 성과, 영향력, 성장에 대한 통찰력을 얻으세요"

  items:
    # items loop
    - number: "50+"
      title: "지원되는 형식"
      content: "60개 이상의 가장 널리 사용되는 비즈니스 파일 형식에 서명합니다."

    # items loop
    - number: "500k"
      title: "NuGet 다운로드"
      content: ".NET용 GroupDocs.Signature은 NuGet에서 550,000회 이상 다운로드된 인기 라이브러리입니다."

    # items loop
    - number: "15k"
      title: "메이븐 다운로드"
      content: "Java 개발자는 Maven에서 15,000회 이상 GroupDocs.Signature을(를) 다운로드했습니다."

    # items loop
    - number: "140+"
      title: "행복한 고객"
      content: "개별 개발자와 전 세계 최고의 기업은 당사 제품을 사용하여 혁신적인 솔루션을 구축합니다."


############################# Customers ###############################
customers:
  enable: true
  title: "우리의 행복한 고객"
  description: "GroupDocs 라이브러리는 전 세계적으로 유명하고 뛰어난 브랜드에서 사용됩니다"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "귀하의 플랫폼에서 무료로 GroupDocs.Signature 기능을 사용해 보세요"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/signature/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/signature/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/signature/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "자주 묻는 질문"
  description: "자주 묻는 질문(FAQ) 살펴보기"

  items:
    # items loop
    - question: "GroupDocs.Signature에는 문서 서명을 위해 외부 라이브러리가 필요합니까?"
      answer: "아니요, GroupDocs.Signature은(는) 독립적으로 작동합니다. Adobe Acrobat, Microsoft Office 등과 같은 타사 종속성은 없습니다."

    # items loop
    - question: "구매하기 전에 GroupDocs.Signature 기능을 테스트할 수 있나요?"
      answer: "전적으로! GroupDocs.Signature에서는 무료 평가판을 제공합니다. 설치하고 기능을 살펴보세요. 평가판 버전은 문서에 '평가판 배지'를 추가하고 처음 3페이지만 처리한다는 점에 유의하세요. 전체 기능을 경험하려면 모든 기능에 액세스할 수 있는 30일 무료 임시 라이선스를 취득하세요. [임시 라이선스](https://purchase.groupdocs.com/temporary-license/)에서 자세한 내용을 확인하세요."

    # items loop
    - question: "어떤 라이선스 유형이 제공되나요?"
      answer: "GroupDocs.Signature 라이선스를 찾고 계십니까? 우리는 귀하의 요구에 맞는 다양한 옵션을 제공합니다. 팀 규모, 배포 위치(단일 사무실 또는 원격 작업장), 최종 고객 배포에 SDK/API를 클라이언트와 공유해야 하는지 여부를 기준으로 선택하세요. 또는 계량 플랜이 포함된 월간 사용 라이선스를 선택하세요. 사용한 만큼만 비용을 지불하세요. [가격](https://purchase.groupdocs.com/pricing/signature/net/)에서 귀하에게 가장 적합한 제품을 찾아보세요."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Signature 로우 코드 API"
  description: "클라우드 기반 REST API를 통해 애플리케이션을 사용하여 파일에 서명하세요."
  
  items:
    # items loop
    - title: "GroupDocs.Signature Cloud for cURL"
      content: "cURL RESTful API를 사용하여 PDF, Word, Excel, PowerPoint, JPEG 및 기타 다양한 파일 형식에 서명을 추가하세요."
      icon: "groupdocs_signature-for-curl"
      link: "https://products.groupdocs.cloud/signature/curl"

    # items loop
    - title: "GroupDocs.Signature Cloud for .NET"
      content: "Cloud SDK를 통한 문서 서명으로 .NET 애플리케이션을 강화하세요. 자신만의 방식으로 비즈니스 문서를 보호하세요."
      icon: "groupdocs_signature-for-net"
      link: "https://products.groupdocs.cloud/signature/net"

    # items loop
    - title: "GroupDocs.Signature Cloud for Java"
      content: "GroupDocs.Signature SDK는 Java 애플리케이션이 모든 파일에 서명할 수 있는 다양한 가능성에 대한 액세스를 부여합니다."
      icon: "groupdocs_signature-for-java"
      link: "https://products.groupdocs.cloud/signature/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Signature 웹 앱"
  description: "GroupDocs.Signature은 문서에 서명할 수 있는 무료 웹 애플리케이션을 제공합니다. 60개 이상의 인기 있는 파일 형식을 즐겨 사용하는 브라우저를 통해 무료로 서명할 수 있습니다."

  items:
    # items loop
    - title: "GroupDocs.Signature Total"
      content: "모든 장치에서 문서에 서명을 추가할 수 있는 온라인 도구입니다."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/signature/total"

    # items loop
    - title: "GroupDocs.Signature DOCX"
      content: "MS Word DOCX에 온라인으로 서명하세요."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/signature/docx"

    # items loop
    - title: "GroupDocs.Signature PDF"
      content: "PDF 문서를 온라인으로 보호하세요."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/signature/pdf"


      


---