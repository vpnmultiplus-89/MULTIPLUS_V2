#!/bin/bash
set -e

cd "$(dirname "$0")"

# cari launcher yang ada di folder menu
if [ -f "menu/bot.sh" ]; then
  chmod +x menu/bot.sh
  exec bash menu/bot.sh
elif [ -f "menu/panelbot.sh" ]; then
  chmod +x menu/panelbot.sh
  exec bash menu/panelbot.sh
elif [ -f "menu/menu" ]; then
  chmod +x menu/menu
  exec bash menu/menu
else
  echo "Launcher tidak ditemukan di folder menu."
  echo "Isi folder menu:"
  ls -la menu || true
  exit 1
fi
