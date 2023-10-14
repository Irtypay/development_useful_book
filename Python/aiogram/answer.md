await message.reply_photo()
message.answer_photo()
await message.reply_photo(message.photo[0].file_id)
отправить фото 
message.answer_audio(...)
аудио файл 
message.answer_video(...)
видео 
message.answer_sticker(...)
стикеры 
message.answer_document()
документы 
message.answer_voice()
голосовые сообщения 
message.answer_sticker()
стикеры 
message.answer_poll()
опроса и тд 
