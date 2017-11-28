# .NetFramwork
123456

makecert -sky exchange -pe -r -n "CN=SelfCertificateRoot" -a sha256 -len 2048 -ss My "MyRoot.cer"
makecert -sky exchange -pe -is my -in "SelfCertificateRoot" -n "CN=MyPc" -a sha256 -len 2048 -ss My
