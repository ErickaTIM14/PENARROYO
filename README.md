*Open file manager and go to the directory where blockchain-training-labs located
*Copy chaincode folder and supply folder
*Paste it inside the fabric-sample

Then open your Terminal and direct to folder "suppy"
Type this on your Teminal 
  type this to terminal

  go get github.com/golang/protobuf/proto
  go get github.com/hyperledger/fabric/common/attrmgr
  go get github.com/pkg/errors
  go get github.com/hyperledger/fabric/core/chaincode/lib/cid
  
  
now open file manager go to Home/go/src/github.com
copy three folders

hyperledger
pkg
golang

paste it inside fabric-sample/chaincode

TYPE THIS ON YOUR TERMINAL:
    ./startFabric.sh
    npm install
    node enrollAdmin.sh
    node registerSupplier.sh
    node registerOem.sh
    node registerBank.sh
    node app
    
 open postman and you should see a GET untitled request
change method from GET to POST
add url localhost:3000/invoice
below url you should see Params Authroization Headers Body
click Headers
Add another key below Content-Type
type user
and the value would be "supplier"
next open the body tab
click the x-www-form-url-encoded
you should see a form there


Type 

KEY                      VALUE

invoicenumber           INVOICE001
billedto                OEM
invoicedate             02/08/19
invoiceamount           10000
itemdescription         KEYBOARD
goodreceived            False
ispaid                  False
paidamount              0
repaid                  False
repaymentamount         0

Then hit Send
