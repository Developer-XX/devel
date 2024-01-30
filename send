import telebot
import requests

Token = "6574402727:AAG60wAjsHiV1hRP_K44sO7_mwjkrXOs100"

url = 'https://api.hydrax.net/5ae38dfa48796a4f2269a39eb790e882/copy/'

bot = telebot.TeleBot(Token)


@bot.message_handler(['start'])
def start(message):
    bot.reply_to(message,"Nobi Dubber hai")


@bot.message_handler()
def start(message):
    t = url + message.text
    r = requests.get(t)
    p = r.text + "Succesfull"
    bot.reply_to(message,p)

bot.polling()  
