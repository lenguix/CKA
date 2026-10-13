## Generar llave privada para cliente
openssl genrsa -out admintest.key 2048

## Solicitar firma de certificado
openssl req -new -key admintest.key -out admintest.csr -subj "/CN=admintest"