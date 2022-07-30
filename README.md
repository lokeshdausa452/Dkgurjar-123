# Dkgurjar-123
𝐋𝐎𝐕𝐄  𝐘𝐎𝐔 𝐀𝐑𝐌𝐘
# Deploy

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

{
    "name": "DKMUSIC",
    "description": "Music allow you to stream music trought the telegram voice chat feature.",
    "keywords": ["Dkmusic", "Dkmusic5bot", "music", "voice chat", "telegram", "Yukki", "Yukki Music", "Private Music"],
    "repository": "https://github.com/DK143GURJAR/Dkgurjar@123",
  "stack": "container",
    "env": {
        "SESSION_NAME": {
            "description": "fill with the pyrogram session string from account",
            "required": true
        },
        "ASSISTANT_NAME": {
            "description": "fill with your telegram id as the owner of the bot",
            "required": true,
            "value": "Dkgurjar143"
        },
        "BOT_USERNAME": {
            "description": "fill with telegram id of account",
            "required": true,
            "value": "Dkmusic5bot"
        },
        "API_ID": {
            "description": "your Api ID from my.telegram.org/apps",
            "required": true,
            "value": "12138418"
        },
        "API_HASH": {
            "description": "your Api Hash from my.telegram.org/apps",
            "required": true,
            "value": "f7c60f0f506a54d27df6bc32a1bbe785"
        },
        "GROUP_SUPPORT": {
            "description": "Ur Support Group Username",
            "required": true,
            "value": "Education_quiz_hub"
        },
        "UPDATES_CHANNEL": {
            "description": "Your Updates Channel",
            "required": true,
            "value": "Dk_music_shayari"
        },
        "SUDO_USERS": {
            "description": "fill with the user id who can access all function in your bot (separate with space).",
            "required": true,
            "value": "1781352356"
        },
        "DURATION_LIMIT": {
            "description": "filled, don't change this !",
            "required": true,
            "value": "540000"
        },
        "BOT_TOKEN": {
            "description": "fill with your bot token get from @BotFather on telegram",
            "required": true,
            "value": ""
        }

    },
  "buildpacks": [
          {
              "url": "heroku/python"
          },
          {
              "url": "heroku/nodejs"
          },
          {
              "url": "https://github.com/jonathanong/heroku-buildpack-ffmpeg-latest.git"
          }
      ],
      "formation": {
          "worker": {
              "quantity": 1,
              "size": "free"
          }
      },
      "stack": "container"
  }
