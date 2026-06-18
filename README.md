
                                  DeployX

 EN - ENGLISH
Welcome to DeployX! 
DeployX is a powerful graphical tool for Windows designed to interact with 
Android devices via ADB (Android Debug Bridge). Its goal is to make maintaining, 
debugging, and managing your phone or tablet easier without needing to type 
complex console commands.

<img width="786" height="682" alt="Captura de pantalla 2026-06-18 102157" src="https://github.com/user-attachments/assets/66c73e65-3895-4a0d-b04c-be47c2637283" />
<img width="786" height="682" alt="Captura de pantalla 2026-06-18 102148" src="https://github.com/user-attachments/assets/30358596-710f-4be0-9eaf-b7f5eaeb4e00" />
<img width="786" height="682" alt="Captura de pantalla 2026-06-18 102135" src="https://github.com/user-attachments/assets/ca48d9ea-87c1-4785-92e5-3068a0e686b2" />
<img width="786" height="682" alt="Captura de pantalla 2026-06-18 102122" src="https://github.com/user-attachments/assets/d0cd5ee3-5da9-47f9-afe4-2f7c08958b8e" />
<img width="786" height="682" alt="Captura de pantalla 2026-06-18 102116" src="https://github.com/user-attachments/assets/99c96593-cd08-42d4-9ed7-ecffff9378cc" />
<img width="786" height="682" alt="Captura de pantalla 2026-06-18 102101" src="https://github.com/user-attachments/assets/71b095dc-85c7-400f-8bbc-c8b1fd318f9f" />

--------------------------------------------------------------------------------
 1. PREREQUISITES AND IMPORTANT WARNINGS
--------------------------------------------------------------------------------
For DeployX to work properly, you need the following:

