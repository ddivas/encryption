# encryption
#Encrypted files for emapp
# First decrypt then check checksum for file integrity


#1. Decrypt using:

$ gpg -o private_key.pepk -d private_key.pepk.gpg
$ gpg -o google_services.json -d google_services.json.gpg


#2. sha256sum checksum of decrypted file:

$ sha256sum private_key.pepk
$ sha256sum google_services.json

#output:

private_key.pepk: c1b2303f8652b4cd0cf4a7eba92a8b902977b07c4e96f28df9566e2963e3b440
google_services.json: f46aa78bd1f7805734e78055d4e7ba8b4320ab284cb18c53d02a6a68236f7149
