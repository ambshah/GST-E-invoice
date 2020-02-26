# GST-E-invoice[link-e-invoice]
Code and Documentation on my journey to Enable GST E invoicing IRN and QR Code

Portal Address for the documentation is https://einv-apisandbox.nic.in

Step1 Read the documentation at the link above. 

Summary: Registered tax payers are only allowed to register. Registration has some prerequisites. 

IT Act 2000 (43A) Compliance by organization. 

Basically says that the data inside organization needs to be properly protected, Also take all precautions to prevent viruses and malaware. 

Auth token expires in 6 hours. store it for requests that are within this time span. you can refresh the token 10 minutes before expiry.

request headers are individual parameters. 
Request body is a base 64 encoded json object with a single property called "data"

Success Respose is also a JSON object with properties

* AckNo
* AckDt
* Irn
* SignedInvoice
* SignedQRCode
* Status

Error Respose is also a JSON object with properties
* status
* Data
* Error Details
* info

Schema and validations are available at https://einv-apisandbox.nic.in/version1.00/generate-irn.html#requestPayload
(#link-e-invoice)