* Windows 10 or Windows 11.
* USB drivers for your phone installed on your PC (if Windows doesn't detect it).
* A data transfer USB cable (cables that are "charge-only" will not work).
* PROGRAM INTEGRITY: This software depends on a browser engine (WebView2) 
  and other libraries. **NEVER take the DeployX.exe file out of its original folder**. 
  If you separate it from files like "WebView2Loader.dll" or the "runtimes" folder, 
  the program will crash and will not work.

--------------------------------------------------------------------------------
 2. STEP-BY-STEP USER MANUAL
--------------------------------------------------------------------------------
Step 1: Prepare the phone (USB Debugging)
Before connecting the phone to the computer, you must enable communication:
  1. Go to Settings > About phone on your Android.
  2. Tap "Build number" 7 consecutive times to enable Developer Options.
  3. Go back, enter "Developer Options" and turn on "USB Debugging".

Step 2: Connection and Automatic Detection
  1. Open "DeployX.exe". You will see the welcome screen. Initially, the sidebar 
     buttons will be grayed out (disabled). This is normal and is a security measure.
  2. Connect your phone to the PC using the USB cable.
  3. Check your phone's screen: a prompt will ask "Allow USB debugging from this 
     computer?". Check the "Always allow" box and tap OK.
  4. Magic! DeployX will automatically detect your device in seconds, and the 
     menu buttons will light up indicating you are connected.

Step 3: Safe Disconnection
  When you are done using the program, simply unplug the cable. DeployX will 
  notice instantly and lock the buttons again to protect the system.

--------------------------------------------------------------------------------
 3. DETAILED FUNCTION DESCRIPTION (SIDEBAR MENU)
--------------------------------------------------------------------------------
* [ DEVICE ]: The main information panel. View essential technical details of 
  your connected device (model, Android version, battery level, etc.).
* [ INSTALL ]: The sideloading manager. Install applications (.apk or .apks) 
  directly from your PC to the phone silently.
* [ APPS ]: A complete package manager. View installed apps, uninstall them 
  (including bloatware), or clear their data/cache.
* [ EXPLORER ]: A two-way file manager. Easily extract files from your phone 
  to your PC (Pull) or send them to your phone (Push) visually.
* [ SCREEN ]: Visual tools. Take exact screenshots of your phone and save them 
  directly to your PC.
* [ LOGCAT ]: Shows a real-time log of everything happening inside the Android 
  system. Essential for developers or diagnosing crashing apps.
* [ MONITOR ]: Live performance tool. Monitor RAM consumption and CPU usage 
  in real-time.

--------------------------------------------------------------------------------
 4. COMMON TROUBLESHOOTING (FAQ)
--------------------------------------------------------------------------------
Q: I connect the phone but the DeployX buttons are still gray (disabled).
A: This happens for three main reasons:
   1. USB DEBUGGING IS NOT ENABLED. This is the most common error. Go to your 
      phone settings, enter "Developer Options", and turn on "USB Debugging".
   2. Missing permissions. Unlock your phone and check the screen; a prompt will 
      ask "Allow USB debugging?". Check "Always allow" and tap OK.
   3. Your USB cable does not support data. Cheap cables are often charge-only. 
      Try using the original cable or one confirmed to transfer data.

Q: The program opens, but crashes almost immediately or throws a fatal error.
A: You are missing vital files. Ensure the "WebView2Loader.dll" file is in the 
   exact same folder as "DeployX.exe".

Q: I try to install an APK but get an error.
A: Check that you have enough storage space and that a newer version of the app 
   isn't already installed.

--------------------------------------------------------------------------------
Credits:
Developed by Pablo Villavicencio
Connection Engine: Android Debug Bridge (ADB)
Web Interface: Microsoft Edge WebView2

 ES - ESPAÑOL
¡Bienvenido a DeployX! 
DeployX es una potente herramienta gráfica para Windows diseñada para interactuar 
con dispositivos Android a través de ADB (Android Debug Bridge). Su objetivo es 
facilitar el mantenimiento, la depuración y la gestión de tu teléfono o tablet 
sin necesidad de escribir complicados comandos en la consola.

--------------------------------------------------------------------------------
 1. REQUISITOS PREVIOS Y ADVERTENCIAS IMPORTANTES
--------------------------------------------------------------------------------
Para que DeployX funcione correctamente, necesitas cumplir con lo siguiente:

* Windows 10 o Windows 11.
* Drivers USB de tu teléfono instalados en la PC (si Windows no lo reconoce por defecto).
* Un cable USB de transferencia de datos (los cables que son "solo para carga" no funcionarán).
* INTEGRIDAD DEL PROGRAMA: Este programa depende de un motor de navegación (WebView2) 
  y otras librerías. **NUNCA saques el archivo DeployX.exe de su carpeta original**. 
  Si lo separas de archivos como "WebView2Loader.dll" o la carpeta "runtimes", 
  el programa se cerrará de golpe y no funcionará.

--------------------------------------------------------------------------------
 2. MANUAL DE USO PASO A PASO
--------------------------------------------------------------------------------
Paso 1: Preparar el teléfono (Depuración USB)
Antes de conectar el teléfono a la computadora, debes habilitar la comunicación:
  1. Ve a Configuración > Acerca del teléfono en tu Android.
  2. Toca 7 veces seguidas donde dice "Número de compilación" para activar las 
     Opciones de Desarrollador.
  3. Regresa, entra a las "Opciones de Desarrollador" y activa "Depuración USB".

Paso 2: Conexión y Detección Automática
  1. Abre "DeployX.exe". Verás la pantalla de bienvenida. Inicialmente, notarás 
     que los botones del menú lateral están desactivados (en gris). Esto es 
     completamente normal y es una medida de seguridad.
  2. Conecta tu teléfono a la PC con el cable USB.
  3. Revisa la pantalla de tu teléfono: te aparecerá un aviso preguntando 
     "¿Permitir depuración USB desde esta computadora?". Marca la casilla 
     "Permitir siempre" y dale en Aceptar.
  4. ¡Magia! DeployX detectará tu dispositivo automáticamente en cuestión de 
     segundos y los botones del menú cobrarán vida indicando que estás conectado.

Paso 3: Desconexión Segura
  Cuando termines de usar el programa, simplemente desconecta el cable. DeployX 
  se dará cuenta al instante y volverá a bloquear los botones para proteger el sistema.

--------------------------------------------------------------------------------
 3. DESCRIPCIÓN DETALLADA DE LAS FUNCIONES (MENÚ LATERAL)
--------------------------------------------------------------------------------
* [ DISPOSITIVO ]: Es el panel principal de información. Aquí podrás ver los detalles 
  técnicos esenciales de tu equipo conectado (modelo, versión de Android, batería, etc.).
* [ INSTALAR ]: El gestor de sideloading. Te permite instalar aplicaciones (.apk o .apks) 
  directamente desde tu PC al teléfono de forma silenciosa.
* [ APLICACIONES ]: Un administrador de paquetes completo. Puedes ver apps instaladas, 
  desinstalarlas (incluso bloatware) o limpiar sus datos/caché.
* [ EXPLORADOR ]: Un gestor de archivos bidireccional. Te permite extraer archivos 
  del teléfono a tu PC (Pull) o enviarlos al teléfono (Push) visualmente.
* [ PANTALLA ]: Herramientas visuales. Te permite tomar capturas de pantalla 
  (screenshots) exactas de tu teléfono y guardarlas en la PC.
* [ LOGCAT ]: Muestra un registro en tiempo real de todo lo que ocurre en el sistema 
  Android. Indispensable para desarrolladores o para diagnosticar apps que fallan.
* [ MONITOR ]: Herramienta para vigilar el consumo de memoria RAM y el uso de CPU 
  del teléfono en tiempo real.

--------------------------------------------------------------------------------
 4. SOLUCIÓN DE PROBLEMAS COMUNES (FAQ)
--------------------------------------------------------------------------------
P: Conecto el celular pero los botones de DeployX siguen en gris (desactivados).
R: Esto pasa por tres razones principales:
   1. NO TIENES LA DEPURACIÓN USB ACTIVADA. Este es el error más común. Ve a la 
      configuración de tu teléfono, entra a "Opciones de Desarrollador" y 
      asegúrate de encender la "Depuración USB".
   2. Falta dar permisos en el teléfono. Revisa la pantalla de tu celular 
      desbloqueado; te aparecerá un aviso preguntando "¿Permitir depuración USB?", 
      marca "Permitir siempre" y dale en Aceptar.
   3. Tu cable USB no soporta datos. Muchos cables baratos son solo para cargar 
      batería. Intenta con el cable original o uno que confirme transferencia de datos.

P: El programa abre, pero se cierra casi inmediatamente o marca un error fatal.
R: Te faltan archivos vitales. Asegúrate de que el archivo "WebView2Loader.dll" 
   esté exactamente en la misma carpeta que "DeployX.exe".

P: Intento instalar un APK pero me da error.
R: Verifica que tengas suficiente espacio de almacenamiento y que la aplicación 
   no esté ya instalada con una versión más nueva.

--------------------------------------------------------------------------------
Créditos:
Desarrollado por Pablo Villavicencio
Motor de conexión: Android Debug Bridge (ADB)
Interfaz Web: Microsoft Edge WebView2

 FR - FRANÇAIS
Bienvenue sur DeployX ! 
DeployX est un outil graphique puissant pour Windows conçu pour interagir avec 
les appareils Android via ADB (Android Debug Bridge). Son but est de faciliter 
la maintenance, le débogage et la gestion de votre téléphone ou tablette sans 
avoir besoin d'écrire des commandes de console complexes.

--------------------------------------------------------------------------------
 1. PRÉREQUIS ET AVERTISSEMENTS IMPORTANTS
--------------------------------------------------------------------------------
Pour que DeployX fonctionne correctement, vous avez besoin de ce qui suit :

* Windows 10 ou Windows 11.
* Les pilotes (drivers) USB de votre téléphone installés sur le PC.
* Un câble USB de transfert de données (les câbles "charge uniquement" ne fonctionneront pas).
* INTÉGRITÉ DU PROGRAMME : Ce logiciel dépend d'un moteur de navigation (WebView2) 
  et d'autres bibliothèques. **NE SORTEZ JAMAIS le fichier DeployX.exe de son dossier 
  d'origine**. Si vous le séparez de fichiers tels que "WebView2Loader.dll" ou du 
  dossier "runtimes", le programme plantera et ne fonctionnera pas.

--------------------------------------------------------------------------------
 2. MANUEL D'UTILISATION ÉTAPE PAR ÉTAPE
--------------------------------------------------------------------------------
Étape 1 : Préparer le téléphone (Débogage USB)
Avant de connecter le téléphone à l'ordinateur, vous devez activer la communication :
  1. Allez dans Paramètres > À propos du téléphone sur votre Android.
  2. Appuyez 7 fois de suite sur "Numéro de build" pour activer les Options 
     pour les développeurs.
  3. Revenez en arrière, entrez dans "Options pour les développeurs" et activez 
     le "Débogage USB".

Étape 2 : Connexion et Détection Automatique
  1. Ouvrez "DeployX.exe". Vous verrez l'écran de bienvenue. Initialement, les 
     boutons du menu latéral seront grisés (désactivés). C'est une mesure de sécurité.
  2. Connectez votre téléphone au PC avec le câble USB.
  3. Vérifiez l'écran de votre téléphone : un message demandera "Autoriser le 
     débogage USB ?". Cochez "Toujours autoriser" et appuyez sur OK.
  4. Magie ! DeployX détectera automatiquement votre appareil en quelques secondes.

Étape 3 : Déconnexion Sécurisée
  Lorsque vous avez terminé, débranchez simplement le câble. DeployX le remarquera 
  instantanément et verrouillera les boutons pour protéger le système.

--------------------------------------------------------------------------------
 3. DESCRIPTION DÉTAILLÉE DES FONCTIONS (MENU LATÉRAL)
--------------------------------------------------------------------------------
* [ APPAREIL ] : Panneau d'informations principal (modèle, version Android, batterie).
* [ INSTALLER ] : Gestionnaire d'installation (sideloading) d'applications (.apk).
* [ APPLICATIONS ] : Gestionnaire de paquets pour désinstaller ou effacer le cache.
* [ EXPLORATEUR ] : Gestionnaire de fichiers bidirectionnel (Pull/Push).
* [ ÉCRAN ] : Permet de prendre des captures d'écran de votre téléphone vers le PC.
* [ LOGCAT ] : Affiche un journal en temps réel du système Android.
* [ MONITEUR ] : Outil de surveillance en direct de la RAM et du CPU.

--------------------------------------------------------------------------------
 4. DÉPANNAGE COURANT (FAQ)
--------------------------------------------------------------------------------
Q : Je connecte le téléphone mais les boutons DeployX restent gris.
R : Cela se produit pour trois raisons principales :
   1. LE DÉBOGAGE USB N'EST PAS ACTIVÉ. C'est l'erreur la plus courante.
   2. Autorisations manquantes. Déverrouillez votre téléphone et acceptez l'invite ADB.
   3. Votre câble USB ne prend pas en charge les données. Essayez un autre câble.

Q : Le programme s'ouvre mais se ferme presque immédiatement.
R : Il vous manque des fichiers vitaux. Assurez-vous que le fichier "WebView2Loader.dll" 
    se trouve dans le même dossier que "DeployX.exe".

--------------------------------------------------------------------------------
Crédits :
Développé par Pablo Villavicencio
Moteur de connexion : Android Debug Bridge (ADB)
Interface Web : Microsoft Edge WebView2

 DE - DEUTSCH
Willkommen bei DeployX! 
DeployX ist ein leistungsstarkes grafisches Tool für Windows, das für die Interaktion 
mit Android-Geräten über ADB (Android Debug Bridge) entwickelt wurde. Es erleichtert 
die Wartung und Verwaltung Ihres Telefons, ohne Konsolenbefehle eingeben zu müssen.

--------------------------------------------------------------------------------
 1. VORAUSSETZUNGEN UND WICHTIGE WARNHINWEISE
--------------------------------------------------------------------------------
Damit DeployX funktioniert, benötigen Sie:

* Windows 10 oder Windows 11.
* Installierte USB-Treiber für Ihr Telefon.
* Ein USB-Datenkabel (reine Ladekabel funktionieren nicht).
* PROGRAMMINTEGRITÄT: Diese Software ist von einer Browser-Engine (WebView2) 
  abhängig. **ENTFERNEN SIE NIEMALS die Datei DeployX.exe aus ihrem ursprünglichen 
  Ordner**. Wenn Sie sie von "WebView2Loader.dll" oder dem "runtimes"-Ordner 
  trennen, stürzt das Programm ab.

--------------------------------------------------------------------------------
 2. SCHRITT-FÜR-SCHRITT BEDIENUNGSANLEITUNG
--------------------------------------------------------------------------------
Schritt 1: Telefon vorbereiten (USB-Debugging)
  1. Gehen Sie auf Ihrem Android zu Einstellungen > Über das Telefon.
  2. Tippen Sie 7 Mal auf "Build-Nummer", um die Entwickleroptionen zu aktivieren.
  3. Gehen Sie zurück zu den Entwickleroptionen und aktivieren Sie "USB-Debugging".

Schritt 2: Verbindung und automatische Erkennung
  1. Öffnen Sie "DeployX.exe". Die Menüschaltflächen sind zunächst aus Sicherheitsgründen deaktiviert (grau).
  2. Verbinden Sie Ihr Telefon über das USB-Kabel mit dem PC.
  3. Auf dem Bildschirm Ihres Telefons erscheint die Meldung "USB-Debugging zulassen?". 
     Setzen Sie ein Häkchen bei "Immer zulassen" und tippen Sie auf OK.
  4. DeployX erkennt Ihr Gerät automatisch.

Schritt 3: Sichere Trennung
  Trennen Sie einfach das Kabel. DeployX sperrt die Tasten automatisch wieder.

--------------------------------------------------------------------------------
 3. DETAILLIERTE FUNKTIONSBESCHREIBUNG (SEITENMENÜ)
--------------------------------------------------------------------------------
* [ GERÄT ]: Hauptinformationsbereich (Modell, Android-Version, Akku).
* [ INSTALLIEREN ]: Sideloading-Manager zum direkten Installieren von .apk-Dateien.
* [ ANWENDUNGEN ]: Paketmanager zum Deinstallieren von Apps oder Löschen des Caches.
* [ EXPLORER ]: Dateimanager zum Extrahieren (Pull) oder Senden (Push) von Dateien.
* [ BILDSCHIRM ]: Erstellen Sie Screenshots Ihres Telefons und speichern Sie diese auf dem PC.
* [ LOGCAT ]: Zeigt das Echtzeitprotokoll des Android-Systems an.
* [ MONITOR ]: Echtzeit-Überwachung von RAM- und CPU-Auslastung.

--------------------------------------------------------------------------------
 4. HÄUFIGE PROBLEMLÖSUNGEN (FAQ)
--------------------------------------------------------------------------------
F: Ich schließe das Telefon an, aber die Tasten bleiben grau.
A: Dafür gibt es drei Hauptgründe:
   1. USB-DEBUGGING IST NICHT AKTIVIERT. Dies ist der häufigste Fehler.
   2. Fehlende Berechtigungen. Entsperren Sie das Telefon und akzeptieren Sie ADB.
   3. Das USB-Kabel unterstützt keine Datenübertragung.

F: Das Programm schließt sich sofort nach dem Öffnen.
A: Stellen Sie sicher, dass sich "WebView2Loader.dll" im selben Ordner wie "DeployX.exe" befindet.

--------------------------------------------------------------------------------
Credits:
Entwickelt von Pablo Villavicencio
Verbindungs-Engine: Android Debug Bridge (ADB)
Web-Oberfläche: Microsoft Edge WebView2

================================================================================
 PT - PORTUGUÊS
================================================================================
Bem-vindo ao DeployX! 
DeployX é uma poderosa ferramenta gráfica para Windows projetada para interagir 
com dispositivos Android via ADB (Android Debug Bridge). Seu objetivo é facilitar 
a manutenção, depuração e gerenciamento do seu telefone ou tablet sem precisar 
digitar comandos complexos.

--------------------------------------------------------------------------------
 1. PRÉ-REQUISITOS E AVISOS IMPORTANTES
--------------------------------------------------------------------------------
Para que o DeployX funcione corretamente, você precisa de:

* Windows 10 ou Windows 11.
* Drivers USB do seu telefone instalados no PC.
* Um cabo USB de transferência de dados (cabos apenas para carga não funcionarão).
* INTEGRIDADE DO PROGRAMA: Este software depende de um motor de navegador (WebView2) 
  e outras bibliotecas. **NUNCA tire o arquivo DeployX.exe de sua pasta original**. 
  Se você separá-lo de arquivos como "WebView2Loader.dll" ou da pasta "runtimes", 
  o programa não funcionará.

--------------------------------------------------------------------------------
 2. MANUAL DO USUÁRIO PASSO A PASSO
--------------------------------------------------------------------------------
Passo 1: Preparar o telefone (Depuração USB)
  1. Vá para Configurações > Sobre o telefone no seu Android.
  2. Toque 7 vezes seguidas no "Número da versão" para ativar as Opções do Desenvolvedor.
  3. Volte, entre em "Opções do Desenvolvedor" e ative a "Depuração USB".

Passo 2: Conexão e Detecção Automática
  1. Abra "DeployX.exe". Inicialmente, os botões estarão desativados (cinza). 
     Isso é uma medida de segurança.
  2. Conecte seu telefone ao PC com o cabo USB.
  3. Verifique a tela do seu telefone: um aviso perguntará "Permitir depuração USB?". 
     Marque "Sempre permitir" e toque em OK.
  4. O DeployX detectará automaticamente seu dispositivo em segundos.

Passo 3: Desconexão Segura
  Ao terminar, basta desconectar o cabo. O DeployX bloqueará os botões instantaneamente.

--------------------------------------------------------------------------------
 3. DESCRIÇÃO DETALHADA DAS FUNÇÕES (MENU LATERAL)
--------------------------------------------------------------------------------
* [ DISPOSITIVO ]: Painel principal de informações (modelo, versão do Android, bateria).
* [ INSTALAR ]: Gerenciador de instalação (sideload) para aplicativos (.apk ou .apks).
* [ APLICATIVOS ]: Gerenciador de pacotes para desinstalar apps ou limpar o cache.
* [ EXPLORADOR ]: Gerenciador de arquivos (Pull e Push).
* [ TELA ]: Permite tirar capturas de tela e salvá-las no PC.
* [ LOGCAT ]: Mostra o log em tempo real do sistema Android.
* [ MONITOR ]: Ferramenta de desempenho ao vivo (RAM e CPU).

--------------------------------------------------------------------------------
 4. SOLUÇÃO DE PROBLEMAS COMUNS (FAQ)
--------------------------------------------------------------------------------
P: Conecto o celular, mas os botões continuam cinza.
R: Isso acontece por três motivos principais:
   1. A DEPURAÇÃO USB NÃO ESTÁ ATIVADA. Este é o erro mais comum.
   2. Falta de permissões. Desbloqueie a tela e aceite o aviso ADB.
   3. Seu cabo USB não suporta transferência de dados.

P: O programa abre, mas fecha quase imediatamente com um erro fatal.
R: Faltam arquivos vitais. Certifique-se de que o arquivo "WebView2Loader.dll" 
   esteja exatamente na mesma pasta que "DeployX.exe".

--------------------------------------------------------------------------------
Créditos:
Desenvolvido por Pablo Villavicencio
Motor de conexão: Android Debug Bridge (ADB)
Interface Web: Microsoft Edge WebView2

 ZH - 中文 (CHINESE)
欢迎使用 DeployX！
DeployX 是一款功能强大的 Windows 图形化工具，旨在通过 ADB (Android Debug Bridge) 
与 Android 设备进行交互。它的目标是简化设备的维护、调试和管理，让您无需在控制台中
输入复杂的命令。

--------------------------------------------------------------------------------
 1. 先决条件和重要警告
--------------------------------------------------------------------------------
为了让 DeployX 正常工作，您需要满足以下条件：

* Windows 10 或 Windows 11。
* 电脑上已安装您手机的 USB 驱动程序。
* 支持数据传输的 USB 数据线（"仅充电"的数据线无效）。
* 程序完整性：本软件依赖于浏览器引擎 (WebView2) 及其他组件。**切勿将 DeployX.exe 
  文件移出其原始文件夹**。如果您将其与 "WebView2Loader.dll" 或 "runtimes" 文件夹
  分开，程序将会崩溃且无法运行。

--------------------------------------------------------------------------------
 2. 分步使用手册
--------------------------------------------------------------------------------
第 1 步：准备手机（USB 调试）
在将手机连接到电脑之前，必须开启通信功能：
  1. 在 Android 手机上进入"设置" > "关于手机"。
  2. 连续点击"版本号" 7 次，以启用"开发者选项"。
  3. 返回上一页，进入"开发者选项"，并开启"USB 调试"。

第 2 步：连接与自动检测
  1. 打开 "DeployX.exe"。起初，侧边栏按钮将显示为灰色（禁用）。这属于正常现象，
     也是一种安全机制。
  2. 使用 USB 数据线将手机连接到电脑。
  3. 查看手机屏幕：会弹出一个提示，询问"是否允许 USB 调试？"。勾选"始终允许"并点击确定。
  4. DeployX 会在几秒钟内自动检测到您的设备。

第 3 步：安全断开连接
  使用完毕后，只需拔下数据线即可。DeployX 会立即锁定按钮以保护系统。

--------------------------------------------------------------------------------
 3. 功能详细说明（侧边栏菜单）
--------------------------------------------------------------------------------
* [ 设备 ]：主要信息面板。查看设备的型号、Android 版本、电池等。
* [ 安装 ]：应用安装管理器。将 .apk 文件从电脑直接静默安装到手机。
* [ 应用程序 ]：完整的包管理器。可卸载应用程序或清除缓存。
* [ 资源管理器 ]：双向文件管理器。方便地在电脑和手机之间提取 (Pull) 或发送 (Push) 文件。
* [ 屏幕 ]：视觉工具。为手机截图并直接保存在电脑上。
* [ LOGCAT ]：实时显示 Android 系统的日志，用于应用诊断。
* [ 监控 ]：实时监控 RAM 和 CPU 使用情况。

--------------------------------------------------------------------------------
 4. 常见问题解答 (FAQ)
--------------------------------------------------------------------------------
问：我连接了手机，但 DeployX 的按钮依然是灰色的。
答：这主要有三个原因：
   1. 未开启 USB 调试。这是最常见的错误。
   2. 缺少权限。请解锁手机并接受屏幕上的 ADB 授权提示。
   3. USB 数据线不支持数据传输。

问：程序打开后几乎立即闪退。
答：缺少关键文件。请确保 "WebView2Loader.dll" 与 "DeployX.exe" 位于同一个文件夹中。

--------------------------------------------------------------------------------
鸣谢：
开发者：Pablo Villavicencio
连接引擎：Android Debug Bridge (ADB)
网页接口：Microsoft Edge WebView2

================================================================================
 JA - 日本語 (JAPANESE)
================================================================================
DeployX へようこそ！
DeployX は、ADB（Android Debug Bridge）を介して Android デバイスと通信する
ために設計された強力な Windows 用グラフィカルツールです。複雑なコマンドを
入力することなく、デバイスのメンテナンスや管理を簡単に行うことができます。

--------------------------------------------------------------------------------
 1. 前提条件と重要な警告
--------------------------------------------------------------------------------
DeployX を正しく動作させるためには、以下が必要です：

* Windows 10 または Windows 11。
* PC にインストールされたデバイスの USB ドライバ。
* データ転送可能な USB ケーブル（「充電専用」ケーブルは機能しません）。
* プログラムの完全性：本ソフトウェアはブラウザエンジン（WebView2）等に依存しています。
  **DeployX.exe ファイルを元のフォルダーから絶対に移動しないでください**。
  「WebView2Loader.dll」や「runtimes」フォルダーから切り離すと、プログラムは
  クラッシュして動作しません。

--------------------------------------------------------------------------------
 2. ステップバイステップ・ユーザーマニュアル
--------------------------------------------------------------------------------
ステップ 1：スマートフォンの準備（USB デバッグ）
  1. Android の「設定」>「デバイス情報」に移動します。
  2. 「ビルド番号」を7回連続でタップし、開発者向けオプションを有効にします。
  3. 戻って「開発者向けオプション」に入り、「USB デバッグ」をオンにします。

ステップ 2：接続と自動検出
  1. "DeployX.exe" を開きます。最初はサイドバーのボタンがグレーアウト（無効）
     されていますが、これは安全のための正常な動作です。
  2. USB ケーブルでスマートフォンを PC に接続します。
  3. スマートフォンの画面を確認します。「USB デバッグを許可しますか？」という
     プロンプトが表示されたら、「常に許可する」にチェックを入れて OK をタップします。
  4. DeployX がデバイスを数秒で自動検出します。

ステップ 3：安全な切断
  終了したらケーブルを抜くだけです。DeployX はシステムを保護するため、ボタンを即座にロックします。

--------------------------------------------------------------------------------
 3. 機能の詳細な説明（サイドバーメニュー）
--------------------------------------------------------------------------------
* [ デバイス ]: デバイスの技術的詳細（モデル、Android バージョン、バッテリー等）を表示。
* [ インストール ]: PC からスマートフォンへ .apk ファイルを直接インストール。
* [ アプリケーション ]: アプリのアンインストールやキャッシュ消去を行うパッケージマネージャー。
* [ エクスプローラー ]: 双方向ファイルマネージャー（Pull / Push 機能）。
* [ 画面 ]: デバイスのスクリーンショットを撮影して PC に保存。
* [ LOGCAT ]: Android システムのリアルタイムログを表示。アプリの診断に不可欠。
* [ モニター ]: RAM の消費量や CPU 使用率をリアルタイムで監視。

--------------------------------------------------------------------------------
 4. よくあるトラブルシューティング（FAQ）
--------------------------------------------------------------------------------
Q: デバイスを接続してもボタンがグレーのままです。
A: 主に以下の3つの原因が考えられます：
   1. USB デバッグが有効になっていない（最も一般的なエラー）。
   2. 権限がない。スマートフォンのロックを解除し、画面のプロンプトで許可してください。
   3. USB ケーブルがデータ転送に対応していない。

Q: プログラムを開いてもすぐにクラッシュします。
A: 重要なファイルが不足しています。"WebView2Loader.dll" が "DeployX.exe" と
   全く同じフォルダー内にあることを確認してください。

--------------------------------------------------------------------------------
クレジット:
開発者：Pablo Villavicencio
接続エンジン：Android Debug Bridge (ADB)
ウェブインターフェース：Microsoft Edge WebView2

 RU - РУССКИЙ (RUSSIAN)
Добро пожаловать в DeployX! 
DeployX — это мощный графический инструмент для Windows, предназначенный для 
взаимодействия с устройствами Android через ADB (Android Debug Bridge). Его цель — 
облегчить обслуживание, отладку и управление вашим телефоном или планшетом 
без необходимости ввода сложных команд в консоли.

--------------------------------------------------------------------------------
 1. ПРЕДВАРИТЕЛЬНЫЕ ТРЕБОВАНИЯ И ВАЖНЫЕ ПРЕДУПРЕЖДЕНИЯ
--------------------------------------------------------------------------------
Для правильной работы DeployX вам потребуется:

* Windows 10 или Windows 11.
* USB-драйверы для вашего телефона, установленные на ПК.
* USB-кабель для передачи данных (кабели «только для зарядки» не подойдут).
* ЦЕЛОСТНОСТЬ ПРОГРАММЫ: Данное программное обеспечение зависит от браузерного 
  движка (WebView2) и других библиотек. **НИКОГДА не извлекайте файл DeployX.exe 
  из его исходной папки**. Если вы отделите его от таких файлов, как 
  «WebView2Loader.dll» или папки «runtimes», программа завершится с ошибкой 
  и не будет работать.

--------------------------------------------------------------------------------
 2. ПОШАГОВОЕ РУКОВОДСТВО ПОЛЬЗОВАТЕЛЯ
--------------------------------------------------------------------------------
Шаг 1: Подготовка телефона (Отладка по USB)
Перед подключением телефона к компьютеру необходимо включить связь:
  1. Перейдите в Настройки > О телефоне на вашем Android.
  2. Нажмите 7 раз подряд на «Номер сборки», чтобы включить Параметры разработчика.
  3. Вернитесь назад, войдите в «Параметры разработчика» и включите «Отладка по USB».

Шаг 2: Подключение и автоматическое обнаружение
  1. Откройте «DeployX.exe». Вы увидите экран приветствия. Изначально кнопки 
     бокового меню будут неактивны (серого цвета). Это мера безопасности.
  2. Подключите телефон к ПК с помощью USB-кабеля.
  3. Проверьте экран телефона: появится запрос «Разрешить отладку по USB?». 
     Установите флажок «Всегда разрешать» и нажмите ОК.
  4. DeployX автоматически обнаружит ваше устройство за несколько секунд.

Шаг 3: Безопасное отключение
  По завершении просто отсоедините кабель. DeployX мгновенно заблокирует кнопки.

--------------------------------------------------------------------------------
 3. ПОДРОБНОЕ ОПИСАНИЕ ФУНКЦИЙ (БОКОВОЕ МЕНЮ)
--------------------------------------------------------------------------------
* [ УСТРОЙСТВО ]: Главная панель (модель, версия Android, заряд батареи).
* [ УСТАНОВИТЬ ]: Установка приложений (.apk) с ПК на телефон.
* [ ПРИЛОЖЕНИЯ ]: Диспетчер пакетов для удаления приложений или очистки кэша.
* [ ПРОВОДНИК ]: Двусторонний файловый менеджер (извлечение/отправка файлов).
* [ ЭКРАН ]: Скриншоты экрана вашего телефона с сохранением на ПК.
* [ LOGCAT ]: Показывает журнал системы Android в реальном времени.
* [ МОНИТОР ]: Мониторинг потребления ОЗУ и загрузки ЦП.

--------------------------------------------------------------------------------
 4. ЧАСТО ЗАДАВАЕМЫЕ ВОПРОСЫ (FAQ)
--------------------------------------------------------------------------------
В: Я подключаю телефон, но кнопки DeployX остаются серыми.
О: Это происходит по трем основным причинам:
   1. ОТЛАДКА ПО USB НЕ ВКЛЮЧЕНА. Это самая частая ошибка.
   2. Отсутствие разрешений. Разблокируйте телефон и примите запрос ADB.
   3. Ваш USB-кабель не поддерживает передачу данных.

В: Программа открывается, но почти сразу закрывается.
О: Отсутствуют жизненно важные файлы. Убедитесь, что файл «WebView2Loader.dll» 
   находится в той же папке, что и «DeployX.exe».

--------------------------------------------------------------------------------
Авторы:
Разработчик: Pablo Villavicencio
Движок подключения: Android Debug Bridge (ADB)
Веб-интерфейс: Microsoft Edge WebView2
