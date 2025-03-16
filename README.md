# NexussAPI

Acesse seus dados do Discord de forma fácil e rápida.  

**Servidor do Discord:** [Clique aqui](https://discord.gg/QaHyQz34Gq) 
**Site:** [Clique aqui](https://nexusync.vercel.app/)

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
      "bot": "false",
      "id": "1141824276119429140",
      "creation_date": "2023-08-17T20:02:01.496Z",
      "member_since": "Aug 17, 2023",
      "username": "determinaram",
      "display_name": "souzaz",
      "pronouns": "keef",
      "bio": "ainda que eu ande pelo vale da sombra da morte, não temerei mal algum",
      "link": "https://discord.com/users/1141824276119429140",
      "avatar": "c652137cb2feb876fc73704207339a74",
      "avatar_image": "https://cdn.discordapp.com/avatars/1141824276119429140/c652137cb2feb876fc73704207339a74.png",
      "badges": [
        {
          "id": "premium",
          "description": "Subscriber since Nov 16, 2024",
          "icon": "2ba85e8026a8614b640c2837bcdfe21b",
          "icon_image": "https://cdn.discordapp.com/badge-icons/2ba85e8026a8614b640c2837bcdfe21b.png",
          "link": "https://discord.com/settings/premium"
        },
        {
          "id": "guild_booster_lvl2",
          "description": "Server boosting since Nov 18, 2024",
          "icon": "0e4080d1d333bc7ad29ef6528b6f2fb7",
          "icon_image": "https://cdn.discordapp.com/badge-icons/0e4080d1d333bc7ad29ef6528b6f2fb7.png",
          "link": "https://discord.com/settings/premium"
        },
        {
          "id": "hypesquad_house_1",
          "description": "Bravery do HypeSquad",
          "icon": "8a88d63823d8a71cd5e390baa45efa02",
          "icon_image": "https://cdn.discordapp.com/badge-icons/8a88d63823d8a71cd5e390baa45efa02.png",
          "link": "https://discord.com/settings/hypesquad-online"
        },
        {
          "id": "active_developer",
          "description": "Desenvolvedor(a) ativo(a)",
          "icon": "6bdc42827a38498929a4920da12695d9",
          "icon_image": "https://cdn.discordapp.com/badge-icons/6bdc42827a38498929a4920da12695d9.png",
          "link": "https://support-dev.discord.com/hc/en-us/articles/10113997751447?ref=badge"
        },
        {
          "id": "quest_completed",
          "description": "Completed a Quest",
          "icon": "7d9ae358c8c5e118768335dbe68b4fb8",
          "icon_image": "https://cdn.discordapp.com/badge-icons/7d9ae358c8c5e118768335dbe68b4fb8.png",
          "link": "https://discord.com/discovery/quests"
        }
      ],
      "connected_accounts": [
        {
          "type": "spotify",
          "name": "szz",
          "link": "https://open.spotify.com/user/31ltog4anx25ppv3ns3gzz3ez3ua"
        }
      ]
    },
    "status": "idle",
    "spotify": {
      "type": "Listening to Spotify",
      "name": "Spotify",
      "song": "Pobre Juan",
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
        "type": "Playing",
        "name": "Visual Studio Code",
        "state": "Workspace: API",
        "details": "Editing index.js",
        "largeText": "Editing a MARKDOWN file",
        "largeImage": "https://cdn.discordapp.com/app-assets/383226320970055681/565945077491433494.png",
        "smallText": "Visual Studio Code",
        "smallImage": "https://cdn.discordapp.com/app-assets/383226320970055681/565945770067623946.png",
        "timestamps": {
          "time_lapsed": "47:13"
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
    "id": "1349796292825710594",
    "owner_id": "1141824276119429140",
    "creation_date": "2025-03-13T17:28:34.212Z",
    "on_since": "Mar 13, 2025",
    "name": "Nexuss",
    "icon": "https://cdn.discordapp.com/icons/1349796292825710594/579404ef0130f7207095cc1a8e32638b.png",
    "boost_count": 0,
    "boost_level": 0,
    "community": false,
    "discoverable": false,
    "verified": false,
    "member_count": 5,
    "member_online_count": 4,
    "country": "en-US"
  },
  "invite": "https://discord.gg/2EsCNWa4",
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
