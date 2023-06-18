# Comparing `tmp/yeref-0.1.98.tar.gz` & `tmp/yeref-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.98.tar", last modified: Thu Jun 15 11:45:40 2023, max compression
+gzip compressed data, was "yeref-0.1.99.tar", last modified: Sun Jun 18 12:52:36 2023, max compression
```

## Comparing `yeref-0.1.98.tar` & `yeref-0.1.99.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-15 11:45:40.412498 yeref-0.1.98/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-15 11:45:40.412825 yeref-0.1.98/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-15 11:45:40.414042 yeref-0.1.98/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-15 11:44:55.000000 yeref-0.1.98/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-15 11:45:40.405449 yeref-0.1.98/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.98/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   556618 2023-06-15 11:44:29.000000 yeref-0.1.98/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   210936 2023-06-14 09:33:51.000000 yeref-0.1.98/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-15 11:45:40.411787 yeref-0.1.98/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-15 11:45:40.000000 yeref-0.1.98/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-15 11:45:40.000000 yeref-0.1.98/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-15 11:45:40.000000 yeref-0.1.98/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-15 11:45:40.000000 yeref-0.1.98/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-18 12:52:36.678305 yeref-0.1.99/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-18 12:52:36.678454 yeref-0.1.99/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-18 12:52:36.679039 yeref-0.1.99/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-18 12:52:23.000000 yeref-0.1.99/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-18 12:52:36.669882 yeref-0.1.99/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.99/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   557031 2023-06-18 12:52:19.000000 yeref-0.1.99/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   211025 2023-06-15 14:36:34.000000 yeref-0.1.99/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-18 12:52:36.677867 yeref-0.1.99/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-18 12:52:36.000000 yeref-0.1.99/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-18 12:52:36.000000 yeref-0.1.99/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-18 12:52:36.000000 yeref-0.1.99/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-18 12:52:36.000000 yeref-0.1.99/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.98/setup.py` & `yeref-0.1.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.98',
+      version='0.1.99',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -43,12 +43,12 @@
 
 # twine upload dist/*
 # freey.sitner.ya
 # cejwez-nosgin-vaVfe7
 
 # python3 -m pip install --upgrade yeref
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.97-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.98-py3-none-any.whl
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.98/yeref/l_.py` & `yeref-0.1.99/yeref/l_.py`

 * *Files 1% similar despite different names*

```diff
@@ -2351,23 +2351,23 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_chn_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> администрирования <b>Telegram</b>-каналов:\n\n▪️<b>защита</b> канала от вступления шпионов\n▪️<b>организация</b> бана и антифлуда\n▪️<b>сбор</b> подписчиков\n▪️<b>счетчик</b> нажатий\n▪️<b>реакции</b> и просмотры\n\n❗️Регулярно-обновляемый /content",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> администрирования <b>Telegram</b>-каналов:\n\n▪️<b>защита</b> канала от вступления шпионов\n▪️<b>организация</b> бана и антифлуда\n▪️<b>сбор</b> подписчиков\n▪️<b>кнопочный</b> счетчик\n▪️<b>реакции</b> и просмотры\n▪️<b>авто-декор</b> поста\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to the <b>Telegram</b> channel администрирования <i>landing bot</i> :\n\n▪️ <b>protection</b> of the channel from spyware entry\n▪️display <b>of statistics</b> and engagement (%)\n▪️restriction of rights before <b>subscribing</b> to the channel\n▪️ <b>organization</b> of a ban and anti-flood\n\n❗️you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> администрирования de canales <b>de Telegram</b> :\n\ <b>n▪️protección</b> del canal contra la entrada de software espía\n▪️visualización <b>de estadísticas</b> e interacción (%)\n▪️restricción de derechos antes de <b>suscribirse</b> al canal\n▪️ <b>organización</b> de una prohibición y anti-inundación\n\n❗️también puedes encargar el desarrollo de un chatbot en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue dans le <i>landing bot</i> администрирования de la chaîne <b>Telegram</b> :\n\n▪️ <b>protection</b> de la chaîne contre l&#x27;entrée de logiciels espions\n▪️affichage <b>des statistiques</b> et de l&#x27;engagement (%)\n▪️restriction des droits avant de <b>s&#x27;abonner</b> à la chaîne\n<b>▪️organisation</b> d'une interdiction et anti-flood\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio de Ferey",
     'zh': "🌱 {0}，欢迎使用<b>Telegram</b>频道администрирования<i>登陆机器人</i>：\n\n▪️<b>保护</b>频道免受间谍软件入侵\n▪️ 显示<b>统计信息</b>和参与度 (%)\n▪️<b>订阅</b>频道前的权利限制\n▪️<b>组织</b>禁令和反洪水\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت</i> администрирования قناة <b>Telegram</b> :\n\n▪️ <b>حماية</b> القناة من إدخال برامج التجسس\n▪️ <b>عرض الإحصائيات</b> والمشاركة (٪)\n▪️ تقييد الحقوق قبل <b>الاشتراك</b> في القناة\n▪️ <b>تنظيم</b> حظر ومكافحة الفيضانات\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
 l_subscribe_channel = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️до 50 <b>реакций</b> и просмотров\n▪️<b>выгрузка</b> базы пользователей\n\n👩🏽‍💻 /balance",
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️до 75 <b>реакций</b>/просмотров на пост\n▪️<b>/parse</b> базы пользователей\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
     'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 
