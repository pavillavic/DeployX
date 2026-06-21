# 📱 DeployX
**Advanced graphical tool for Windows to interact with Android devices via ADB.**

---

## 🇺🇸 [EN] ENGLISH

Welcome to DeployX!
DeployX is a powerful graphical tool for Windows designed to interact with Android devices via ADB (Android Debug Bridge). Its goal is to make maintaining, debugging, and managing your phone or tablet easier without needing to type complex console commands.

<img width="786" height="682" alt="1" src="https://github.com/user-attachments/assets/21a5446b-2057-488b-a4ef-aa537753bb95" />
<img width="786" height="682" alt="2" src="https://github.com/user-attachments/assets/78d584e8-b6a8-41a4-a6cf-8873dcfcc6cd" />
<img width="786" height="682" alt="3" src="https://github.com/user-attachments/assets/fa65b012-1a7d-48f1-8cc4-4ee5dd11a751" />
<img width="786" height="682" alt="4" src="https://github.com/user-attachments/assets/9e3dd1c7-3f55-48ff-be60-f05f1fa75efd" />
<img width="786" height="682" alt="5" src="https://github.com/user-attachments/assets/f68e4c9d-e05f-4bc5-a221-5d40cc535f75" />
<img width="787" height="686" alt="6" src="https://github.com/user-attachments/assets/59f2bb01-b5c0-446c-bc4d-1e97b5d7e2be" />
<img width="786" height="682" alt="7" src="https://github.com/user-attachments/assets/cccb6f7a-3c3f-4ed9-8285-cbf1994abd2b" />
<img width="787" height="682" alt="8" src="https://github.com/user-attachments/assets/ad786cbe-ca73-420a-96e0-61c1d77eae10" />
<img width="786" height="682" alt="9" src="https://github.com/user-attachments/assets/8fb91ac2-1990-47f6-b204-03d5fd5cfd1c" />

### 1. PREREQUISITES AND IMPORTANT WARNINGS
For DeployX to work properly, you need the following:

