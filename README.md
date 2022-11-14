
# realtime-chat-app

Esse projeto consome o framework [GoFiber](https://github.com/gofiber/fiber)
para enviar requisições de chat em tempo real utilizando a linguagem Go.

Considere olhar as screenshots publicadas abaixo para verificar o funcionamento da aplicação.


## Instalação

```bash
  npm install https://github.com/teixtarcio/realtime-chat-app.git
  cd realtime-chat-app
  go install
  go run main.go
```
    
## Uso/Exemplos

Para monitorar e receber as requisições, utilizei o [Pusher](https://pusher.com/).

É necessário para que você faça uso da aplicação, alterar os dados em `pusherClient := pusher.Client` no código, acrescentando as suas credenciais.

```go
	pusherClient := pusher.Client{
		AppID:   "xxxxx",
		Key:     "xxxxx",
		Secret:  "xxxxx",
		Cluster: "xxxxx",
		Secure:  xxxxx,
	}
```


## Screenshots

Servidor em funcionamento:

![App Screenshot](https://i.imgur.com/rz4vjd5.png)

Requisição de mensagem enviada (via Postman):

![App Screenshot](https://i.imgur.com/dGx2GU3.png)

Confirmação do recebimento da requisição:

![App Screenshot](https://i.imgur.com/usHiVfm.png)
