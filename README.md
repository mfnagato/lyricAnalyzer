# Lyrics Analyzer

Este projeto analisa letras de músicas de um álbum específico, buscando informações no Wikipedia e Genius, e gera um relatório PDF com análises detalhadas.

## Estrutura do Projeto

- `lyricAn.py`: Programa principal que coordena a análise de letras
- `crypto_utils.py`: Módulo para gerenciamento seguro de chaves de API
- `requirements.txt`: Dependências do projeto

## Configuração da API Key

Para usar o programa, você precisa de uma chave de API do ChatGPT. Siga estes passos:
1. Obtenha uma chave de API do ChatGPT.
2. Execute o Python e use o módulo crypto_utils para criptografar sua chave:

```python
from crypto_utils import encrypt_api_key
encrypt_api_key('sua-chave-api-aqui')
```

Isso criará dois arquivos:
- `secret.key`: Chave de criptografia
- `api.key`: Sua chave de API criptografada

## Uso

Após configurar a chave de API, você pode executar o programa principal:

```bash
python lyricAn.py
```

O programa irá:
1. Descriptografar automaticamente a chave de API
2. Buscar informações do álbum no Wikipedia
3. Buscar letras das músicas no Genius
4. Gerar análises das letras
5. Criar um relatório PDF na pasta 'analises'

## Segurança

- A chave de API é armazenada de forma criptografada
- A chave de criptografia é gerada automaticamente na primeira execução
- Nunca compartilhe os arquivos `secret.key` e `api.key`#   l y r i c A n a l y z e r  
 