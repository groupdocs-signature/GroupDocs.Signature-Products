    items: 
          
        # operation loop 1
        - name: "<% "{common-content.operations.esign.name}" %>"
          operation: "esign"
          link: "/signature/<% get "ProdCode" %>/esign/<% get "OperationUrl" %>/"
          description: "<% "{common-content.operations.esign.description}" %>"

        # operation loop 2
        - name: "<% "{common-content.operations.text.name}" %>"
          operation: "text"
          link: "/signature/<% get "ProdCode" %>/text/<% get "OperationUrl" %>/"
          description: "<% "{common-content.operations.text.description}" %>"

        # operation loop 3
        - name: "<% "{common-content.operations.image.name}" %>"
          operation: "image"
          link: "/signature/<% get "ProdCode" %>/image/<% get "OperationUrl" %>/"
          description: "<% "{common-content.operations.image.description}" %>"

        # operation loop 4
        - name: "<% "{common-content.operations.barcode.name}" %>"
          operation: "barcode"
          link: "/signature/<% get "ProdCode" %>/barcode/<% get "OperationUrl" %>/"
          description: "<% "{common-content.operations.barcode.description}" %>"

        # operation loop 5
        - name: "<% "{common-content.operations.qrcode.name}" %>"
          operation: "qrcode"
          link: "/signature/<% get "ProdCode" %>/qrcode/<% get "OperationUrl" %>/"
          description: "<% "{common-content.operations.qrcode.description}" %>"
          
        # operation loop 6
        - name: "<% "{common-content.operations.digital.name}" %>"
          operation: "digital"
          link: "/signature/<% get "ProdCode" %>/digital/<% get "OperationUrl" %>/"
          description: "<% "{common-content.operations.digital.description}" %>"

        # operation loop 7
        - name: "<% "{common-content.operations.stamp.name}" %>"
          operation: "stamp"
          link: "/signature/<% get "ProdCode" %>/stamp/<% get "OperationUrl" %>/"
          description: "<% "{common-content.operations.stamp.description}" %>"
          
        # operation loop 8
        - name: "<% "{common-content.operations.search.name}" %>"
          operation: "search"
          link: "/signature/<% get "ProdCode" %>/search/<% get "OperationUrl" %>/"
          description: "<% "{common-content.operations.search.description}" %>"
          
        # operation loop 9
        - name: "<% "{common-content.operations.verify.name}" %>"
          operation: "verify"
          link: "/signature/<% get "ProdCode" %>/verify/<% get "OperationUrl" %>/"
          description: "<% "{common-content.operations.verify.description}" %>"
          
        # operation loop 10
        - name: "<% "{common-content.operations.modify.name}" %>"
          operation: "modify"
          link: "/signature/<% get "ProdCode" %>/modify/<% get "OperationUrl" %>/"
          description: "<% "{common-content.operations.modify.description}" %>"
          
        # operation loop 11
        - name: "<% "{common-content.operations.delete.name}" %>"
          operation: "delete"
          link: "/signature/<% get "ProdCode" %>/delete/<% get "OperationUrl" %>/"
          description: "<% "{common-content.operations.delete.description}" %>"
          