# SaniApp

🔧 Technischer Überblick (ohne Geld)
Cross-Plattform App: Du brauchst ein Framework wie Flutter oder React Native, das Android und iOS unterstützt.

Push-Benachrichtigungen: Kostenlos über Firebase Cloud Messaging (FCM).

Backend-Kommunikation: Kostenloses Backend wie Supabase, Firebase, oder ein eigener kleiner Node.js-Server auf Render.com (Free Tier).

Deployment auf Android: Kostenlos möglich.

Deployment auf iOS: Kein App Store ohne Developer Account, aber:

Testen/Verteilen über TestFlight oder lokal auf deinem iPhone mit Xcode, wenn du einen Mac hast.

✅ Lösungsschritte
1. App Entwicklung (Flutter)
Verwende Flutter (kostenlos, Open Source, entwickelt von Google)

Damit kannst du eine App für Android & iOS gleichzeitig entwickeln

IDE: Visual Studio Code oder Android Studio

2. Push Benachrichtigungen (Firebase Cloud Messaging)
Erstelle ein kostenloses Konto bei Firebase

Richte dort ein Projekt ein

Integriere FCM in deine Flutter App → damit kannst du sowohl Android als auch iOS Pushs senden

3. Backend für das Sekretariat
Variante A (einfach):

Erstelle ein kleines Web-Formular (HTML/JS) für das Sekretariat (z. B. "Notfall senden")

Wenn gedrückt, sendet es eine Anfrage an dein Backend (z. B. Firebase Function oder Render)

Variante B (robuster):

Supabase (kostenloses Backend as a Service) oder ein kleiner Express.js Server auf Render.com

4. Push senden
Dein Backend empfängt die Anfrage und sendet via FCM eine Push Notification an die registrierten Geräte

🧪 Testing & Deployment
Android:
Kompilieren und direkt auf dein Gerät laden (flutter run oder adb install)

Oder: APK/Bundle generieren und manuell installieren

iOS (ohne Dev Account):
Schwierig, aber möglich:

Mit Mac: App mit Xcode direkt auf ein iPhone installieren (max. 7 Tage gültig ohne Account)

Oder: AltStore oder TestFlight mit Einladung durch einen Freund mit Dev Account
