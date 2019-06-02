# Gdrivedl

Script Shell que facilita downloads de arquivos compartilhados do Google Drive via Curl no Linux.

## Getting Started

Baixe o script e torne-o executável.
```
sudo wget -O /usr/sbin/gdrivedl 'https://f.mjh.nz/gdrivedl'
sudo chmod +x /usr/sbin/gdrivedl
```

### Examples

Abaixo estão alguns exemplos dos diferentes URLs com os quais ele trabalhará
```
gdrivedl https://drive.google.com/open?id=1sNhrr2u6n48vb5xuOe8P9pTayojQoOc_
gdrivedl https://drive.google.com/file/d/1sNhrr2u6n48vb5xuOe8P9pTayojQoOc_/view?usp=sharing
gdrivedl 1sNhrr2u6n48vb5xuOe8P9pTayojQoOc_
```
Qualquer um deles irá baixar o arquivo para um arquivo tmp no diretório atual. 
Em seguida, ele tentará obter o nome do arquivo dos cabeçalhos de solicitações e, em seguida, renomear o arquivo. 

Você também pode especificar seu próprio caminho de arquivo de saída como um segundo argumento.
```
gdrivedl https://drive.google.com/open?id=1sNhrr2u6n48vb5xuOe8P9pTayojQoOc_ /tmp/my_file.rar
```
## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

Informações retirado do [site](https://www.matthuisman.nz/2019/01/download-google-drive-files-wget-curl.html) de [Matthuisman](https://github.com/matthuisman)
:.
