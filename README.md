# 学习rasa使用的repos

##  使用UI测试  
1. 在credentials.yml文件中添加以下内容 :
socketio:
  user_message_evt: user_uttered
  bot_message_evt: bot_uttered
  session_persistence: true
  
2. 启动后端bot
rasa run -m models --enable-api --cors "*" --debug

3. 浏览器打开web_ui.html即可测试