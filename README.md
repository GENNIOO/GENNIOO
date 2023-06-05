import telebot

bot = telebot.TeleBot("Here is the token for bot consulcpfbot @messiCpfbot:

6031056676:AAEADU_STSxHz-77x_qAapGzyw8USG-oZDw")


@bot.message_handler(commands=['start', 'hello'])
def send_welcome(message):
    bot.reply_to(message, "Howdy, how are you doing?")

bot.infinity_polling()

