прикольные фишки
@dp.message(Command(commands='start', prefix='|')) - можно поставить вместо / , все что угодно 

@dp.message(Command(commands=["start"]))
команды

@dp.my_chat_member(ChatMemberUpdatedFilter(member_status_changed=KICKED))
async def process_user_blocked_bot(event: ChatMemberUpdated):
    print(f'Пользователь {event.from_user.id} заблокировал бота')
проверка на заблокировали ли бота 

@dp.message(F.content_type.in_({'voice', 'video', 'text'}))
1 вариант несколько

@dp.message(F.content_type.in_({ContentType.VOICE,ContentType.VIDEO,ContentType.TEXT}))
2 вариант несколько 

handlers
@dp.message(CommandStart())
команда /start

@dp.message()
все

@dp.message(F.content_type == ContentType.PHOTO)
фото

@dp.message(F.content_type == ContentType.TEXT)
текст 

@dp.message(F.content_type == ContentType.DOCUMENT)
документ

@dp.message(F.content_type == ContentType.STICKER)
стикер 

@dp.message(F.content_type == ContentType.VIDEO)
видео 

@dp.message(F.content_type == ContentType.VIDEO_NOTE)
видео сообщения(кружочки)

@dp.message(F.content_type == ContentType.VOICE)
голосовые сообщения 

@dp.message(F.content_type == ContentType.LOCATION)
местоположение 

@dp.message(F.content_type == ContentType.CONTACT)
контакт 

@dp.message(F.content_type == ContentType."...")
- ANIMATION - анимация (GIF)
- VENUE - место проведения
- POLL - опрос
- DICE - игральная кость
- NEW_CHAT_MEMBERS - новые участники чата
- LEFT_CHAT_MEMBER - участник покинул чат
- NEW_CHAT_TITLE - новое название чата
- NEW_CHAT_PHOTO - новая фотография чата
- DELETE_CHAT_PHOTO - удаление фотографии чата
- GROUP_CHAT_CREATED - создание группового чата
- SUPERGROUP_CHAT_CREATED - создание супергруппового чата
- CHANNEL_CHAT_CREATED - создание канала
- MIGRATE_TO_CHAT_ID - миграция в другой чат
- MIGRATE_FROM_CHAT_ID - миграция из другого чата
- PINNED_MESSAGE - закрепленное сообщение
- INVOICE - счет
- SUCCESSFUL_PAYMENT - успешный платеж
- CONNECTED_WEBSITE - подключенный веб-сайт
- PASSPORT_DATA - данные паспорта
- PROXIMITY_ALERT_TRIGGERED - сработало предупреждение о приближении
- VOICE_CHAT_SCHEDULED - запланирована голосовая беседа
- VOICE_CHAT_STARTED - началась голосовая беседа
- VOICE_CHAT_ENDED - завершилась голосовая беседа
- VOICE_CHAT_PARTICIPANTS_INVITED - приглашены участники голосовой беседы


documentation aiogram : https://docs.aiogram.dev/en/dev-3.x/api/enums/content_type.html#module-aiogram.enums.content_type - типы 
documentation aiogram : https://docs.aiogram.dev/en/dev-3.x/dispatcher/filters/chat_member_updated.html - статусы 
