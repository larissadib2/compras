# Team Henrique — Beach Tennis

Site/app de página única (`index.html`) para gestão de aulas de beach tennis.

## Como usar

Abra `index.html` em qualquer navegador (não precisa de servidor/backend). Os dados de alunos, agendamentos, cancelamentos e pagamentos ficam salvos no `localStorage` do navegador em que o cadastro/login foi feito.

## Acesso da área do professor

- URL: `index.html#area-professor`
- Login padrão (primeiro acesso): `professor@teamhenrique.com` / `beachtennis123`
- Troque o e-mail e a senha em **Configurações** assim que entrar pela primeira vez.
- Configure também a **chave Pix** em Configurações para poder gerar cobranças Pix para os alunos.

## O que o painel do professor tem

- **Alunos**: lista com nome, WhatsApp, e-mail, nível, plano e horários fixos.
- **Agenda**: grade semanal (segunda a quinta, 15h–20h) e cancelamentos recentes.
- **Financeiro**: registrar pagamento automaticamente (valor do plano) ou gerar cobrança via Pix (código copia-e-cola padrão Banco Central), com status pago/aguardando.
- **Mensagens**: escreva uma mensagem e envie para todos os alunos. Cada aluno recebe uma aba do WhatsApp com o texto pronto — o próprio WhatsApp exige confirmar o envio manualmente em cada conversa (não existe forma de disparo 100% automático sem contratar a API oficial do WhatsApp Business).

## Importante — limitações

- **Sem backend real**: os dados ficam apenas no navegador/dispositivo usado. Para ter os mesmos dados em vários dispositivos (ex.: professor acessando do celular e do computador), será necessário migrar para um banco de dados na nuvem no futuro.
- **Segurança do login do professor**: como é um site 100% estático, a validação de senha acontece no próprio navegador. É suficiente para uso interno/baixo risco, mas não substitui autenticação de servidor caso os dados se tornem sensíveis.
- **Número de WhatsApp do professor**: (31) 98214-3914, usado no botão "aula grátis" e nos links de mensagem.