* Windows 10 or Windows 11.
* USB drivers for your phone installed on your PC (if Windows doesn't detect it).
* A data transfer USB cable (cables that are "charge-only" will not work).
* PROGRAM INTEGRITY: This software depends on a browser engine (WebView2) and other libraries. **NEVER take the `DeployX.exe` file out of its original folder**. If you separate it from files like `WebView2Loader.dll` or the `runtimes` folder, the program will crash and will not work.

### 2. STEP-BY-STEP USER MANUAL

**Step 1: Prepare the phone (Developer Options)**
Before connecting the phone to the computer, you must enable communication:
1. Go to Settings > About phone on your Android.
2. Tap "Build number" 7 consecutive times to enable Developer Options.
3. Go back, enter "Developer Options" and turn on "USB Debugging".

**Step 2: USB Connection (Wired)**
1. Open `DeployX.exe`. You will see the welcome screen. Initially, the sidebar buttons will be grayed out (disabled). This is normal and is a security measure.
2. Connect your phone to the PC using the USB cable.
3. Check your phone's screen: a prompt will ask "Allow USB debugging from this computer?". Check the "Always allow" box and tap OK.
4. Magic! DeployX will automatically detect your device in seconds, and the menu buttons will light up indicating you are connected.

**Step 3: Wireless Debugging Connection (Wi-Fi)**
1. Ensure your PC and phone are connected to the same Wi-Fi network.
2. In Developer Options, turn on "Wireless debugging" and tap on it to see your IP address and Port (e.g., `192.168.1.70:37413`).
3. In DeployX, click on **[ WIRELESS DEBUGGING ]**, enter the exact IP and Port, and press Connect.

**Step 4: Safe Disconnection**
When you are done using the program, simply unplug the cable or click **[ DISCONNECT ]**. DeployX will notice instantly and lock the buttons again to protect the system.

### 3. DETAILED FUNCTION DESCRIPTION (SIDEBAR MENU)
* **[ SHOW DEVICES ]:** Checks and refreshes the list of connected devices via USB or Wi-Fi.
* **[ WIRELESS DEBUGGING ]:** Connect to your device over Wi-Fi using its IP address and port.
* **[ DEVICE INFO ]:** The main information panel. View essential technical details of your connected device (model, Android version, battery level, etc.).
* **[ APP STORES ]:** Quick access to alternative web stores (APKPure, F-Droid, etc.) to download apps directly.
* **[ INSTALL APK/XAPK ]:** The sideloading manager. Install applications directly from your PC to the phone silently.
* **[ APPS LIST ]:** A complete package manager. View installed apps, uninstall them (including bloatware), or clear their data/cache.
* **[ EXPLORER ]:** A two-way file manager. Easily extract files from your phone to your PC (Pull) or send them to your phone (Push) visually.
* **[ VIEW SCREEN ]:** Advanced screen mirroring and recording (powered by scrcpy). Cast your device with audio routing, use it as a PC webcam, create virtual displays, or record the screen in high quality (H.265/FPS controls).
* **[ LOGCAT ]:** Shows a real-time log of everything happening inside the Android system. Essential for developers or diagnosing crashing apps.
* **[ TASK MONITOR ]:** Live performance tool. Monitor RAM consumption and CPU usage in real-time. **Includes the new Advanced Device Report for deep forensic diagnostics and data extraction.**
* **[ ADB VERSION ]:** Checks the current version of the Android Debug Bridge engine running.
* **[ ANDROID CONSOLE ]:** Opens a native command prompt ready to receive direct ADB shell commands.
* **[ DISCONNECT ]:** Safely terminates the ADB server and disconnects all devices.

### 4. COMMON TROUBLESHOOTING (FAQ)
**Q: I connect the phone but the DeployX buttons are still gray (disabled).**
A: This happens for three main reasons:
1. **USB DEBUGGING IS NOT ENABLED.** This is the most common error. Go to your phone settings, enter "Developer Options", and turn on "USB Debugging".
2. **Missing permissions.** Unlock your phone and check the screen; a prompt will ask "Allow USB debugging?". Check "Always allow" and tap OK.
3. **Your USB cable does not support data.** Cheap cables are often charge-only. Try using the original cable or one confirmed to transfer data.

**Q: The program opens, but crashes almost immediately or throws a fatal error.**
A: You are missing vital files. Ensure the `WebView2Loader.dll` file is in the exact same folder as `DeployX.exe`.

**Q: I try to install an APK but get an error.**
A: Check that you have enough storage space and that a newer version of the app isn't already installed.

### CHANGELOG (v1.0.2)
* **New features:** Added the "Advanced Device Report", a powerful forensic diagnostic tool.
* **Mega-extraction:** Deep system parameters are now extracted (base hardware, battery wear, processor, live network, users, security policies, and sensors).
* **Accounts & Privacy:** Complete and detailed detection of emails and linked accounts.
* **Interface:** Interactive floating windows (ToolTips) integrated into the table to explain each parameter in detail. Added a subtle version tag (v1.0.2) below the language selector.
* **Export:** Added the option to export the complete diagnostic to a text file (`.txt`).

### CHANGELOG (v1.0.1)
* **New features:** Added "High Quality (H.265)" mode and FPS selector (30, 24, 15) for screen mirroring/recording with scrcpy.
* **Bug fixes:** Resolved an issue where screen recordings were not saving to the selected path.
* **Critical patches:** Fixed a bug causing the internal browser (WebView2) to display a blank screen when opening app stores in the installed version.

**Credits & Acknowledgements:**
* **DeployX Developed by:** Pablo Villavicencio
* **ADB (Android Debug Bridge):** Google / Android Open Source Project
* **Screen Mirroring Engine (scrcpy):** Genymobile
* **Web Interface:** Microsoft Edge WebView2

---

## 🇲🇽 [ES] ESPAÑOL

¡Bienvenido a DeployX!
DeployX es una potente herramienta gráfica para Windows diseñada para interactuar con dispositivos Android a través de ADB (Android Debug Bridge). Su objetivo es facilitar el mantenimiento, la depuración y la gestión de tu teléfono o tablet sin necesidad de escribir complicados comandos en la consola.

### 1. REQUISITOS PREVIOS Y ADVERTENCIAS IMPORTANTES
Para que DeployX funcione correctamente, necesitas cumplir con lo siguiente:

* Windows 10 o Windows 11.
* Drivers USB de tu teléfono instalados en la PC (si Windows no lo reconoce por defecto).
* Un cable USB de transferencia de datos (los cables que son "solo para carga" no funcionarán).
* INTEGRIDAD DEL PROGRAMA: Este programa depende de un motor de navegación (WebView2) y otras librerías. **NUNCA saques el archivo `DeployX.exe` de su carpeta original**. Si lo separas de archivos como `WebView2Loader.dll` o la carpeta `runtimes`, el programa se cerrará de golpe y no funcionará.

### 2. MANUAL DE USO PASO A PASO

**Paso 1: Preparar el teléfono (Opciones de Desarrollador)**
Antes de conectar el teléfono a la computadora, debes habilitar la comunicación:
1. Ve a Configuración > Acerca del teléfono en tu Android.
2. Toca 7 veces seguidas donde dice "Número de compilación" para activar las Opciones de Desarrollador.
3. Regresa, entra a las "Opciones de Desarrollador" y activa "Depuración USB".

**Paso 2: Conexión por USB (Cable)**
1. Abre `DeployX.exe`. Verás la pantalla de bienvenida. Inicialmente, notarás que los botones del menú lateral están desactivados (en gris). Esto es completamente normal y es una medida de seguridad.
2. Conecta tu teléfono a la PC con el cable USB.
3. Revisa la pantalla de tu teléfono: te aparecerá un aviso preguntando "¿Permitir depuración USB desde esta computadora?". Marca la casilla "Permitir siempre" y dale en Aceptar.
4. ¡Magia! DeployX detectará tu dispositivo automáticamente en cuestión de segundos y los botones del menú cobrarán vida indicando que estás conectado.

**Paso 3: Conexión Inalámbrica (Wi-Fi)**
1. Asegúrate de que tu PC y teléfono estén en la misma red Wi-Fi.
2. En las Opciones de Desarrollador, activa "Depuración inalámbrica" y tócalo para ver tu dirección IP y Puerto (ej. `192.168.1.70:37413`).
3. En DeployX, haz clic en **[ DEPURACIÓN INALÁMBRICA ]**, ingresa la IP y el Puerto exactos, y presiona Conectar.

**Paso 4: Desconexión Segura**
Cuando termines de usar el programa, simplemente desconecta el cable o haz clic en **[ DESCONECTAR ]**. DeployX se dará cuenta al instante y volverá a bloquear los botones para proteger el sistema.

### 3. DESCRIPCIÓN DETALLADA DE LAS FUNCIONES (MENÚ LATERAL)
* **[ VER DISPOSITIVOS ]:** Comprueba y actualiza la lista de equipos conectados por USB o Wi-Fi.
* **[ DEPURACIÓN INALÁMBRICA ]:** Conecta tu dispositivo por Wi-Fi usando su dirección IP y puerto.
* **[ INFO DISPOSITIVO ]:** El panel principal de información. Aquí podrás ver los detalles técnicos esenciales de tu equipo (modelo, versión de Android, batería, etc.).
* **[ TIENDAS DE APPS ]:** Acceso rápido a tiendas web alternativas (APKPure, F-Droid, etc.) para descargar apps directamente.
* **[ INSTALAR APK/XAPK ]:** El gestor de sideloading. Te permite instalar aplicaciones directamente desde tu PC al teléfono de forma silenciosa.
* **[ LISTA DE APPS ]:** Un administrador de paquetes completo. Puedes ver apps instaladas, desinstalarlas (incluso bloatware) o limpiar sus datos/caché.
* **[ EXPLORADOR ]:** Un gestor de archivos bidireccional. Te permite extraer archivos del teléfono a tu PC (Pull) o enviarlos al teléfono (Push) visualmente.
* **[ VER PANTALLA ]:** Transmisión y grabación avanzada de pantalla (con scrcpy). Duplica tu dispositivo con desvío de audio, úsalo como webcam en la PC, crea pantallas virtuales o graba en alta calidad (H.265/FPS ajustables).
* **[ LOGCAT ]:** Muestra un registro en tiempo real de todo lo que ocurre en el sistema Android. Indispensable para desarrolladores o para diagnosticar apps que fallan.
* **[ MONITOR DE TAREAS ]:** Herramienta para vigilar el consumo de memoria RAM y el uso de CPU del teléfono en tiempo real. **Incluye el nuevo Reporte Avanzado del Dispositivo para diagnósticos forenses y extracción profunda de datos.**
* **[ VERSIÓN ADB ]:** Comprueba la versión actual del motor Android Debug Bridge en ejecución.
* **[ CONSOLA ANDROID ]:** Abre una ventana de comandos nativa lista para recibir comandos ADB directos.
* **[ DESCONECTAR ]:** Termina de forma segura el servidor ADB y desconecta todos los equipos.

### 4. SOLUCIÓN DE PROBLEMAS COMUNES (FAQ)
**P: Conecto el celular pero los botones de DeployX siguen en gris (desactivados).**
R: Esto pasa por tres razones principales:
1. **NO TIENES LA DEPURACIÓN USB ACTIVADA.** Este es el error más común. Ve a la configuración de tu teléfono, entra a "Opciones de Desarrollador" y asegúrate de encender la "Depuración USB".
2. **Falta dar permisos en el teléfono.** Revisa la pantalla de tu celular desbloqueado; te aparecerá un aviso preguntando "¿Permitir depuración USB?", marca "Permitir siempre" y dale en Aceptar.
3. **Tu cable USB no soporta datos.** Muchos cables baratos son solo para cargar batería. Intenta con el cable original o uno que confirme transferencia de datos.

**P: El programa abre, pero se cierra casi inmediatamente o marca un error fatal.**
R: Te faltan archivos vitales. Asegúrate de que el archivo `WebView2Loader.dll` esté exactamente en la misma carpeta que `DeployX.exe`.

**P: Intento instalar un APK pero me da error.**
R: Verifica que tengas suficiente espacio de almacenamiento y que la aplicación no esté ya instalada con una versión más nueva.

### NOVEDADES EN v1.0.2
* **Nuevas funciones:** Se agregó el "Reporte Avanzado del Dispositivo", una potente herramienta de diagnóstico forense.
* **Mega-extracción de datos:** Ahora se extraen parámetros profundos (hardware base, desgaste de batería, procesador, red en vivo, usuarios, políticas de seguridad y sensores).
* **Cuentas y Privacidad:** Detección completa y detallada de correos electrónicos y cuentas vinculadas.
* **Interfaz:** Se integraron ventanas flotantes interactivas (ToolTips) en la tabla para explicar detalladamente cada parámetro. Se agregó un discreto indicador de versión (v1.0.2) debajo del selector de idioma.
* **Exportación:** Se añadió la opción para exportar el diagnóstico completo a un archivo de texto (`.txt`).

### NOVEDADES EN v1.0.1
* **Nuevas funciones:** Se agregó el modo "Alta Calidad (H.265)" y un selector de FPS (30, 24, 15) para la transmisión y grabación de pantalla con scrcpy.
* **Correcciones:** Se solucionó un problema donde las grabaciones de pantalla no se guardaban en la ruta elegida.
* **Parches críticos:** Se solucionó el error que dejaba en blanco el navegador interno (WebView2) al abrir las tiendas de aplicaciones en la versión instalada.

**Créditos y Agradecimientos:**
* **Desarrollado por:** Pablo Villavicencio
* **Motor de conexión (ADB):** Google / Android Open Source Project
* **Motor de transmisión de pantalla (scrcpy):** Genymobile
* **Interfaz Web:** Microsoft Edge WebView2

---

## 🇫🇷 [FR] FRANÇAIS

Bienvenue sur DeployX !
DeployX est un outil graphique puissant pour Windows conçu pour interagir avec les appareils Android via ADB (Android Debug Bridge). Son but est de faciliter la maintenance, le débogage et la gestion de votre téléphone ou tablette sans avoir besoin d'écrire des commandes de console complexes.

### 1. PRÉREQUIS ET AVERTISSEMENTS IMPORTANTS
Pour que DeployX fonctionne correctement, vous avez besoin de ce qui suit :

* Windows 10 ou Windows 11.
* Les pilotes (drivers) USB de votre téléphone installés sur le PC.
* Un câble USB de transfert de données (les câbles "charge uniquement" ne fonctionneront pas).
* INTÉGRITÉ DU PROGRAMME : Ce logiciel dépend d'un moteur de navigation (WebView2) et d'autres bibliothèques. **NE SORTEZ JAMAIS le fichier `DeployX.exe` de son dossier d'origine**. Si vous le séparez de fichiers tels que `WebView2Loader.dll` ou du dossier `runtimes`, le programme plantera et ne fonctionnera pas.

### 2. MANUEL D'UTILISATION ÉTAPE PAR ÉTAPE

**Étape 1 : Préparer le téléphone (Débogage USB)**
Avant de connecter le téléphone à l'ordinateur, vous devez activer la communication :
1. Allez dans Paramètres > À propos du téléphone sur votre Android.
2. Appuyez 7 fois de suite sur "Numéro de build" pour activer les Options pour les développeurs.
3. Revenez en arrière, entrez dans "Options pour les développeurs" et activez le "Débogage USB".

**Étape 2 : Connexion USB (Filaire)**
1. Ouvrez `DeployX.exe`. Vous verrez l'écran de bienvenue. Initialement, les boutons du menu latéral seront grisés (désactivés). C'est une mesure de sécurité.
2. Connectez votre téléphone au PC avec le câble USB.
3. Vérifiez l'écran de votre téléphone : un message demandera "Autoriser le débogage USB ?". Cochez "Toujours autoriser" et appuyez sur OK.
4. Magie ! DeployX détectera automatiquement votre appareil en quelques secondes.

**Étape 3 : Connexion de Débogage Sans Fil (Wi-Fi)**
1. Assurez-vous que votre PC et votre téléphone sont sur le même réseau Wi-Fi.
2. Dans les Options pour les développeurs, activez le "Débogage sans fil" et appuyez dessus pour voir votre adresse IP et votre port (ex. `192.168.1.70:37413`).
3. Dans DeployX, cliquez sur **[ DÉBOGAGE SANS FIL ]**, entrez l'adresse IP et le port exacts, et appuyez sur Connecter.

**Étape 4 : Déconnexion Sécurisée**
Lorsque vous avez terminé, débranchez simplement le câble ou cliquez sur **[ DÉCONNECTER ]**. DeployX le remarquera instantanément et verrouillera les boutons pour protéger le système.

### 3. DESCRIPTION DÉTAILLÉE DES FONCTIONS (MENU LATÉRAL)
* **[ VOIR LES APPAREILS ] :** Vérifie et actualise la liste des appareils connectés via USB ou Wi-Fi.
* **[ DÉBOGAGE SANS FIL ] :** Connectez votre appareil via Wi-Fi en utilisant son adresse IP et son port.
* **[ INFO APPAREIL ] :** Panneau d'informations principal (modèle, version Android, batterie).
* **[ BOUTIQUES D'APPLICATIONS ] :** Accès rapide aux boutiques Web alternatives (APKPure, F-Droid, etc.) pour télécharger des applications directement.
* **[ INSTALLER APK/XAPK ] :** Gestionnaire d'installation (sideloading) d'applications directement depuis votre PC.
* **[ LISTE D'APPLICATIONS ] :** Gestionnaire de paquets pour désinstaller ou effacer le cache.
* **[ EXPLORATEUR ] :** Gestionnaire de fichiers bidirectionnel (Pull/Push).
* **[ VOIR L'ÉCRAN ] :** Mise en miroir et enregistrement d'écran avancés (via scrcpy). Diffusez votre appareil avec routage audio, utilisez-le comme webcam PC, créez des écrans virtuels ou enregistrez en haute qualité (H.265/FPS ajustables).
* **[ LOGCAT ] :** Affiche un journal en temps réel du système Android.
* **[ MONITEUR DES TÂCHES ] :** Outil de surveillance en direct de la RAM et du CPU. **Inclut le nouveau Rapport Avancé de l'Appareil pour des diagnostics médico-légaux et une extraction approfondie des données.**
* **[ VERSION ADB ] :** Vérifie la version actuelle du moteur Android Debug Bridge en cours d'exécution.
* **[ CONSOLE ANDROID ] :** Ouvre une invite de commande native prête à recevoir des commandes ADB directes.
* **[ DÉCONNECTER ] :** Termine le serveur ADB en toute sécurité et déconnecte tous les appareils.

### 4. DÉPANNAGE COURANT (FAQ)
**Q : Je connecte le téléphone mais les boutons DeployX restent gris.**
R : Cela se produit pour trois raisons principales :
1. **LE DÉBOGAGE USB N'EST PAS ACTIVÉ.** C'est l'erreur la plus courante.
2. **Autorisations manquantes.** Déverrouillez votre téléphone et acceptez l'invite ADB.
3. **Votre câble USB ne prend pas en charge les données.** Essayez un autre câble.

**Q : Le programme s'ouvre mais se ferme presque immédiatement.**
R : Il vous manque des fichiers vitaux. Assurez-vous que le fichier `WebView2Loader.dll` se trouve dans le même dossier que `DeployX.exe`.

### NOUVEAUTÉS DE LA v1.0.2
* **Nouvelles fonctionnalités :** Ajout du "Rapport avancé de l'appareil", un puissant outil de diagnostic médico-légal.
* **Méga-extraction :** Extraction approfondie des paramètres du système (matériel de base, usure de la batterie, processeur, réseau en direct, utilisateurs, politiques de sécurité et capteurs).
* **Comptes et confidentialité :** Détection complète et détaillée des e-mails et comptes associés.
* **Interface :** Fenêtres flottantes interactives (ToolTips) intégrées au tableau pour expliquer chaque paramètre en détail. Ajout d'une étiquette de version subtile (v1.0.2).
* **Exportation :** Ajout de l'option permettant d'exporter le diagnostic complet vers un fichier texte (`.txt`).

### NOUVEAUTÉS DE LA v1.0.1
* **Nouvelles fonctionnalités :** Ajout du mode "Haute Qualité (H.265)" et d'un sélecteur de FPS (30, 24, 15) pour la mise en miroir/enregistrement d'écran avec scrcpy.
* **Corrections :** Résolution d'un problème où les enregistrements d'écran n'étaient pas sauvegardés dans le chemin sélectionné.
* **Correctif critique :** Correction d'un bug provoquant l'affichage d'un écran blanc par le navigateur interne (WebView2) lors de l'ouverture des magasins d'applications dans la version installée.

**Crédits et Remerciements :**
* **Développé par :** Pablo Villavicencio
* **Moteur de connexion (ADB) :** Google / Android Open Source Project
* **Moteur de mise en miroir (scrcpy) :** Genymobile
* **Interface Web :** Microsoft Edge WebView2

---

## 🇩🇪 [DE] DEUTSCH

Willkommen bei DeployX!
DeployX ist ein leistungsstarkes grafisches Tool für Windows, das für die Interaktion mit Android-Geräten über ADB (Android Debug Bridge) entwickelt wurde. Es erleichtert die Wartung und Verwaltung Ihres Telefons, ohne Konsolenbefehle eingeben zu müssen.

### 1. VORAUSSETZUNGEN UND WICHTIGE WARNHINWEISE
Damit DeployX funktioniert, benötigen Sie:

* Windows 10 oder Windows 11.
* Installierte USB-Treiber für Ihr Telefon.
* Ein USB-Datenkabel (reine Ladekabel funktionieren nicht).
* PROGRAMMINTEGRITÄT: Diese Software ist von einer Browser-Engine (WebView2) abhängig. **ENTFERNEN SIE NIEMALS die Datei `DeployX.exe` aus ihrem ursprünglichen Ordner**. Wenn Sie sie von `WebView2Loader.dll` oder dem `runtimes`-Ordner trennen, stürzt das Programm ab.

### 2. SCHRITT-FÜR-SCHRITT BEDIENUNGSANLEITUNG

**Schritt 1: Telefon vorbereiten (USB-Debugging)**
1. Gehen Sie auf Ihrem Android zu Einstellungen > Über das Telefon.
2. Tippen Sie 7 Mal auf "Build-Nummer", um die Entwickleroptionen zu aktivieren.
3. Gehen Sie zurück zu den Entwickleroptionen und aktivieren Sie "USB-Debugging".

**Schritt 2: USB-Verbindung (Kabelgebunden)**
1. Öffnen Sie `DeployX.exe`. Die Menüschaltflächen sind zunächst aus Sicherheitsgründen deaktiviert (grau).
2. Verbinden Sie Ihr Telefon über das USB-Kabel mit dem PC.
3. Auf dem Bildschirm Ihres Telefons erscheint die Meldung "USB-Debugging zulassen?". Setzen Sie ein Häkchen bei "Immer zulassen" und tippen Sie auf OK.
4. DeployX erkennt Ihr Gerät automatisch.

**Schritt 3: Kabellose Debugging-Verbindung (WLAN)**
1. Stellen Sie sicher, dass sich PC und Telefon im selben WLAN-Netzwerk befinden.
2. Aktivieren Sie in den Entwickleroptionen das "Kabelloses Debugging" und tippen Sie darauf, um Ihre IP-Adresse und den Port anzuzeigen (z. B. `192.168.1.70:37413`).
3. Klicken Sie in DeployX auf **[ KABELLOSES DEBUGGING ]**, geben Sie die genaue IP und den Port ein und drücken Sie auf Verbinden.

**Schritt 4: Sichere Trennung**
Trennen Sie einfach das Kabel oder klicken Sie auf **[ TRENNEN ]**. DeployX sperrt die Tasten automatisch wieder.

### 3. DETAILLIERTE FUNKTIONSBESCHREIBUNG (SEITENMENÜ)
* **[ GERÄTE ANZEIGEN ]:** Überprüft und aktualisiert die Liste der über USB oder WLAN verbundenen Geräte.
* **[ KABELLOSES DEBUGGING ]:** Verbinden Sie Ihr Gerät über WLAN mit seiner IP-Adresse und seinem Port.
* **[ GERÄTEINFO ]:** Hauptinformationsbereich (Modell, Android-Version, Akku).
* **[ APP-STORES ]:** Schneller Zugriff auf alternative Web-Stores (APKPure, F-Droid usw.), um Apps direkt herunterzuladen.
* **[ APK/XAPK INSTALLIEREN ]:** Sideloading-Manager zum direkten Installieren von Dateien.
* **[ APP-LISTE ]:** Paketmanager zum Deinstallieren von Apps oder Löschen des Caches.
* **[ EXPLORER ]:** Dateimanager zum Extrahieren (Pull) oder Senden (Push) von Dateien.
* **[ BILDSCHIRM ANZEIGEN ]:** Erweiterte Bildschirmspiegelung und -aufzeichnung (über scrcpy). Übertragen Sie Ihr Gerät mit Audio-Routing, nutzen Sie es als PC-Webcam, erstellen Sie virtuelle Displays oder nehmen Sie in hoher Qualität auf (H.265/FPS anpassbar).
* **[ LOGCAT ]:** Zeigt das Echtzeitprotokoll des Android-Systems an.
* **[ TASK-MONITOR ]:** Echtzeit-Überwachung von RAM- und CPU-Auslastung. **Enthält den neuen Erweiterten Gerätebericht für forensische Diagnosen und tiefe Datenextraktion.**
* **[ ADB-VERSION ]:** Überprüft die aktuelle Version der ausgeführten Android Debug Bridge-Engine.
* **[ ANDROID-KONSOLE ]:** Öffnet eine native Eingabeaufforderung, die bereit ist, direkte ADB-Shell-Befehle zu empfangen.
* **[ TRENNEN ]:** Beendet den ADB-Server sicher und trennt alle Geräte.

### 4. HÄUFIGE PROBLEMLÖSUNGEN (FAQ)
**F: Ich schließe das Telefon an, aber die Tasten bleiben grau.**
A: Dafür gibt es drei Hauptgründe:
1. **USB-DEBUGGING IST NICHT AKTIVIERT.** Dies ist der häufigste Fehler.
2. **Fehlende Berechtigungen.** Entsperren Sie das Telefon und akzeptieren Sie ADB.
3. **Das USB-Kabel unterstützt keine Datenübertragung.**

**F: Das Programm schließt sich sofort nach dem Öffnen.**
A: Stellen Sie sicher, dass sich `WebView2Loader.dll` im selben Ordner wie `DeployX.exe` befindet.

### NEUERUNGEN IN v1.0.2
* **Neue Funktionen:** "Erweiterter Gerätebericht" hinzugefügt, ein leistungsstarkes forensisches Diagnosetool.
* **Mega-Extraktion:** Tiefe Systemparameter werden nun extrahiert (Basishardware, Akkuverschleiß, Prozessor, Live-Netzwerk, Benutzer, Sicherheitsrichtlinien und Sensoren).
* **Konten & Privatsphäre:** Vollständige und detaillierte Erkennung von E-Mails und verknüpften Konten.
* **Schnittstelle:** Interaktive schwebende Fenster (ToolTips) in die Tabelle integriert, um jeden Parameter im Detail zu erklären. Subtiles Versions-Tag (v1.0.2) hinzugefügt.
* **Export:** Option hinzugefügt, um die gesamte Diagnose in eine Textdatei (`.txt`) zu exportieren.

### NEUERUNGEN IN v1.0.1
* **Neue Funktionen:** "Hohe Qualität (H.265)"-Modus und FPS-Wahlschalter (30, 24, 15) für Bildschirmspiegelung/Aufnahme mit scrcpy hinzugefügt.
* **Fehlerbehebungen:** Ein Problem wurde behoben, bei dem Bildschirmaufnahmen nicht im ausgewählten Pfad gespeichert wurden.
* **Kritischer Patch:** Ein Fehler wurde behoben, der dazu führte, dass der interne Browser (WebView2) beim Öffnen von App-Stores in der installierten Version einen weißen Bildschirm anzeigte.

**Credits & Danksagungen:**
* **Entwickelt von:** Pablo Villavicencio
* **Verbindungs-Engine (ADB):** Google / Android Open Source Project
* **Bildschirmspiegelungs-Engine (scrcpy):** Genymobile
* **Web-Oberfläche:** Microsoft Edge WebView2

---

## 🇧🇷 [PT] PORTUGUÊS

Bem-vindo ao DeployX!
DeployX é uma poderosa ferramenta gráfica para Windows projetada para interagir com dispositivos Android via ADB (Android Debug Bridge). Seu objetivo é facilitar a manutenção, depuração e gerenciamento do seu telefone ou tablet sem precisar digitar comandos complexos.

### 1. PRÉ-REQUISITOS E AVISOS IMPORTANTES
Para que o DeployX funcione corretamente, você precisa de:

* Windows 10 ou Windows 11.
* Drivers USB do seu telefone instalados no PC.
* Um cabo USB de transferência de dados (cabos apenas para carga não funcionarão).
* INTEGRIDADE DO PROGRAMA: Este software depende de um motor de navegador (WebView2) e outras bibliotecas. **NUNCA tire o arquivo `DeployX.exe` de sua pasta original**. Se você separá-lo de arquivos como `WebView2Loader.dll` ou da pasta `runtimes`, o programa não funcionará.

### 2. MANUAL DO USUÁRIO PASSO A PASSO

**Passo 1: Preparar o telefone (Depuração USB)**
1. Vá para Configurações > Sobre o telefone no seu Android.
2. Toque 7 vezes seguidas no "Número da versão" para ativar as Opções do Desenvolvedor.
3. Volte, entre em "Opções do Desenvolvedor" e ative a "Depuração USB".

**Passo 2: Conexão USB (Com fio)**
1. Abra `DeployX.exe`. Inicialmente, os botões estarão desativados (cinza). Isso é uma medida de segurança.
2. Conecte seu telefone ao PC com o cabo USB.
3. Verifique a tela do seu telefone: um aviso perguntará "Permitir depuração USB?". Marque "Sempre permitir" e toque em OK.
4. O DeployX detectará automaticamente seu dispositivo em segundos.

**Passo 3: Conexão de Depuração Sem Fio (Wi-Fi)**
1. Certifique-se de que seu PC e telefone estejam na mesma rede Wi-Fi.
2. Nas Opções do Desenvolvedor, ative a "Depuração sem fio" e toque nela para ver seu endereço IP e Porta (ex: `192.168.1.70:37413`).
3. No DeployX, clique em **[ DEPURAÇÃO SEM FIO ]**, digite o IP e a Porta exatos e pressione Conectar.

**Passo 4: Desconexão Segura**
Ao terminar, basta desconectar o cabo ou clicar em **[ DESCONECTAR ]**. O DeployX bloqueará os botões instantaneamente.

### 3. DESCRIÇÃO DETALHADA DAS FUNÇÕES (MENU LATERAL)
* **[ VER DISPOSITIVOS ]:** Verifica e atualiza a lista de dispositivos conectados via USB ou Wi-Fi.
* **[ DEPURAÇÃO SEM FIO ]:** Conecte seu dispositivo por Wi-Fi usando seu endereço IP e porta.
* **[ INFO DISPOSITIVO ]:** Painel principal de informações (modelo, versão do Android, bateria).
* **[ LOJAS DE APPS ]:** Acesso rápido a lojas web alternativas (APKPure, F-Droid, etc.) para baixar apps diretamente.
* **[ INSTALAR APK/XAPK ]:** Gerenciador de instalação (sideload) para aplicativos diretamente do PC.
* **[ LISTA DE APPS ]:** Gerenciador de pacotes para desinstalar apps ou limpar o cache.
* **[ EXPLORADOR ]:** Gerenciador de arquivos (Pull e Push).
* **[ VER TELA ]:** Espelhamento e gravação de tela avançados (via scrcpy). Transmita seu dispositivo com roteamento de áudio, use-o como webcam no PC, crie telas virtuais ou grave em alta qualidade (H.265/FPS ajustável).
* **[ LOGCAT ]:** Mostra o log em tempo real do sistema Android.
* **[ MONITOR DE TAREFAS ]:** Ferramenta de desempenho ao vivo (RAM e CPU). **Inclui o novo Relatório Avançado do Dispositivo para diagnósticos forenses e extração profunda de dados.**
* **[ VERSÃO ADB ]:** Verifica a versão atual do motor Android Debug Bridge em execução.
* **[ CONSOLE ANDROID ]:** Abre um prompt de comando nativo pronto para receber comandos ADB diretos.
* **[ DESCONECTAR ]:** Encerra com segurança o servidor ADB e desconecta todos os dispositivos.

### 4. SOLUÇÃO DE PROBLEMAS COMUNS (FAQ)
**P: Conecto o celular, mas os botões continuam cinza.**
R: Isso acontece por três motivos principais:
1. **A DEPURAÇÃO USB NÃO ESTÁ ATIVADA.** Este é o erro mais comum.
2. **Falta de permissões.** Desbloqueie a tela e aceite o aviso ADB.
3. **Seu cabo USB não suporta transferência de dados.**

**P: O programa abre, mas fecha quase imediatamente com um erro fatal.**
R: Faltam arquivos vitais. Certifique-se de que o arquivo `WebView2Loader.dll` esteja exatamente na mesma pasta que `DeployX.exe`.

### NOVIDADES NA v1.0.2
* **Novas funcionalidades:** Adicionado o "Relatório Avançado do Dispositivo", uma poderosa ferramenta de diagnóstico forense.
* **Mega-extração:** Extração profunda de parâmetros do sistema (hardware base, desgaste da bateria, processador, rede ao vivo, usuários, políticas de segurança e sensores).
* **Contas e Privacidade:** Detecção completa e detalhada de e-mails e contas vinculadas.
* **Interface:** Janelas flutuantes interativas (ToolTips) integradas à tabela para explicar cada parâmetro em detalhes. Adicionada uma tag de versão sutil (v1.0.2).
* **Exportação:** Adicionada a opção de exportar o diagnóstico completo para um arquivo de texto (`.txt`).

### NOVIDADES NA v1.0.1
* **Novas funcionalidades:** Adicionado o modo "Alta Qualidade (H.265)" e seletor de FPS (30, 24, 15) para espelhamento/gravação de tela com scrcpy.
* **Correções:** Resolvido um problema onde as gravações de tela não eram salvas no caminho selecionado.
* **Patch crítico:** Corrigido um bug que fazia o navegador interno (WebView2) exibir uma tela em branco ao abrir lojas de aplicativos na versão instalada.

**Créditos e Agradecimentos:**
* **Desenvolvido por:** Pablo Villavicencio
* **Motor de conexão (ADB):** Google / Android Open Source Project
* **Motor de espelhamento (scrcpy):** Genymobile
* **Interface Web:** Microsoft Edge WebView2

---

## 🇨🇳 [ZH] 中文 (CHINESE)

欢迎使用 DeployX！
DeployX 是一款功能强大的 Windows 图形化工具，旨在通过 ADB (Android Debug Bridge) 与 Android 设备进行交互。它的目标是简化设备的维护、调试和管理，让您无需在控制台中输入复杂的命令。

### 1. 先决条件和重要警告
为了让 DeployX 正常工作，您需要满足以下条件：

* Windows 10 或 Windows 11。
* 电脑上已安装您手机的 USB 驱动程序。
* 支持数据传输的 USB 数据线（"仅充电"的数据线无效）。
* 程序完整性：本软件依赖于浏览器引擎 (WebView2) 及其他组件。**切勿将 `DeployX.exe` 文件移出其原始文件夹**。如果您将其与 `WebView2Loader.dll` 或 `runtimes` 文件夹分开，程序将会崩溃且无法运行。

### 2. 分步使用手册

**第 1 步：准备手机（USB 调试）**
在将手机连接到电脑之前，必须开启通信功能：
1. 在 Android 手机上进入"设置" > "关于手机"。
2. 连续点击"版本号" 7 次，以启用"开发者选项"。
3. 返回上一页，进入"开发者选项"，并开启"USB 调试"。

**第 2 步：USB 连接（有线）**
1. 打开 `DeployX.exe`。起初，侧边栏按钮将显示为灰色（禁用）。这属于正常现象，也是一种安全机制。
2. 使用 USB 数据线将手机连接到电脑。
3. 查看手机屏幕：会弹出一个提示，询问"是否允许 USB 调试？"。勾选"始终允许"并点击确定。
4. DeployX 会在几秒钟内自动检测到您的设备。

**第 3 步：无线调试连接 (Wi-Fi)**
1. 确保您的电脑和手机连接到同一个 Wi-Fi 网络。
2. 在"开发者选项"中，开启"无线调试"并点击它以查看您的 IP 地址和端口（例如：`192.168.1.70:37413`）。
3. 在 DeployX 中，点击 **[ 无线调试 ]**，输入准确的 IP 和端口，然后点击连接。

**第 4 步：安全断开连接**
使用完毕后，只需拔下数据线或点击 **[ 断开连接 ]**。DeployX 会立即锁定按钮以保护系统。

### 3. 功能详细说明（侧边栏菜单）
* **[ 显示设备 ]：** 检查并刷新通过 USB 或 Wi-Fi 连接的设备列表。
* **[ 无线调试 ]：** 使用 IP 地址和端口通过 Wi-Fi 连接您的设备。
* **[ 设备信息 ]：** 主要信息面板。查看设备的型号、Android 版本、电池等。
* **[ 应用商店 ]：** 快速访问第三方网页商店（APKPure、F-Droid 等）以直接下载应用。
* **[ 安装 APK/XAPK ]：** 应用安装管理器。将文件从电脑直接静默安装到手机。
* **[ 应用程序列表 ]：** 完整的包管理器。可卸载应用程序或清除缓存。
* **[ 资源管理器 ]：** 双向文件管理器。方便地在电脑和手机之间提取 (Pull) 或发送 (Push) 文件。
* **[ 查看屏幕 ]：** 高级屏幕镜像与录制（基于 scrcpy）。支持音频路由投屏、作为电脑网络摄像头使用、创建虚拟显示器，或进行高质量录屏（支持 H.265 和 FPS 控制）。
* **[ LOGCAT ]：** 实时显示 Android 系统的日志，用于应用诊断。
* **[ 任务监控 ]：** 实时监控 RAM 和 CPU 使用情况。**包含全新的“高级设备报告”，用于深度取证诊断和数据提取。**
* **[ ADB 版本 ]：** 检查当前运行的 Android Debug Bridge 引擎版本。
* **[ ANDROID 控制台 ]：** 打开原生的命令提示符，准备接收直接的 ADB shell 命令。
* **[ 断开连接 ]：** 安全地终止 ADB 服务器并断开所有设备的连接。

### 4. 常见问题解答 (FAQ)
**问：我连接了手机，但 DeployX 的按钮依然是灰色的。**
答：这主要有三个原因：
1. **未开启 USB 调试。** 这是最常见的错误。
2. **缺少权限。** 请解锁手机并接受屏幕上的 ADB 授权提示。
3. **USB 数据线不支持数据传输。**

**问：程序打开后几乎立即闪退。**
答：缺少关键文件。请确保 `WebView2Loader.dll` 与 `DeployX.exe` 位于同一个文件夹中。

### 更新日志 (v1.0.2)
* **新功能：** 添加了“高级设备报告”，这是一款强大的取证诊断工具。
* **超级提取：** 现在可以提取深度系统参数（基础硬件、电池损耗、处理器、实时网络、用户、安全策略和传感器）。
* **帐户和隐私：** 全面详细地检测电子邮件和关联帐户。
* **界面：** 在表格中集成了交互式悬浮窗 (ToolTips)，详细解释每个参数。在语言选择器下方添加了版本标签 (v1.0.2)。
* **导出：** 添加了将完整诊断结果导出为文本文件 (`.txt`) 的选项。

### 更新日志 (v1.0.1)
* **新功能：** 添加了“高质量 (H.265)”模式和 FPS 选择器（30, 24, 15），用于 scrcpy 的屏幕镜像/录制。
* **错误修复：** 解决了屏幕录像未保存到所选路径的问题。
* **关键补丁：** 修复了导致内部浏览器 (WebView2) 在安装版本中打开应用商店时显示白屏的错误。

**鸣谢与致谢：**
* **开发者：** Pablo Villavicencio
* **连接引擎 (ADB)：** Google / Android Open Source Project
* **屏幕镜像引擎 (scrcpy)：** Genymobile
* **网页接口：** Microsoft Edge WebView2

---

## 🇯🇵 [JA] 日本語 (JAPANESE)

DeployX へようこそ！
DeployX は、ADB（Android Debug Bridge）を介して Android デバイスと通信するために設計された強力な Windows 用グラフィカルツールです。複雑なコマンドを入力することなく、デバイスのメンテナンスや管理を簡単に行うことができます。

### 1. 前提条件と重要な警告
DeployX を正しく動作させるためには、以下が必要です：

* Windows 10 または Windows 11。
* PC にインストールされたデバイスの USB ドライバ。
* データ転送可能な USB ケーブル（「充電専用」ケーブルは機能しません）。
* プログラムの完全性：本ソフトウェアはブラウザエンジン（WebView2）等に依存しています。 **`DeployX.exe` ファイルを元のフォルダーから絶対に移動しないでください**。「`WebView2Loader.dll`」や「`runtimes`」フォルダーから切り離すと、プログラムはクラッシュして動作しません。

### 2. ステップバイステップ・ユーザーマニュアル

**ステップ 1：スマートフォンの準備（USB デバッグ）**
1. Android の「設定」>「デバイス情報」に移動します。
2. 「ビルド番号」を7回連続でタップし、開発者向けオプションを有効にします。
3. 戻って「開発者向けオプション」に入り、「USB デバッグ」をオンにします。

**ステップ 2：USB 接続（有線）**
1. `DeployX.exe` を開きます。最初はサイドバーのボタンがグレーアウト（無効）されていますが、これは安全のための正常な動作です。
2. USB ケーブルでスマートフォンを PC に接続します。
3. スマートフォンの画面を確認します。「USB デバッグを許可しますか？」というプロンプトが表示されたら、「常に許可する」にチェックを入れて OK をタップします。
4. DeployX がデバイスを数秒で自動検出します。

**ステップ 3：ワイヤレスデバッグ接続（Wi-Fi）**
1. PC とスマートフォンが同じ Wi-Fi ネットワークに接続されていることを確認します。
2. 開発者向けオプションで「ワイヤレスデバッグ」をオンにし、そこをタップして IP アドレスとポートを確認します（例: `192.168.1.70:37413`）。
3. DeployX で **[ ワイヤレスデバッグ ]** をクリックし、正確な IP とポートを入力して「接続」を押します。

**ステップ 4：安全な切断**
終了したらケーブルを抜くか、**[ 切断 ]** をクリックするだけです。DeployX はシステムを保護するため、ボタンを即座にロックします。

### 3. 機能の詳細な説明（サイドバーメニュー）
* **[ デバイスを表示 ]:** USB または Wi-Fi 経由で接続されているデバイスのリストを確認して更新します。
* **[ ワイヤレスデバッグ ]:** IP アドレスとポートを使用して、Wi-Fi 経由でデバイスに接続します。
* **[ デバイス情報 ]:** デバイスの技術的詳細（モデル、Android バージョン、バッテリー等）を表示。
* **[ アプリストア ]:** アプリを直接ダウンロードするための代替ウェブストア (APKPure、F-Droid など) にすばやくアクセスします。
* **[ APK/XAPK のインストール ]:** PC からスマートフォンへ直接インストール。
* **[ アプリリスト ]:** アプリのアンインストールやキャッシュ消去を行うパッケージマネージャー。
* **[ エクスプローラー ]:** 双方向ファイルマネージャー（Pull / Push 機能）。
* **[ 画面を表示 ]:** 高度な画面ミラーリングと録画（scrcpyを使用）。音声ルーティング機能付きでキャストしたり、PCのWebカメラとして使用したり、仮想ディスプレイを作成したり、高画質で録画（H.265/FPS制御）できます。
* **[ LOGCAT ]:** Android システムのリアルタイムログを表示。アプリの診断に不可欠。
* **[ タスクモニター ]:** RAM の消費量や CPU 使用率をリアルタイムで監視。**高度なフォレンジック診断とデータ抽出のための新しい「高度なデバイスレポート」が含まれています。**
* **[ ADB バージョン ]:** 実行中の Android Debug Bridge エンジンの現在のバージョンを確認します。
* **[ ANDROID コンソール ]:** 直接の ADB shell コマンドを受信する準備ができたネイティブ コマンドプロンプトを開きます。
* **[ 切断 ]:** ADB サーバーを安全に終了し、すべてのデバイスを切断します。

### 4. よくあるトラブルシューティング（FAQ）
**Q: デバイスを接続してもボタンがグレーのままです。**
A: 主に以下の3つの原因が考えられます：
1. **USB デバッグが有効になっていない。** （最も一般的なエラー）。
2. **権限がない。** スマートフォンのロックを解除し、画面のプロンプトで許可してください。
3. **USB ケーブルがデータ転送に対応していない。**

**Q: プログラムを開いてもすぐにクラッシュします。**
A: 重要なファイルが不足しています。`WebView2Loader.dll` が `DeployX.exe` と全く同じフォルダー内にあることを確認してください。

### 更新履歴 (v1.0.2)
* **新機能：** 強力なフォレンジック診断ツール「高度なデバイスレポート」を追加しました。
* **メガ抽出：** 深いシステムパラメータ（基本ハードウェア、バッテリーの劣化、プロセッサ、リアルタイムネットワーク、ユーザー、セキュリティポリシー、センサー）を抽出するようになりました。
* **アカウントとプライバシー：** メールとリンクされたアカウントの完全かつ詳細な検出。
* **インターフェース：** 各パラメータを詳細に説明するインタラクティブなフローティングウィンドウ（ToolTips）をテーブルに統合しました。言語セレクターの下に目立たないバージョンタグ (v1.0.2) を追加しました。
* **エクスポート：** 完全な診断をテキストファイル（`.txt`）にエクスポートするオプションを追加しました。

### 更新履歴 (v1.0.1)
* **新機能：** scrcpyを使用した画面ミラーリング/録画用の「高画質（H.265）」モードとFPSセレクター（30、24、15）を追加しました。
* **バグ修正：** 画面録画が選択したパスに保存されない問題を解決しました。
* **重要なパッチ：** インストール版でアプリストアを開く際、内部ブラウザ（WebView2）が真っ白な画面を表示するバグを修正しました。

**クレジットと謝辞:**
* **開発者：** Pablo Villavicencio
* **接続エンジン (ADB):** Google / Android Open Source Project
* **画面ミラーリングエンジン (scrcpy):** Genymobile
* **ウェブインターフェース:** Microsoft Edge WebView2

---

## 🇷🇺 [RU] РУССКИЙ (RUSSIAN)

Добро пожаловать в DeployX!
DeployX — это мощный графический инструмент для Windows, предназначенный для взаимодействия с устройствами Android через ADB (Android Debug Bridge). Его цель — облегчить обслуживание, отладку и управление вашим телефоном или планшетом без необходимости ввода сложных команд в консоли.

### 1. ПРЕДВАРИТЕЛЬНЫЕ ТРЕБОВАНИЯ И ВАЖНЫЕ ПРЕДУПРЕЖДЕНИЯ
Для правильной работы DeployX вам потребуется:

* Windows 10 или Windows 11.
* USB-драйверы для вашего телефона, установленные на ПК.
* USB-кабель для передачи данных (кабели «только для зарядки» не подойдут).
* ЦЕЛОСТНОСТЬ ПРОГРАММЫ: Данное программное обеспечение зависит от браузерного движка (WebView2) и других библиотек. **НИКОГДА не извлекайте файл `DeployX.exe` из его исходной папки**. Если вы отделите его от таких файлов, как `WebView2Loader.dll` или папки `runtimes`, программа завершится с ошибкой и не будет работать.

### 2. ПОШАГОВОЕ РУКОВОДСТВО ПОЛЬЗОВАТЕЛЯ

**Шаг 1: Подготовка телефона (Отладка по USB)**
Перед подключением телефона к компьютеру необходимо включить связь:
1. Перейдите в Настройки > О телефоне на вашем Android.
2. Нажмите 7 раз подряд на «Номер сборки», чтобы включить Параметры разработчика.
3. Вернитесь назад, войдите в «Параметры разработчика» и включите «Отладка по USB».

**Шаг 2: Подключение по USB (проводное)**
1. Откройте `DeployX.exe`. Вы увидите экран приветствия. Изначально кнопки бокового меню будут неактивны (серого цвета). Это мера безопасности.
2. Подключите телефон к ПК с помощью USB-кабеля.
3. Проверьте экран телефона: появится запрос «Разрешить отладку по USB?». Установите флажок «Всегда разрешать» и нажмите ОК.
4. DeployX автоматически обнаружит ваше устройство за несколько секунд.

**Шаг 3: Беспроводная отладка (Wi-Fi)**
1. Убедитесь, что ваш ПК и телефон подключены к одной сети Wi-Fi.
2. В параметрах разработчика включите «Беспроводная отладка» и нажмите на нее, чтобы увидеть свой IP-адрес и порт (например, `192.168.1.70:37413`).
3. В DeployX нажмите **[ БЕСПРОВОДНАЯ ОТЛАДКА ]**, введите точные IP и порт и нажмите «Подключить».

**Шаг 4: Безопасное отключение**
По завершении просто отсоедините кабель или нажмите **[ ОТКЛЮЧИТЬ ]**. DeployX мгновенно заблокирует кнопки.

### 3. ПОДРОБНОЕ ОПИСАНИЕ ФУНКЦИЙ (БОКОВОЕ МЕНЮ)
* **[ ПОКАЗАТЬ УСТРОЙСТВА ]:** Проверяет и обновляет список устройств, подключенных через USB или Wi-Fi.
* **[ БЕСПРОВОДНАЯ ОТЛАДКА ]:** Подключение к устройству по Wi-Fi с использованием его IP-адреса и порта.
* **[ ИНФО ОБ УСТРОЙСТВЕ ]:** Главная панель (модель, версия Android, заряд батареи).
* **[ МАГАЗИНЫ ПРИЛОЖЕНИЙ ]:** Быстрый доступ к альтернативным веб-магазинам (APKPure, F-Droid и т. д.) для прямой загрузки приложений.
* **[ УСТАНОВИТЬ APK/XAPK ]:** Установка приложений напрямую с ПК на телефон.
* **[ СПИСОК ПРИЛОЖЕНИЙ ]:** Диспетчер пакетов для удаления приложений или очистки кэша.
* **[ ПРОВОДНИК ]:** Двусторонний файловый менеджер (извлечение/отправка файлов).
* **[ ПРОСМОТР ЭКРАНА ]:** Расширенное зеркалирование и запись экрана (на базе scrcpy). Транслируйте устройство с маршрутизацией звука, используйте его как веб-камеру ПК, создавайте виртуальные дисплеи или записывайте в высоком качестве (H.265/контроль FPS).
* **[ LOGCAT ]:** Показывает журнал системы Android в реальном времени.
* **[ МОНИТОР ЗАДАЧ ]:** Мониторинг потребления ОЗУ и загрузки ЦП. **Включает новый «Расширенный отчет об устройстве» для глубокой криминалистической диагностики и извлечения данных.**
* **[ ВЕРСИЯ ADB ]:** Проверка текущей версии работающего движка Android Debug Bridge.
* **[ КОНСОЛЬ ANDROID ]:** Открывает встроенную командную строку, готовую к приему прямых команд оболочки ADB.
* **[ ОТКЛЮЧИТЬ ]:** Безопасное завершение работы сервера ADB и отключение всех устройств.

### 4. ЧАСТО ЗАДАВАЕМЫЕ ВОПРОСЫ (FAQ)
**В: Я подключаю телефон, но кнопки DeployX остаются серыми.**
О: Это происходит по трем основным причинам:
1. **ОТЛАДКА ПО USB НЕ ВКЛЮЧЕНА.** Это самая частая ошибка.
2. **Отсутствие разрешений.** Разблокируйте телефон и примите запрос ADB.
3. **Ваш USB-кабель не поддерживает передачу данных.**

**В: Программа открывается, но почти сразу закрывается.**
О: Отсутствуют жизненно важные файлы. Убедитесь, что файл `WebView2Loader.dll` находится в той же папке, что и `DeployX.exe`.

### ИСТОРИЯ ИЗМЕНЕНИЙ (v1.0.2)
* **Новые функции:** Добавлен «Расширенный отчет об устройстве», мощный криминалистический диагностический инструмент.
* **Мега-извлечение:** Теперь извлекаются глубокие системные параметры (базовое оборудование, износ батареи, процессор, сеть в реальном времени, пользователи, политики безопасности и датчики).
* **Учетные записи и конфиденциальность:** Полное и подробное обнаружение электронных писем и связанных учетных записей.
* **Интерфейс:** В таблицу встроены интерактивные всплывающие окна (ToolTips) для подробного объяснения каждого параметра. Добавлен ненавязчивый тег версии (v1.0.2).
* **Экспорт:** Добавлена возможность экспорта полной диагностики в текстовый файл (`.txt`).

### ИСТОРИЯ ИЗМЕНЕНИЙ (v1.0.1)
* **Новые функции:** Добавлен режим «Высокое качество (H.265)» и селектор FPS (30, 24, 15) для трансляции/записи экрана с помощью scrcpy.
* **Исправления:** Решена проблема, из-за которой записи экрана не сохранялись по выбранному пути.
* **Критический патч:** Исправлена ошибка, из-за которой внутренний браузер (WebView2) отображал белый экран при открытии магазинов приложений в установленной версии.

**Авторы и Благодарности:**
* **Разработчик:** Pablo Villavicencio
* **Движок подключения (ADB):** Google / Android Open Source Project
* **Механизм зеркалирования экрана (scrcpy):** Genymobile
* **Веб-интерфейс:** Microsoft Edge WebView2
