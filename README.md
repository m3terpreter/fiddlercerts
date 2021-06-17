# fiddlercerts
For Android >= 7.0,the certificate will be installed by USER but SYSTEM
So after exporting fiddler certificate to desktop,you need to transfer it to another form.
Use
`openssl x509 -subject_hash_old -in 123.pem`
and
`adb push ab6544ad.0 /system/etc/security/cacerts/ `
