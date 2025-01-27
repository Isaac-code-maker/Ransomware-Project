# Ransomware Troll

Este repositório contém dois scripts Python simples que demonstram o processo de criptografia e descriptografia de arquivos usando a biblioteca `pyaes`. Eles foram desenvolvidos apenas para fins educacionais e para explorar conceitos de segurança da informação. **Não use esses scripts para fins maliciosos.**

## Descrição

Os scripts permitem:

1. Criptografar o conteúdo de um arquivo de texto específico.
2. Descriptografar o arquivo previamente criptografado, retornando ao seu estado original.

## Pré-requisitos

Antes de executar os scripts, certifique-se de que você tenha:

- Python 3 instalado.
- A biblioteca `pyaes` instalada. Para instalá-la, execute:
  ```bash
  pip install pyaes
  ```

## Scripts

### 1. Criptografia (`encrypt.py`)

Este script realiza os seguintes passos:

1. Lê o conteúdo de um arquivo de texto (`teste.txt`).
2. Remove o arquivo original.
3. Criptografa os dados usando o algoritmo AES (CTR mode) com uma chave de 16 bytes.
4. Salva os dados criptografados em um novo arquivo com a extensão `.ransomwaretroll`.

### 2. Descriptografia (`decrypt.py`)

Este script realiza os seguintes passos:

1. Lê o conteúdo de um arquivo previamente criptografado (`teste.txt.ransomwaretroll`).
2. Remove o arquivo criptografado.
3. Descriptografa os dados usando a mesma chave de criptografia.
4. Salva os dados originais em um novo arquivo com o mesmo nome do arquivo original (`teste.txt`).

## Como Usar

### Criptografar um Arquivo

1. Coloque o arquivo que deseja criptografar no mesmo diretório do script.
2. Certifique-se de que o arquivo tenha o nome `teste.txt` ou ajuste o código para o nome desejado.
3. Execute o script de criptografia:
   ```bash
   python encrypt.py
   ```
4. O arquivo original será removido e um novo arquivo criptografado será gerado com a extensão `.ransomwaretroll`.

### Descriptografar um Arquivo

1. Certifique-se de que o arquivo criptografado (`teste.txt.ransomwaretroll`) esteja no mesmo diretório do script.
2. Execute o script de descriptografia:
   ```bash
   python decrypt.py
   ```
3. O arquivo criptografado será removido e o arquivo original será recriado com o nome `teste.txt`.

## Avisos

- **Uso Responsável:** Este projeto é apenas para aprendizado. Não utilize para propósitos ilegais ou antiéticos.
- **Chave de Criptografia:** A chave usada nos scripts (`1234567890123456`) é apenas para demonstração. Nunca use chaves hardcoded em aplicações reais.

## Licença

Este projeto está licenciado sob a licença MIT. Consulte o arquivo LICENSE para mais informações.

## Autor

[[Isaac Aires](https://github.com/Isaac-code-maker)]

---

