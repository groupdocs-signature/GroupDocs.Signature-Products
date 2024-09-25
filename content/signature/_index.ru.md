---
############################# Static ############################
layout: "family"
date:  2024-09-25T12:45:24
draft: false

product: "Signature"
product_tag: "signature"

lang: ru

############################# Head ############################
head_title: "C# .NET, Java, приложения для цифровой подписи Node.js"
head_description: "Интегрируйте электронные подписи в приложения .NET, Java или Node.js с помощью GroupDocs.Signature. Подписывайте популярные форматы деловых документов."

############################# Header ############################
title: "Решение для электронной подписи документов"
description:  |
  Подписывайте цифровые документы и изображения на любой платформе, используя наши гибкие API и решения на базе приложений для программистов и конечных пользователей.

  Найдите и измените ранее добавленные подписи, используя расширенные методы.

  Защитите документы от изменений с помощью цифровых сертификатов и контролируйте скрытые метаданные.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Выберите свою платформу"
  title: "Независимость от платформы"
  description: "Библиотека GroupDocs.Signature поддерживает следующие операционные системы и платформы:"
  details_link_title: "Узнать больше"

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
                    Atom <br> Visual Studio Code <br> Любой другой текстовый редактор
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Python"
      description: GroupDocs.Signature Python
      color: "yellow"
      tag: "python-net"
      link: "/signature/python-net/"
      features_link: "https://docs.groupdocs.com/signature/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Python 3.9+ and .Net 6+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IDLE <br> PyCharm <br> Visual Studio Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

