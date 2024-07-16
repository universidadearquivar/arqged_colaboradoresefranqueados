# ▫️ Fevereiro | 2024



<details>

<summary>07/02: ArqFlow - Resiliência para as Notificações</summary>

O envio das notificações do workflow foi alterado para garantir a entrega e eficiência no menor tempo possível.

Houve a **contratação** do serviço de e-mail **SendGrid** que possui foco na entrega das mensagens, além de facilitar a gestão das notificações através de relatórios de envios e falhas. Além deste novo serviço, **continuamos com o SMTP.com e Microsoft 365**, já utilizados anteriormente.

Com **três** possibilidades de **redundância**, criamos um processo para **aumentar a resiliência** das notificações. Caso aconteça alguma eventual falha no serviço principal, a aplicação irá, automaticamente, redirecionar o envio das notificações para algum dos outros serviços disponíveis.

<mark style="color:green;">**Serviço Principal:**</mark> SendGrid

<mark style="color:green;">**Serviços Secundários:**</mark> SMTP.com e Microsoft 365

</details>
