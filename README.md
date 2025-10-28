name: Boner Alarm
on: [push]

jobs:
  discord:
    runs-on: ubuntu-latest
    steps:
      - name: Send message to Discord
        uses: Ilshidur/action-discord@v3
        with:
          webhook: ${{ secrets.DISCORD_WEBHOOK }}
          message: "Boner Alarm"