############################# Features ###############################
features:
  enable: true
  title: "Основные функции GroupDocs.Signature"
  description: "Наше решение предназначено для добавления различных типов подписей к популярным форматам документов и файлов. Легко обогатите свои бизнес-процессы."

  items:
    # items loop
    - icon: "additional"
      title: "Дополните свои данные подписями"
      content: "Добавляйте текст, изображения, водяные знаки и т. д. в свои деловые документы."

    # items loop
    - icon: "protect"
      title: "Защитите содержимое документов"
      content: "Запретите изменение документа, запечатав его цифровым сертификатом."

    # items loop
    - icon: "search"
      title: "Добавляйте скрытые данные и штрих-коды"
      content: "Используйте метаданные для хранения невидимой информации или размещайте на страницах собственные штрих-коды."

    # items loop
    - icon: "manipulate"
      title: "Манипулировать подписями"
      content: "Найдите, обновите или удалите все подписи, добавленные ранее."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Защитите свои файлы с помощью подписей"
  description: "Примеры кода GroupDocs.Signature"
  items:
    # code sample loop
    - title: "Сгенерируйте и добавьте QR-код"
      content: |
       GroupDocs.Signature позволяет нам генерировать и добавлять QR-коды в документы поддерживаемых форматов. Укажите путь к документу, который необходимо подписать, и настройте нужные текстовые и визуальные параметры QR-кода. Вы можете поместить сгенерированное изображение QR-кода в любую область любой страницы документа.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Укажите документ для подписания
            using (Signature signature = new Signature("source.docx"))
            {
                // Создать варианты подписи QR-кода
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // Установите параметры QR-кода
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150,
                };

                // Подпишите и сохраните обработанный файл
                SignResult result = signature.Sign("result.docx", options);
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Укажите документ для подписания
            Signature signature = new Signature("source.docx");

            // Создать варианты подписи QR-кода
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith");

            // Установите параметры QR-кода
            options.setEncodeType(QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Подпишите и сохраните обработанный файл
            signature.sign("result.docx", options);
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            const signatureLib = require('@groupdocs/groupdocs.signature')

            // Укажите документ для подписания
            const signature = new signatureLib.Signature('source.docx');

            // Создать варианты подписи QR-кода
            const options = new signatureLib.QrCodeSignOptions('JohnSmith');

            // Установите параметры QR-кода
            options.setEncodeType(signatureLib.QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Подпишите и сохраните обработанный файл
            signature.sign('result.docx', options);
            ```
        - language: "Python"
          color: "yellow"
          content: |
            ```python {style=abap}  
            import groupdocs.signature as sg

            def run():

                # Укажите документ для подписания
                with sg.Signature('source.docx') as signature:

                    # Создать варианты подписи QR-кода
                    options = sg.QrCodeSignOptions('JohnSmith')

                    # Установите параметры QR-кода
                    options.setEncodeType(sg.QrCodeTypes.QR)
                    options.setLeft(50)
                    options.setTop(100)

                    # Подпишите и сохраните обработанный файл
                    signature.sign('result.docx', options)
            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "Поддерживается более 60 форматов файлов"
  description: "GroupDocs.Signature поддерживает практически все популярные форматы файлов"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Статистические данные нашей библиотеки"
  description: "Изучите ключевые показатели продукта, чтобы получить представление о наших достижениях, влиянии и росте"

  items:
    # items loop
    - number: "50+"
      title: "Поддерживаемые форматы"
      content: "Подписание более 60 самых популярных форматов бизнес-файлов."

    # items loop
    - number: "500k"
      title: "Загрузки NuGet"
      content: "GroupDocs.Signature для .NET — популярная библиотека, которую на NuGet скачали более 550 000 раз."

    # items loop
    - number: "15k"
      title: "Загрузки Maven"
      content: "Разработчики Java загрузили GroupDocs.Signature на Maven более 15 тысяч раз."

    # items loop
    - number: "140+"
      title: "Счастливые клиенты"
      content: "Отдельные разработчики и ведущие компании по всему миру используют наши продукты для создания инновационных решений."


############################# Customers ###############################
customers:
  enable: true
  title: "Наши счастливые клиенты"
  description: "Библиотеки GroupDocs используются всемирно известными и выдающимися брендами по всему миру"

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
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Signature бесплатно на своей платформе."

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
  title: "Часто задаваемые вопросы"
  description: "Изучите наши часто задаваемые вопросы"

  items:
    # items loop
    - question: "Нужна ли GroupDocs.Signature внешняя библиотека для подписи документов?"
      answer: "Нет, GroupDocs.Signature работает независимо. Нет сторонних зависимостей, таких как Adobe Acrobat, Microsoft Office и т. д."

    # items loop
    - question: "Можно ли протестировать функции GroupDocs.Signature перед покупкой?"
      answer: "Абсолютно! GroupDocs.Signature предлагает бесплатную пробную версию. Установите его и изучите его возможности. Обратите внимание, что пробные версии добавляют к вашим документам «пробные значки» и обрабатывают только первые три страницы. Чтобы получить все возможности, получите бесплатную 30-дневную временную лицензию для доступа ко всем функциям. Подробности см. в разделе [временная лицензия](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Какие типы лицензий предоставляются?"
      answer: "Ищете лицензию GroupDocs.Signature? Мы предлагаем различные варианты с учетом ваших потребностей. Выбирайте в зависимости от размера команды, места развертывания (отдельный офис или удаленные рабочие места), а также того, требует ли распространение среди конечных пользователей совместного использования SDK/API с клиентами. Альтернативно, выберите ежемесячную лицензию на использование с тарифными планами — платите только за то, что вы используете. Найдите наиболее подходящий вариант в разделе [pricing](https://purchase.groupdocs.com/pricing/signature/net/)."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Signature API с низким кодом"
  description: "Подписывайте файлы с помощью своего приложения через наш облачный REST API."
  
  items:
    # items loop
    - title: "GroupDocs.Signature Cloud for cURL"
      content: "Используйте cURL RESTful API для проставления подписей в файлах PDF, Word, Excel, PowerPoint, JPEG и многих других форматах."
      icon: "groupdocs_signature-for-curl"
      link: "https://products.groupdocs.cloud/signature/curl"

    # items loop
    - title: "GroupDocs.Signature Cloud for .NET"
      content: "Расширьте возможности своих .NET-приложений, подписав документы с помощью Cloud SDK. Защитите деловые документы по-своему."
      icon: "groupdocs_signature-for-net"
      link: "https://products.groupdocs.cloud/signature/net"

    # items loop
    - title: "GroupDocs.Signature Cloud for Java"
      content: "GroupDocs.Signature SDK предоставляет вашим Java-приложениям доступ к различным возможностям подписи любых файлов."
      icon: "groupdocs_signature-for-java"
      link: "https://products.groupdocs.cloud/signature/java"

############################# App links ###############################
app_links:
  enable: true
  title: "Веб-приложения GroupDocs.Signature"
  description: "GroupDocs.Signature представляет бесплатное веб-приложение, с помощью которого вы можете подписывать документы. Более 60 популярных форматов файлов можно БЕСПЛАТНО подписать через ваш любимый браузер."

  items:
    # items loop
    - title: "GroupDocs.Signature Total"
      content: "Онлайн-инструмент для постановки подписей на документах с любого устройства."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/signature/total"

    # items loop
    - title: "GroupDocs.Signature DOCX"
      content: "Подпишите MS Word DOCX онлайн."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/signature/docx"

    # items loop
    - title: "GroupDocs.Signature PDF"
      content: "Защитите PDF-документы онлайн."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/signature/pdf"


      


---