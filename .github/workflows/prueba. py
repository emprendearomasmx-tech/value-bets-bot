import os, requests

token = os.getenv("TELEGRAM_BOT_TOKEN")
chat_id = os.getenv("TELEGRAM_CHAT_ID")

if token and chat_id:
    url = f"https://api.telegram.org/bot{token}/sendMessage"
    payload = {"chat_id": chat_id, "text": "🚀 ¡Prueba exitosa! El sistema de valor está conectado y listo para trabajar."}
    respuesta = requests.post(url, json=payload)
    print("Mensaje enviado:", respuesta.json())
else:
    print("Error: Faltan los secretos en GitHub.")
