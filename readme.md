# Aplicativo de Envio de E-mail em PHP

Este é um aplicativo simples de envio de e-mail desenvolvido como parte do módulo de PHP Orientado a Objeto no curso de Desenvolvimento Web. O aplicativo permite que os usuários enviem e-mails fornecendo informações como destinatário, assunto e mensagem.

## Funcionalidades

- Envio de e-mails para destinatários especificados.
- Tratamento de erros usando `try`, `catch`, `throw` e `finally`.
- Integração com servidor SMTP para o envio seguro de e-mails.

## Requisitos

- PHP instalado no servidor.
- Acesso a um servidor SMTP para envio de e-mails (exemplo: Gmail, Outlook).
- As bibliotecas PHPMailer para lidar com o envio de e-mails.

## Como Usar

1. Clone o repositório para o seu servidor web: https://github.com/edukleber100/app_send_mail.git

2. Instale as bibliotecas PHPMailer necessárias. Você pode fazer isso com o Composer ou baixando manualmente as bibliotecas a partir do [GitHub do PHPMailer](https://github.com/PHPMailer/PHPMailer).

3. Configure as credenciais do servidor SMTP no arquivo `processa_envio.php`. Edite as seguintes linhas:

```php
$mail->Host = 'smtp.servidor.com';
$mail->SMTPAuth = true;
$mail->Username = 'seu-email@gmail.com';
$mail->Password = 'sua-senha';
$mail->SMTPSecure = 'tls';
$mail->Port = 587;
$mail->setFrom('seu-email@gmail.com', 'Seu Nome');
