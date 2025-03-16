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
