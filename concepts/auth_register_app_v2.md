# <a name="register-your-app-with-the-azure-ad-v20-endpoint"></a>Registrieren Ihrer App beim Azure AD v2.0-Endpunkt

Ihre App muss bei Azure AD registriert werden. Durch Registrieren Ihrer App werden eine eindeutige Anwendungs-ID und andere Werte erstellt, die die App zum Authentifizieren bei Azure AD und zum Abrufen von Tokens verwendet. Für den Azure AD v2.0-Endpunkt registrieren Sie Ihre App mit dem [Microsoft App-Registrierungsportal](https://apps.dev.microsoft.com). Sie können entweder ein Microsoft-Konto oder ein Geschäfts-, Schul- oder Unikonto zum Registrieren Ihrer App verwenden. Abhängig vom Typ der von Ihnen entwickelten App müssen Sie während der Registrierung eine oder mehrere Eigenschaften kopieren, die beim Konfigurieren von Authentifizierung und Autorisierung für die App verwendet werden sollen. 


> **Hinweis:** Dieser Artikel befasst sich in erster Linie mit dem Registrieren von Apps beim Azure AD v2.0-Endpunkt. Informationen zum Registrieren Ihrer App beim Azure AD-Endpunkt finden Sie unter [Überlegungen zum Azure AD-Endpunkt](#azure-ad-endpoint-considerations) weiter unten.
> 
> Beachten Sie außerdem Folgendes: Wenn Sie bereits zuvor Apps im Microsoft Azure-Portal registriert haben, werden diese nicht im App-Registrierungsportal aufgeführt. Verwalten Sie diese Apps im Azure-Portal. 


Der folgende Screenshot zeigt ein Beispiel für die Registrierung einer Web-App, die mit einem Kennwort und implizitem Fluss konfiguriert wurde. ![Web-App-Registrierung mit Kennwort und Zulassung des impliziten Flusses](./images/v2-web-registration.png)

Führen Sie die folgenden Schritte aus, um Ihre App zu registrieren; denken Sie daran, die angegebenen Werte für die Konfiguration der Autorisierung für Ihre App zu kopieren:

1. Melden Sie sich beim [Microsoft App-Registrierungsportal](https://apps.dev.microsoft.com/) an.
   
    Sie können sich mit einem Microsoft-Konto oder einem Geschäfts-, Schul- oder Unikonto anmelden. 

2. Klicken Sie auf **App hinzufügen**.
    > Hinweis: Wenn Sie sich mit einem Geschäfts-, Schul- oder Unikonto angemeldet haben, wählen Sie die Schaltfläche **App hinzufügen** für **Konvergente Anwendungen**. 

3. Geben Sie einen Namen für die App ein, und wählen Sie **Anwendung erstellen** aus.

    Die Registrierungsseite wird angezeigt, und die Eigenschaften der App werden aufgeführt.

4. Kopieren Sie die Anwendungs-ID: Dies ist der eindeutige Bezeichner für Ihre App.

    Sie werden die Anwendungs-ID verwenden, um die App zu konfigurieren.

5. Wählen Sie unter **Plattformen** **Plattform hinzufügen**, und wählen Sie die passende Plattform für Ihre App aus:
    
    **Für systemeigene oder mobile Apps**:

    1. Wählen Sie **Systemeigene Anwendung**.

    2. Kopieren Sie den Wert des **integrierten Umleitungs-URI**. Sie benötigen diesen, um Ihre App zu konfigurieren.

        Der Umleitungs-URI ist ein eindeutiger URI für Ihre Anwendung, der sicherstellt, dass an diesen URI gesendete Nachrichten nur an diese Anwendung gesendet werden. 

    **Für Web-Apps:**

    1. Klicken Sie auf **Web**.

    2. Abhängig vom verwendeten Authentifizierungsflusstyp müssen Sie möglicherweise sicherstellen, dass das Kontrollkästchen **Impliziten Fluss zulassen** aktiviert ist. 
        
        Die Option **Impliziten Fluss zulassen** aktiviert den hybriden und den impliziten OpenID Connect-Fluss. Der hybride Fluss ermöglicht es der App, sowohl Anmeldeinformationen (das ID-Token) als auch Artefakte (in diesem Fall einen Autorisierungscode) zu erhalten, die die App zum Abrufen eines Zugriffstokens verwendet. Der hybride Fluss ist der von der Middleware OWIN OpenID Connect verwendete Standardfluss. Für Einzelseiten-Apps (SPA) ermöglicht der implizite Fluss der App, Anmeldeinformationen und das Zugriffstoken zu erhalten. 

    3. Geben Sie eine Umleitungs-URL an.
        
        Die Umleitungs-URL ist die Position in Ihrer App, die der Azure AD v2.0-Endpunkt aufruft, wenn er die Authentifizierungsanforderung verarbeitet hat.

    4. Wählen Sie unter **Anwendungsgeheimnisse** die Option **Neues Kennwort generieren** aus. Kopieren Sie das Anwendungsgeheimnis aus dem Dialogfeld **Neues Kennwort wurde generiert**.
        > **Wichtig:** Sie müssen das Anwendungsgeheimnis kopieren, bevor Sie das Dialogfeld **Neues Kennwort wurde generiert** schließen. Nachdem Sie das Dialogfeld geschlossen haben, können Sie das Geheimnis nicht mehr abrufen. 
            
6. Wählen Sie **Speichern** aus.


Die folgende Tabelle zeigt die Eigenschaften, die Sie für verschiedene Arten von Apps konfigurieren und kopieren müssen. _Zugewiesen_ bedeutet, dass Sie den von Azure AD zugewiesenen Wert verwenden sollten.


| App-Typ | Plattform | Anwendungs-ID | Anwendungsgeheimnis | Umleitungs-URI/-URL | Impliziter Fluss 
| --- | --- | --- | --- | --- | --- |
| Systemeigen/Mobil | Systemeigen | Zugewiesen  | Nein | Zugewiesen | Nein |
| Web-App | Web | Zugewiesen | Ja | Ja | Optional <br/>Die Middleware OpenID Connect verwendet standardmäßig den hybriden Fluss (Ja) | 
| Einzelseiten-App (Single Page App, SPA) | Web | Zugewiesen | Ja | Ja | Ja <br/> SPAs verwenden den impliziten OpenID Connect-Fluss |
| Dienst/Dämon | Web | Zugewiesen | Ja | Ja | Nein |

Apps, die eine Funktion zur Administratorzustimmung bereitstellen, benötigen möglicherweise eine zusätzliche Umleitungs-URL, an die Azure AD die Antwort zurückgeben kann.

Weitere Details zum App-Registrierungsportal und zu den Eigenschaften, die Sie für Ihre App konfigurieren können, finden Sie in der [Referenz zur App-Registrierung](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-v2-registration-portal).  

## <a name="azure-ad-endpoint-considerations"></a>Überlegungen zum Azure AD-Endpunkt

Sie verwenden das [Azure-Portal](https://aka.ms/aadapplist), um Ihre App beim Azure AD-Endpunkt zu registrieren. Sie konfigurieren die gleichen grundlegenden Eigenschaften wie z. B. Anwendungs-ID, Anwendungsgeheimmis und Umleitungs-URI/-URL, die Sie auch für den v2.0-Endpunkt angeben; es sind jedoch einige wichtige Unterschiede zu beachten: 

- Sie können zum Registrieren einer App nur ein Geschäfts-, Schul- oder Unikonto verwenden.
- Ihre App erfordert für jede Plattform eine andere Anwendungs-ID.
- Wenn Ihre App mehrinstanzenfähig ist, müssen Sie sie im Portal explizit als mehrinstanzenfähig konfigurieren.
- Sie müssen alle Berechtigungen (einschließlich Microsoft Graph-Berechtigungen), die Ihre App im Portal benötigt, vorab konfigurieren. 

Eine Anleitung zur Verwendung des Azure-Portals zum Hinzufügen einer App finden Sie unter [Integrieren von Anwendungen in Azure Active Directory: Hinzufügen einer Anwendung](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications#adding-an-application).
