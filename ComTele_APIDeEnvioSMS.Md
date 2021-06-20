# SMS

## api de envio sms

veja como é fácil e rápido integrar seu sistema com a api de envio da comtele

dotnet add package Comtele

### PYTHON
...
# instalação da biblioteca
# pip install comtele_sdk

from comtele_sdk.textmessage_service import TextMessageService

__api_key = ‘XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX’
textmessage_service = TextMessageService(__api_key)
result = textmessage_service.send(‘Sender’, ‘Content’, [‘Receivers’])
...

### .NET
...
// Instalação da biblioteca
// Install-Package Comtele.Sdk

using System;
using Comtele.Sdk.Services;

static string API_KEY = “XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX”;
var textMessageService = new TextMessageService(API_KEY);
var result = textMessageService.Send(“Sender”, “Content”, new string[] {“Receivers”});
...

### .NET CORE
...
/ Instalação da biblioteca
// dotnet add package Comtele.Sdk

using System;
using Comtele.Sdk.Services;

static string API_KEY = “XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX”;
var textMessageService = new TextMessageService(API_KEY);
var result = textMessageService.Send(“Sender”, “Content”, new string[] {“Receivers”});
...

### NODE JS
...
// Instalação da biblioteca
// npm install comtele-sdk

const TextMessageService = require(‘comtele-sdk’).TextMessageService;

const apiKey = ‘XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX’;
var textMessageService = new TextMessageService(apiKey);
textMessageService.send(‘Sender’, ‘Content’, [‘Receivers’], data => console.log(data));
...

### JAVA
...
// Instalação da biblioteca
// https://github.com/comtele/comtele-java-sdk/blob/master/ComteleSDK-Java.zip

import models.*;
import service.Accounts;

static string API_KEY = “XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX”;
TextMessageService textMessageService = new TextMessageService(API_KEY);
DefaultSeviceResult sendResult = textMessageService.Send(“Sender”, “Content”, Arrays.asList(“Receivers”));
...

### RUBY	
...
# Instalação da biblioteca
# gem install comtele_sdk

require ‘comtele_sdk’;
include ComteleSdk

API_KEY = ‘XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX’;
textmessage_service = TextMessageService.new(API_KEY);
result = textmessage_service.send(‘Sender’, ‘Content’, [‘Receivers’]);
...

### PHP
...
// Instalação da biblioteca
// composer require comtele/comtele_sdk

require_once “vendor/autoload.php”;
use ComteleServicesTextMessageService;

const API_KEY = “XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX”;

$textMessageService = new TextMessageService(API_KEY);
$result = $textMessageService->send(“Sender”, “Content”, [“Receivers”]);
...

### PHP Classic
...
// Instalação da biblioteca
// https://github.com/comtele/comtele-php-classic-sdk/blob/master/ComteleSDK-PHP-Classic.zip

require_once “textmessage_service.php”;

$API_KEY = “XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX”;
$result = send(“Sender”, “Content”, [“Receivers”]);
...

### Importante visite o site da COMTELE para ver as ultimas novidades e se inteirar das novas apis

[Artigo original](https://comtele.com.br/integracao-api-sms/)