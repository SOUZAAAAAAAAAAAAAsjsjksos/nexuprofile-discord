⚡ Acesse todos os seus dados do Discord de forma fácil com a Nexuss API!

A Nexuss API é um serviço que permite acessar informações detalhadas sobre presença de usuários e servidores do Discord por meio de uma API RESTful. Com apenas um clique, você pode exibir perfis do Discord, badges, status, atividades e dados de guilds no seu site ou aplicativo.

🚀 Como começar

1. Entre no nosso servidor do Discord


2. Seus dados de presença estarão disponíveis em https://nexussapi-production.up.railway.app/user/:userid



E pronto! É tudo o que você precisa fazer!

📜 Documentação da API

🔍 Obter presença de um usuário

GET https://nexussapi-production.up.railway.app/user/:userid

Exemplo de resposta:

{
  "data": {
    "profile": {
      "bot": "false",
      "id": "1274150219482660897",
      "creation_date": "2024-08-16T23:38:04.891Z",
      "member_since": "16 de agosto de 2024",
      "username": "grwx",
      "pronouns": "ele/dele",
      "bio": "Desenvolvedor e entusiasta de tecnologia",
      "link": "https://discord.com/users/1274150219482660897",
      "avatar_image": "https://cdn.discordapp.com/avatars/1274150219482660897/7499eb14961cf682385521f20d6501f3.png",
      "badges": [
        {
          "id": "premium",
          "description": "Assinante desde 16 de novembro de 2024",
          "icon_image": "https://cdn.discordapp.com/badge-icons/2ba85e8026a8614b640c2837bcdfe21b.png",
          "link": "https://discord.com/settings/premium"
        }
      ],
      "connected_accounts": [
        {
          "type": "spotify",
          "name": "grwx",
          "link": "https://open.spotify.com/user/31w2axshoydaipmkuz6xvu337egq"
        }
      ]
    },
    "status": "idle",
    "activity": [
      {
        "type": "Jogando",
        "name": "Visual Studio Code",
        "state": "Editando código",
        "details": "Trabalhando no projeto Nexuss API",
        "largeImage": "https://cdn.discordapp.com/app-assets/383226320970055681/565945077491433494.png",
        "timestamps": {
          "time_lapsed": "35:44"
        }
      }
    ]
  },
  "success": true
}

🔍 Obter informações de um servidor

GET https://nexussapi-production.up.railway.app/guild/:guildid

Exemplo de resposta:

{
  "data": {
    "id": "1313726337994723441",
    "owner_id": "303699181900660737",
    "creation_date": "2024-12-04T04:39:26.833Z",
    "name": "/nerdolas",
    "icon": "https://cdn.discordapp.com/icons/1313726337994723441/9dfb41c9a7f263feb85da4d1186a9c80.png",
    "boost_count": 24,
    "boost_level": 3,
    "community": true,
    "member_count": 333,
    "member_online_count": 109
  },
  "invite": "https://discord.gg/MBpV2NJF",
  "success": true
}

🔗 Endpoints rápidos

🔹 Perfil (em breve) – Retorna avatar, nome de usuário e exibição
📌 https://nexussapi-production.up.railway.app/profile/:userid

🔹 Atividades – Retorna informações do Spotify e jogos ativos
🎮 https://nexussapi-production.up.railway.app/activity/:userid

🔹 Servidores – Lista todas as guilds que o bot participa
🏠 https://nexussapi-production.up.railway.app/guilds

❌ Códigos de erro

ℹ️ Observações

🎭 Algumas imagens de atividades podem não ser exibidas corretamente devido a limitações do Discord. Para corrigir, adicionamos ícones personalizados para certos aplicativos como VALORANT, Roblox e Fortnite. Se precisar adicionar mais, contribua com um pull request!

🤝 Contribuindo

Quer ajudar a melhorar a Nexuss API? Sinta-se à vontade para abrir issues e enviar pull requests!

💡 Entre no nosso Discord e faça parte dessa comunidade!

