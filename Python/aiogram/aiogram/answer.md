***answrer***
```python
await message.reply_photo()

await message.reply_photo(message.photo[0].file_id)

message.answer_photo() #отправить фото 

message.answer_audio(...) #аудио файл 
 
message.answer_video(...)#видео 

message.answer_sticker(...)#стикеры 

message.answer_document()#документы 

message.answer_voice()#голосовые сообщения 

message.answer_sticker()#стикеры 

message.answer_poll()#опроса и тд

message.send_copy(chat_id=message.chat.id) #отпрввить копию(не работает с несколькими типами)

```