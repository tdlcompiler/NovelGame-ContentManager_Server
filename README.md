# NovelGame - Content Manager Server

Скомпилированный сервер для работы подсистемы наполнения контентом игр-новелл (дипломная работа).

## Установка

### 1. Установка .NET Runtime 6.0

Если на вашем компьютере не установлен .NET Runtime 6.0, выполните следующие шаги:

#### Для Windows

1. Перейдите на официальный сайт .NET и загрузите установщик .NET Runtime 6.0: [ссылка на скачивание для 64-битной версии Windows](https://dotnet.microsoft.com/ru-ru/download/dotnet/thank-you/runtime-6.0.31-windows-x64-installer) или [ссылка на скачивание для 32-битной версии Windows](https://dotnet.microsoft.com/ru-ru/download/dotnet/thank-you/runtime-6.0.31-windows-x86-installer).
   
2. Запустите скачанный установщик и следуйте инструкциям по установке.

### 2. Установка и настройка MySQL

Для хранения данных сервера вам потребуется база данных MySQL. Рекомендую использовать XAMPP для удобства развертывания.

#### Установка MySQL с использованием XAMPP

1. Скачайте и установите XAMPP с официального сайта: [ссылка на скачивание](https://www.apachefriends.org/download.html).
   
2. Запустите XAMPP и запустите сервис MySQL.

### 3. Заполнение конфигурации server_config.json

Перед запуском сервера необходимо настроить файл конфигурации `server_config.json`, который должен находиться в директории сервера. Пример содержимого файла:

```json
{
	"port": 12361,
	"dbname": "contentmanagerapp_db",
	"dbendpoint": "localhost",
	"dbcredentials":
	{
		"username": "empty",
		"password": "empty"
	}
}
```

### 4. Запуск сервера

После установки .NET Runtime 6.0 и настройки MySQL, вы можете запустить сервер.

1. [Скачайте](https://github.com/tdlcompiler/NovelGame-ContentManager_Server/archive/refs/heads/main.zip) последнюю версию сервера с этого репозитория.

2. Разархивируйте скачанный архив и перейдите в директорию с сервером.

3. Запустите сервер, запустив файл `NovelGame.Server.exe`.

Теперь клиенты смогут подключиться к серверу, если в их конфигурациях будут указаны верные данные для подключения к серверу.
