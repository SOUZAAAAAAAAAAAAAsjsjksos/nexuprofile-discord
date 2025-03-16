# NexussAPI

Acesse seus dados do Discord de forma fácil e rápida.  

**Servidor do Discord:** [Clique aqui](https://discord.gg/QaHyQz34Gq)  

---

## Endpoints

### Obter presença de um usuário  

**Método:** `GET`  
**URL:** `https://nexussapi-production.up.railway.app/user/:userid`  

#### Exemplo de resposta  

```json
{
  "data": {
    "profile": {
      "bot": false,
      "id": "1274150219482660897",
      "creation_date": "2024-08-16T23:38:04.891Z",
      "member_since": "16 de agosto de 2024",
      "username": "grwx",
      "pronouns": "ele/dele",
      "bio": "dfideliz",
      "link": "https://discord.com/users/1274150219482660897",
      "avatar": "7499eb14961cf682385521f20d6501f3",
      "avatar_image": "https://cdn.discordapp.com/avatars/1274150219482660897/7499eb14961cf682385521f20d6501f3.png",
      "badges": [
        {
          "id": "premium",
          "description": "Assinante desde 16 de novembro de 2024",
          "icon": "2ba85e8026a8614b640c2837bcdfe21b",
          "icon_image": "https://cdn.discordapp.com/badge-icons/2ba85e8026a8614b640c2837bcdfe21b.png",
          "link": "https://discord.com/settings/premium"
        }
      ],
      "connected_accounts": [
        {
          "type": "spotify",
          "name": "audibert",
          "link": "https://open.spotify.com/user/31w2axshoydaipmkuz6xvu337egq"
        }
      ]
    },
    "status": "idle",
    "spotify": {
      "type": "Ouvindo Spotify",
      "song": "SPINNIN (Segway Remix)",
      "artist": "ONEFOUR, Nemzzz, Segway",
      "album": "SPINNIN (Segway Remix)",
      "album_image": "https://i.scdn.co/image/ab67616d0000b273c16a46456c512bf475a211f7",
      "link": "https://open.spotify.com/track/5H7JrQsT47tMwNFiPLSnEi",
      "timestamps": {
        "progress": "2:42",
        "duration": "2:42"
      }
    },
    "activity": [
      {
        "type": "Jogando",
        "name": "Visual Studio Code",
        "state": "Workspace: Nexuss",
        "details": "Editando README.md",
        "largeText": "Editando um arquivo Markdown",
        "largeImage": "https://cdn.discordapp.com/app-assets/383226320970055681/565945077491433494.png",
        "smallText": "Visual Studio Code",
        "smallImage": "https://cdn.discordapp.com/app-assets/383226320970055681/565945770067623946.png",
        "timestamps": {
          "time_lapsed": "35:44"
        }
      }
    ]
  },
  "success": true
}
```

---

### Obter informações de um servidor  

**Método:** `GET`  
**URL:** `https://nexussapi-production.up.railway.app/guild/:guildid`  

#### Exemplo de resposta  

```json
{
  "data": {
    "id": "1313726337994723441",
    "owner_id": "303699181900660737",
    "creation_date": "2024-12-04T04:39:26.833Z",
    "on_since": "04 de dezembro de 2024",
    "name": "/nerdolas",
    "icon": "https://cdn.discordapp.com/icons/1313726337994723441/9dfb41c9a7f263feb85da4d1186a9c80.png",
    "banner": "https://cdn.discordapp.com/banners/1313726337994723441/0a9a2bbd38d0c785e3116bf96ffa60ae.png",
    "boost_count": 24,
    "boost_level": 3,
    "community": true,
    "member_count": 333,
    "member_online_count": 109,
    "emoji": "https://cdn3.emoji.gg/emojis/3388-community-server-boosted.png",
    "country": "pt-BR"
  },
  "invite": "https://discord.gg/MBpV2NJF",
  "success": true
}
```

---

## Endpoints adicionais  

- **`/profile/:userid`** - Retorna foto de perfil, nome de usuário e nome de exibição *(Em breve)*.  
- **`/activity/:userid`** - Retorna informações de Spotify e atividades.  
- **`/guilds`** - Retorna todos os servidores que o bot faz parte.  

---

## Códigos de erro  

| Código | Descrição |
|--------|------------|
| `404`  | Recurso não encontrado (rota, usuário ou servidor). |
| `500`  | Erro interno no servidor. |

---

## Problemas com imagens de atividades  

Algumas imagens de atividades podem não ser exibidas corretamente devido a limitações da API. Estamos trabalhando para corrigir isso em futuras versões.