@@ -3159,15 +3159,15 @@
     'ar': "🔔 في إعدادات [Administrators] ، قم بتمكين خيار @ {0} -bot:\n[✅ تثبيت الرسائل]\n\n🕚 انتظر دقيقة واحدة",
 }
 # endregion
 
 
 # region creact_
 l_creact_text = {
-    'ru': "👍🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> креативные авто-реакции на последний пост канала\n\n👩🏽‍💻 Используй команду /react {0}, чтобы задать количество авто-реакций на пост(<b>текущее</b> количество: <u>{0}</u>)",
+    'ru': "👍🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> креативные авто-реакции на последний пост канала\n\n👩🏽‍💻 Используй команду <code>/react {0}</code>, чтобы задать количество авто-реакций на пост (без подписки: <u>{1}</u>)\n\n👍🏽 <b>Tекущее</b> количество: <u>{0}</u>",
     'en': "👍🏽 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> creative auto-reactions on the last post of the channel\n\n👩🏽‍💻 Use the command /react {0} to set the number of auto-reactions per post ( <b>current</b> number: <u>{0 }</u> )",
     'es': "👍🏽 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> las reacciones automáticas creativas en la última publicación del canal\n\n👩🏽‍💻 Usa el comando /react {0} para configurar el número de reacciones automáticas por publicación ( número <b>actual</b> : <u>{0 }</u> )",
     'fr': "👍🏽 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> les auto-réactions créatives sur la dernière publication de la chaîne\n\n👩🏽‍💻 Utilisez la commande /réagir {0} pour définir le nombre d&#x27;auto-réactions par publication ( numéro <b>actuel</b> : <u>{0 }</u> )",
     'zh': "👍🏽<b>点击</b>✅/☑️<b>打开/关闭</b>频道最后一个帖子的创意自动反应\n\n👩🏽‍💻 使用命令 /react {0} 设置每个帖子的自动反应数量 (<b>当前</b>号码： <u>{0 }</u> )",
     'ar': "👍🏽 <b>انقر</b> على ✅ / ☑️ <b>لتشغيل / إيقاف</b> ردود الفعل التلقائية الإبداعية في آخر مشاركة للقناة\n\n👩🏽‍💻 استخدم الأمر / رد الفعل {0} لتعيين عدد التفاعلات التلقائية لكل مشاركة ( الرقم <b>الحالي</b> : <u>{0}</u> )",
 }
 l_creact_call = {
@@ -3175,23 +3175,23 @@
     'en': "👍🏽 In the [Administrators] settings for @{0} on:\n[✅ Add member]\n\n🕚Wait 1min",
     'es': "👍🏽 En la configuración de [Administradores] para @{0} en:\n[✅ Agregar miembro]\n\n🕚Espera 1 minuto",
     'fr': "👍🏽 Dans les paramètres [Administrateurs] pour @{0} sur :\n[✅ Ajouter un membre]\n\n🕚Attendez 1min",
     'zh': "👍🏽在@{0}的[管理员]设置中：\n[✅添加成员]\n\n🕚等待1分钟",
     'ar': "👍🏽 في إعدادات [Administrators] لـ @ {0} على:\n[✅ إضافة عضو]\n\n🕚 انتظر دقيقة واحدة",
 }
 l_creact_correct = {
-    'ru': "👍🏽 <b>Введи</b> корректное <b>число</b> креативных авто-реакций на последний пост канала\n\n👩🏽‍💻 Используй команду /react {0}, чтобы задать количество авто-реакций (<b>текущее</b> количество: <u>{0}</u>)",
+    'ru': "👍🏽 <b>Введи</b> корректное <b>число</b> креативных авто-реакций на последний пост канала\n\n👩🏽‍💻 Используй команду <code>/react {0}</code>, чтобы задать количество авто-реакций (без подписки: <u>{1}</u>)",
     'en': "👍🏽 <b>Enter</b> the correct <b>number</b> of creative auto-reactions to the last post of the channel\n\n👩🏽‍💻 Use the /react {0} command to set the number of auto-reactions ( <b>current</b> number: <u>{0}</u> )",
     'es': "👍🏽 <b>Ingresa</b> el <b>número</b> correcto de reacciones automáticas creativas a la última publicación del canal\n\n👩🏽‍💻 Usa el comando /react {0} para establecer el número de reacciones automáticas (número <b>actual</b> : <u>{0}</u> )",
     'fr': "👍🏽 <b>Saisissez</b> le <b>nombre</b> correct de réactions automatiques créatives au dernier message de la chaîne\n\n👩🏽‍💻 Utilisez la commande /react {0} pour définir le nombre de réactions automatiques (nombre <b>actuel</b> : <u>{0}</u> )",
     'zh': "👍🏽<b>输入</b>频道最后一个帖子的正确创意自动反应<b>数量</b>\n\n👩🏽‍💻 使用/react {0}命令设置自动反应数量（<b>当前</b>数量： <u>{0}</u> ）",
     'ar': "👍🏽 <b>أدخل</b> <b>العدد</b> الصحيح من ردود الفعل التلقائية الإبداعية على آخر مشاركة للقناة\n\n👩🏽‍💻 استخدم الأمر /react {0} لتعيين عدد التفاعلات التلقائية (الرقم <b>الحالي</b> : <u>{0}</u> )",
 }
 l_creact_on = {
-    'ru': "👍🏽 <b>Готово!</b> Текущее количество <b>авто-реакций</b> на пост канала установлено в значение <u>{0}</u>",
+    'ru': "👍🏽 <b>Готово!</b> Текущее количество <b>авто-реакций</b> на пост канала установлено в значение <u>{0}</u> (без подписки: <u>{1}</u>)",
     'en': "👍🏽 <b>Done!</b> The current number of <b>auto-reactions</b> per channel post is set to <u>{0}</u>",
     'es': "👍🏽 <b>Listo!</b> El número actual de <b>reacciones automáticas</b> por publicación de canal está establecido en <u>{0}</u>",
     'fr': "👍🏽 <b>C&#x27;est fait !</b> Le nombre actuel de <b>réactions automatiques</b> par publication de chaîne est défini sur <u>{0}</u>",
     'zh': "👍🏽<b>完成！</b>每个频道帖子的当前<b>自动反应</b>数设置为<u>{0}</u>",
     'ar': "👍🏽 <b>انتهى!</b> تم تعيين العدد الحالي <b>للردود التلقائية</b> لكل مشاركة على القناة على <u>{0}</u>",
 }
 l_creact_off = {
@@ -3203,15 +3203,15 @@
     'ar': "👍🏽 / وضع رد الفعل معطل",
 }
 # endregion
 
 
 # region cview_
 l_cview_text = {
-    'ru': "👁️‍🗨️ <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-просмотры поста канала\n\n👩🏽‍💻 Используй команду /view {0}, чтобы задать количество авто-просмотров (<b>текущее</b> количество: <u>{0}</u>)",
+    'ru': "👁️‍🗨️ <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-просмотры поста канала\n\n👩🏽‍💻 Используй команду <code>/view {0}</code>, чтобы задать количество авто-просмотров (без подписки: <u>{1}</u>)\n\n👁️‍🗨️ <b>Tекущее</b> количество: <u>{0}</u>",
     'en': "👁️‍🗨️ <b>Press</b> ✅/☑️ to <b>turn on/off</b> channel post auto views\n\n👩🏽‍💻 Use command /view {0} to set number of auto views ( <b>current</b> number: <u>{0}</u> )",
     'es': "👁️‍🗨️ <b>Presiona</b> ✅/☑️ para <b>activar/desactivar</b> las vistas automáticas de las publicaciones del canal\n\n👩🏽‍💻 Usa el comando /view {0} para establecer el número de vistas automáticas (número <b>actual</b> : <u>{0}</u> )",
     'fr': "👁️‍🗨️ <b>Appuyez sur</b> ✅/☑️ pour <b>activer/désactiver</b> les vues automatiques des publications de la chaîne\n\n👩🏽‍💻 Utilisez la commande /view {0} pour définir le nombre de vues automatiques (nombre <b>actuel</b> : <u>{0}</u> )",
     'zh': "👁️‍🗨️<b>按</b>✅/☑️<b>打开/关闭</b>频道帖子自动观看\n\n👩🏽‍💻 使用命令 /view {0} 设置自动观看次数（<b>当前</b>次数： <u>{0}</u> ）",
     'ar': "👁️‍🗨️ <b>اضغط على</b> ✅ / ☑️ <b>لتشغيل / إيقاف</b> العرض التلقائي لنشر القناة\n\n👩🏽‍💻 استخدم الأمر / العرض {0} لتعيين عدد المشاهدات التلقائية (الرقم <b>الحالي</b> : <u>{0}</u> )",
 }
 l_cview_call = {
@@ -3219,23 +3219,23 @@
     'en': "👁️‍🗨️ In the [Administrators] settings for @{0} on:\n[✅ Add member]\n\n🕚Please wait 1min",
     'es': "👁️‍🗨️ En la configuración de [Administradores] para @{0} en:\n[✅ Agregar miembro]\n\n🕚Espere 1 minuto",
     'fr': "👁️‍🗨️ Dans les paramètres [Administrateurs] pour @{0} sur :\n[✅ Ajouter un membre]\n\n🕚Veuillez patienter 1 min",
     'zh': "👁️‍🗨️ 在@{0}的[管理员]设置中：\n[✅添加成员]\n\n🕚请稍候1分钟",
     'ar': "👁️‍🗨️ في إعدادات [Administrators] لـ @ {0} على:\n[✅ إضافة عضو]\n\n🕚 يرجى الانتظار لمدة دقيقة",
 }
 l_cview_correct = {
-    'ru': "👁️‍🗨️ <b>Введи</b> корректное <b>число</b> авто-просмотров последнего поста канала\n\n👩🏽‍💻 Используй команду /view {0}, чтобы задать количество авто-просмотров (<b>текущее</b> количество: <u>{0}</u>)",
+    'ru': "👁️‍🗨️ <b>Введи</b> корректное <b>число</b> авто-просмотров последнего поста канала\n\n👩🏽‍💻 Используй команду <code>/view {0}</code>, чтобы задать количество авто-просмотров (без подписки: <u>{1}</u>)",
     'en': "👁️‍🗨️ <b>Enter</b> the correct <b>number of</b> auto-views for the last post of the channel\n\n👩🏽‍💻 Use /view {0} to set the number of auto-views ( <b>current</b> number: <u>{0}</u> )",
     'es': "👁️‍🗨️ <b>Ingresa</b> la <b>cantidad correcta de</b> vistas automáticas para la última publicación del canal\n\n👩🏽‍💻 Usa /view {0} para establecer la cantidad de vistas automáticas (número <b>actual</b> : <u>{0}</u> )",
     'fr': "👁️‍🗨️ <b>Entrez</b> le <b>nombre correct de</b> vues automatiques pour le dernier message de la chaîne\n\n👩🏽‍💻 Utilisez /view {0} pour définir le nombre de vues automatiques (nombre <b>actuel</b> : <u>{0}</u> )",
     'zh': "👁️‍🗨️ 为频道的最后一个帖子<b>输入</b>正确<b>的自动观看次数</b>\n\n👩🏽‍💻 使用/view {0}设置自动观看次数（<b>当前</b>次数： <u>{0}</u> ）",
     'ar': "👁️‍🗨️ <b>أدخل</b> <b>العدد</b> الصحيح للمشاهدات التلقائية لآخر مشاركة للقناة\n\n👩🏽‍💻 استخدم /view {0} لتعيين عدد المشاهدات التلقائية (الرقم <b>الحالي</b> : <u>{0}</u> )",
 }
 l_cview_on = {
-    'ru': "👁️‍🗨️ <b>Готово!</b> Текущее количество <b>авто-просмотров</b> на последний пост канала установлено в значение <u>{0}</u>",
+    'ru': "👁️‍🗨️ <b>Готово!</b> Текущее количество <b>авто-просмотров</b> на последний пост канала установлено в значение <u>{0}</u> (без подписки: <u>{1}</u>)",
     'en': "👁️‍🗨️ <b>Done!</b> The current number of <b>auto-views</b> for the channel&#x27;s last post is set to <u>{0}</u>",
     'es': "👁️‍🗨️ <b>Listo!</b> El número actual de <b>visualizaciones automáticas</b> de la última publicación del canal está establecido en <u>{0}.</u>",
     'fr': "👁️‍🗨️ <b>C&#x27;est fait !</b> Le nombre actuel de <b>vues automatiques</b> pour le dernier message de la chaîne est défini sur <u>{0}</u>",
     'zh': "👁️‍🗨️<b>完成！</b>频道上一篇帖子的当前<b>自动观看</b>次数设置为<u>{0}</u>",
     'ar': "👁️‍🗨️ <b>انتهى!</b> تم تعيين العدد الحالي <b>للمشاهدات التلقائية</b> لآخر مشاركة على القناة على <u>{0}</u>",
 }
 l_cview_off = {
@@ -3279,15 +3279,15 @@
     'en': "🪄 <b>Enter</b> a short <b>text</b> that will be added to the end of the channel posts (for example, frequently used #хэштеги )",
     'es': "🪄 <b>Ingrese</b> un <b>texto</b> breve que se agregará al final de las publicaciones del canal (por ejemplo, #хэштеги de uso frecuente)",
     'fr': "🪄 <b>Entrez</b> un court <b>texte</b> qui sera ajouté à la fin des publications de la chaîne (par exemple, #хэштеги fréquemment utilisés)",
     'zh': "🪄<b>输入</b>将添加到频道帖子末尾的短<b>文本</b>（例如，经常使用的#хэштеги ）",
     'ar': "🪄 <b>أدخل</b> <b>نصًا</b> قصيرًا سيتم إضافته إلى نهاية منشورات القناة (على سبيل المثال ، #хэштеги المستخدمة بشكل متكرر)",
 }
 l_cdecor_footer_done = {
-    'ru': "🪄 <b>Готово!</b> <b>Футер</b> из <u>{0}</u>-символов будет использоваться как окончание поста в канале\n\nОпцию можно включить, нажав <b>[✅☑Вкл футер]</b>",
+    'ru': "🪄 <b>Готово!</b> <b>Футер</b> из <u>{0}</u>-символов будет использоваться как окончание поста в канале\n\n👩🏽‍💻 Опцию можно включить, нажав <b>[✅☑Вкл футер]</b>",
     'en': "🪄 <b>Done!</b> <b>The footer</b> of <u>{0}</u> characters will be used as the end of the post in the channel\n\nThis option can be enabled by pressing <b>[✅☑Enable footer]</b>",
     'es': "🪄 <b>Listo!</b> <b>El pie de página</b> de <u>{0}</u> caracteres se utilizará como final de la publicación en el canal\n\nEsta opción se puede habilitar presionando <b>[✅☑Habilitar pie de página]</b>",
     'fr': "🪄 <b>C&#x27;est fait !</b> <b>Le pied de page</b> de <u>{0}</u> caractères sera utilisé comme fin de message dans le canal\n\nCette option peut être activée en appuyant sur <b>[✅☑Activer le pied de page]</b>",
     'zh': "🪄<b>完成！</b> <u>{0}</u>个字符的<b>页脚</b>将用作频道中帖子的结尾\n\n可以通过按<b>[✅☑启用页脚]</b>来启用此选项",
     'ar': "🪄 <b>انتهى!</b> سيتم استخدام <b>تذييل مكون</b> من <u>{0}</u> حرفًا كنهاية للنشر في القناة\n\nيمكن تمكين هذا الخيار بالضغط على <b>[✅☑ تمكين التذييل]</b>",
 }
 l_cdecor_page_on = {
@@ -3339,15 +3339,15 @@
     'ar': "☑️☐إيقاف تنسيق النص",
 }
 # endregion
 
 
 # region cmember_
 l_cmember_text = {
-    'ru': "👥 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> сбор подписчиков канала (с момента подключения бота в канал)\n\n👩🏽‍💻 Для выгрузки подписчиков канала выполни команду /parse",
+    'ru': "👥 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> сбор подписчиков канала\n\n👩🏽‍💻 Для выгрузки подписчиков канала выполни команду /parse",
     'en': "👥 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> the collection of channel subscribers (from the moment the bot joins the channel)\n\n👩🏽‍💻 To unload channel subscribers, run the /parse command",
     'es': "👥 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> la recopilación de suscriptores del canal (desde el momento en que el bot se une al canal)\n\n👩🏽‍💻 Para descargar suscriptores del canal, ejecuta el comando /parse",
     'fr': "👥 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> la collecte des abonnés à la chaîne (à partir du moment où le bot rejoint la chaîne)\n\n👩🏽‍💻 Pour décharger les abonnés à la chaîne, exécutez la commande /parse",
     'zh': "👥<b>点击</b>✅/☑️<b>打开/关闭</b>频道订阅者的收集（从机器人加入频道的那一刻起）\n\n👩🏽‍💻 要卸载频道订阅者，运行 /parse 命令",
     'ar': "👥 <b>انقر</b> فوق ✅ / ☑️ <b>لتشغيل / إيقاف</b> مجموعة مشتركي القناة (من لحظة انضمام الروبوت إلى القناة)\n\n👩🏽‍💻 لإلغاء تحميل مشتركي القناة ، قم بتشغيل الأمر / parse",
 }
 l_cmember_on = {
@@ -3363,15 +3363,15 @@
     'en': "👁️‍🗨️ /view-auto-views disabled",
     'es': "👁️‍🗨️ /view-auto-views deshabilitado",
     'fr': "👁️‍🗨️ /view-auto-views désactivé",
     'zh': "👁️‍🗨️ /view-auto-views 已禁用",
     'ar': "👁️‍🗨️ / عرض-طرق العرض التلقائي معطلة",
 }
 l_cmember_parse = {
-    'ru': "👥 <b>Готово!</b> Собрано реальных участников: <u>{0}</u>\n\n👩🏽‍💻 Старые подписчики будут постепенно пополнять базу, пока у @{1}-бота есть права [✅ Назначение администраторов]\n\n{2}",
+    'ru': "👥 <b>Собрано</b> реальных участников: <u>{0}</u>\n\n👩🏽‍💻 <b>Старые</b> подписчики будут постепенно пополнять базу, пока у @{1}-бота есть права:\n[✅ <i>Назначение администраторов</i>]\n\n{2}\n👩🏽‍💻 <b>Для получения</b> имен пользователей должна быть <a href='{3}'>оформлена подписка</a>",
     'en': "👥 <b>Done!</b> Collected real participants: <u>{0}</u>\n\n👩🏽‍💻 Old subscribers will gradually replenish the database as long as the @{1}-bot has rights [✅ Appointment of administrators]\n\n{2}",
     'es': "👥 <b>Listo!</b> Participantes reales recopilados: <u>{0}</u>\n\n👩🏽‍💻 Los suscriptores antiguos repondrán gradualmente la base de datos siempre que el @{1}-bot tenga derechos [✅ Nombramiento de administradores]\n\n{2}",
     'fr': "👥 <b>C&#x27;est fait !</b> Participants réels collectés : <u>{0}</u>\n\n👩🏽‍💻 Les anciens abonnés reconstitueront progressivement la base de données tant que le @{1}-bot aura des droits [✅ Nomination d'administrateurs]\n\n{2}",
     'zh': "👥<b>完成！</b>收集到的真实参与者： <u>{0}</u>\n\n👩🏽‍💻 只要@{1}-bot 有权限，老订阅者就会逐渐补充数据库【✅管理员任命】\n\n{2}",
     'ar': "👥 <b>انتهى!</b> المشاركون الحقيقيون الذين تم جمعهم: <u>{0}</u>\n\n👩🏽‍💻 سوف يقوم المشتركون القدامى بتجديد قاعدة البيانات تدريجيًا طالما أن @ {1} الروبوت لديه حقوق [✅ تعيين المسؤولين]\n\n{2}",
 }
 l_parse_rights = {
@@ -3400,15 +3400,15 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_group_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> администрирования <b>Telegram</b>-групп:\n\n▪️<b>защита</b> группы от вступления шпионов\n▪️вывод <b>статистики</b> и вовлеченности (%)\n▪️ограничение прав до <b>подписки</b>\n▪️<b>организация</b> бана и антифлуда\n▪️<b>авто-ответы</b> и стоп-слова\n\n❗️Регулярно-обновляемый /content",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> администрирования <b>Telegram</b>-групп:\n\n▪️<b>защита</b> группы от вступления шпионов\n▪️вывод <b>статистики</b> и вовлеченности (%)\n▪️ограничение прав до <b>подписки</b>\n▪️<b>организация</b> бана и антифлуда\n▪️<b>авто-ответы</b> и стоп-слова\n▪️<b>кнопочный</b> счетчик\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to <i>the landing bot</i> администрирования <b>Telegram</b> groups:\n\n▪️ <b>protecting</b> the group from spyware\n▪️displaying <b>statistics</b> and engagement (%)\n▪️restricting rights before <b>subscribing</b> to the channel\n▪️ <b>organizing</b> a ban and anti-flood\n\n❗️you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> администрирования grupos <b>de Telegram</b> :\n\ <b>n▪️proteger</b> al grupo de spyware\n▪️mostrar <b>estadísticas</b> e interacción (%)\n▪️restringir los derechos antes de <b>suscribirse</b> al canal\ <b>n▪️organizar</b> un prohibición y anti-inundación\n\n❗️también puede solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue dans <i>le landing bot</i> администрирования des groupes <b>Telegram</b> :\n\n▪️ <b>protéger</b> le groupe des spywares\n▪️afficher <b>les statistiques</b> et l&#x27;engagement (%)\n▪️restreindre les droits avant de <b>s&#x27;abonner</b> à la chaîne\n▪️ <b>organiser</b> un interdiction et anti-flood\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio de Ferey",
     'zh': "🌱 {0}，欢迎使用администрирования <b>Telegram</b>群组的<i>登陆机器人</i>：\n\n▪️<b>保护</b>群组免受间谍软件的侵害\n▪️ 显示<b>统计数据</b>和参与度 (%)\n▪️ 在<b>订阅</b>频道之前限制权利\n▪️<b>组织</b>一个ban 和 anti-flood\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوط</i> администрирования مجموعات <b>Telegram</b> :\n\n▪️ <b>حماية</b> المجموعة من برامج التجسس\n▪️ عرض <b>الإحصائيات</b> والمشاركة (٪)\n▪️ تقييد الحقوق قبل <b>الاشتراك</b> في القناة\n▪️ <b>تنظيم</b> الحظر ومكافحة الفيضانات\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
 l_subscribe_group = {
@@ -3900,15 +3900,15 @@
     'es': "⚠️ Estado <b>{0}</b> para {1}:\n\n",
     'fr': "⚠️ Statut <b>{0}</b> pour {1} :\n\n",
     'zh': "⚠️ {1} 的状态<b>{0}</b> ：\n\n",
     'ar': "⚠️ الحالة <b>{0}</b> لـ {1}:\n\n",
 }
 
 l_transfer_reply = {
-    'ru': "⚠️ Используй команду /transfer в <b>ответном</b> сообщении пользователя, которому вы хотите передать права",
+    'ru': "⚠️ <b>Используй</b> команду /transfer в <b>ответном</b> сообщении пользователя, которому вы хотите передать права",
     'en': "⚠️ Use the /transfer command in <b>the response</b> message of the user you want to transfer rights to",
     'es': "⚠️ Use el comando /transfer en <b>el mensaje de respuesta</b> del usuario al que desea transferir los derechos",
     'fr': "⚠️ Utilisez la commande /transfer dans <b>le message de réponse</b> de l'utilisateur à qui vous souhaitez transférer les droits",
     'zh': "⚠️ 在你想转让权限的用户的<b>响应</b>消息中使用 /transfer 命令",
     'ar': "⚠️ استخدم الأمر / transfer في رسالة <b>استجابة</b> المستخدم الذي تريد نقل الحقوق إليه",
 }
 l_button_handler = {
```

### Comparing `yeref-0.1.98/yeref/yeref.py` & `yeref-0.1.99/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -3108,22 +3108,22 @@
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result.as_markup()
 
 
-async def create_replymarkup2(bot, offer_id, OFFER_BUTTON, type_='pst'):
+async def create_replymarkup2(bot, offer_id, OFFER_BUTTON, type_='pst', is_counter=False):
     result = None
     try:
         if OFFER_BUTTON is None or OFFER_BUTTON == '': return
         tmp = []
         buttons = []
         offer_id = int(offer_id)
-        dic_btns = await check_buttons(bot, None, OFFER_BUTTON)
+        dic_btns = await check_buttons(bot, None, OFFER_BUTTON, is_counter)
         result = InlineKeyboardBuilder()
         for k, v in dic_btns.items():
             try:
                 if v[0]:
                     if len(tmp) > 0 and tmp[-1] is None:
                         result.add(*buttons)
                         if 'ᴵ' in v[0]:
@@ -3151,15 +3151,15 @@
     except Exception as e:
         logger.info(log_ % str(e))
         pass
     finally:
         return result
 
 
-async def check_buttons(bot, chat_id, txt):
+async def check_buttons(bot, chat_id, txt, is_counter=False):
     result = {}
     txt = txt.strip()
     try:
         start_ = []
         finish_ = []
         for ix in range(0, len(txt)):
             try:
@@ -3186,15 +3186,15 @@
                     if len(split_btn) > 1:
                         btn_name = split_btn[0].strip() if len(split_btn) > 1 else "🔗 Go"
                         btn_link = split_btn[-1].strip()
                         if not await is_url(btn_link):
                             await bot.send_message(chat_id, f"🔗 {btn_link}: invalid")
                             return
                     else:
-                        btn_name = split_btn[0]
+                        btn_name =  f"⁰{split_btn[0]}" if is_counter else split_btn[0]
                         # btn_link = cleanhtml(split_btn[0])[:20]
                         # btn_link = f"btn_{btn_link.encode('utf-8').hex()}"
                         btn_link = f"btn_"
 
                     result[ix] = [btn_name, btn_link]
             except Exception as e:
                 logger.info(log_ % str(e))
```

