

# HTTP IN DETAIL

Learn about how you request content from a web server using the HTTP Protocol.

HTTP é usado em qualquer momento em que precisamos visualizar um site. Foi desenvolvido por Tim Berners-Lee e sua equipe entre 1989-1991.  

## HTTPS (HyperText Transfer Protocol Secure)

HTTPS é a versão segura do HTTP.  
No HTTPS os dados são criptografados, ou seja, ninguém consegue ver o que você está recebendo ou enviando.  
Em palavras mais técnicas: *getting* e *posting*.  

Quando precisamos acessar um site, nosso navegador envia *requests* para um servidor web, indexados em HTML, imagens, e baixa as respostas.  

---

### O que é URL (Uniform Resource Locator)

Se você utiliza minimamente a internet, deve saber que sempre usa uma URL.  
Basicamente, é uma instrução de como acessar um site e de como ele aparece.  

**Estrutura:**
http://user:psw@host/domain:port/path/string/fragment

- **scheme/http:** protocolo usado (HTTP, HTTPS, FTP – *File Transfer Protocol*)  
- **user:** usuário  
- **host:** domínio  
- **port:** geralmente 80 para HTTP e 443 para HTTPS  
- **path:** nome do arquivo e local (onde você está acessando)  
- **string:** informações extras (dependem do que você está acessando)  
- **fragment:** referência ao local  

---

#### MÉTODOS DE HTTP

- **GET** – usado para pegar informação  
- **POST** – usado para enviar dados e criar novas gravações  
- **PUT** – usado para atualizar informações  
- **DELETE** – usado para deletar informações  

---

## HTTP Status Codes

Quando um servidor HTTP responde, a primeira linha sempre contém um *status code* informando ao cliente o resultado da requisição.  

### 🔢 Faixas de códigos

| Faixa | Significado |
|-------|-------------|
| **100-199 - Information Response** | Informam que a primeira parte da requisição foi aceita e o cliente deve continuar enviando o restante. Pouco comuns hoje. |
| **200-299 - Success** | Requisição bem-sucedida. |
| **300-399 - Redirection** | Redirecionam a requisição para outro recurso. |
| **400-499 - Client Errors** | Erro na requisição do cliente. |
| **500-599 - Server Errors** | Erros no servidor, geralmente graves. |

---

## Common HTTP Status Codes

| Código | Significado |
|--------|-------------|
| **200 - OK** | Requisição concluída com sucesso. |
| **201 - Created** | Um recurso foi criado (ex.: novo usuário ou post). |
| **301 - Moved Permanently** | Redirecionamento permanente. |
| **302 - Found** | Redirecionamento temporário. |
| **400 - Bad Request** | Erro ou parâmetro faltando na requisição. |
| **401 - Not Authorised** | Necessário autenticação (usuário/senha). |
| **403 - Forbidden** | Sem permissão para acessar o recurso. |
| **404 - Page Not Found** | Página ou recurso não existe. |
| **405 - Method Not Allowed** | Método não permitido para o recurso. |
| **500 - Internal Server Error** | Erro inesperado no servidor. |
| **503 - Service Unavailable** | Servidor sobrecarregado ou em manutenção. |

👉 Para aprender de forma visual, confira [http.cat](https://http.cat/).

---

## Conceitos básicos

- **Host:** servidores web podem ter múltiplos hosts  
- **User-agent:** esse é você (o navegador)  
- **Content:** quantidade de dados que o site envia  
- **Encoding:** informa ao servidor quais tipos de compressão o navegador suporta  
- **Cookie:** dados enviados para lembrar informações  

---

## Common Response Headers

Esses são os cabeçalhos retornados ao cliente pelo servidor após uma requisição:

- **Set-Cookie:** informações armazenadas e enviadas de volta ao servidor em cada requisição  
- **Cache-Control:** tempo que o conteúdo pode ficar armazenado no cache do navegador  
- **Content-Type:** tipo de dado retornado (HTML, CSS, JS, imagens, PDF, vídeo etc.)  
- **Content-Encoding:** método usado para comprimir os dados e enviá-los de forma eficiente  

---
