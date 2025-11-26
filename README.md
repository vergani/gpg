# gpg
GPG commands

Criptografia simétrica (senha)
# Encriptar
gpg --symmetric --cipher-algo AES256 meu_arquivo.pdf

# Descriptografar
gpg --output meu_arquivo_decrypted.pdf --decrypt meu_arquivo.pdf.gpg


Criptografia assimétrica “para si mesmo”
# Encriptar (apenas para você)
gpg --output meu_arquivo.pdf.gpg --encrypt --recipient seu@email.com meu_arquivo.pdf

# Encriptar + assinar
gpg --output meu_arquivo.pdf.gpg --encrypt --sign --recipient seu@email.com meu_arquivo.pdf

# Descriptografar
gpg --output meu_arquivo_decrypted.pdf --decrypt meu_arquivo.pdf.gpg
