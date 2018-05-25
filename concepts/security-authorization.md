# <a name="authorization-and-the-security-api-in-microsoft-graph"></a>Autorisierung und die Sicherheits-API in Microsoft Graph

Sicherheitsdaten, auf die über die Sicherheits-API in Microsoft Graph zugegriffen werden kann, sind vertraulich und sind sowohl durch Berechtigungen als auch durch Azure Active Directory (Azure AD) Rollen geschützt.

Die Sicherheits-API unterstützt zwei Arten von Autorisierung:

- **Autorisierung auf Anwendungsebene** – Es ist kein Benutzer angemeldet (z. B. ein SIEM-Szenario). Die Berechtigungen, die der Anwendung gewährt wurden, bestimmen die Autorisierung. 
    >**Hinweis:** Diese Option unterstützt auch Fälle, in denen die rollenbasierte Zugriffssteuerung (RBAC) von der Anwendung verwaltet wird.
- **Benutzer-delegierte Autorisierung** – Ein Benutzer, der ein Mitglied des Azure AD-Mandanten ist, ist angemeldet. Der Benutzer muss ein Mitglied einer beschränkten Azure AD-Administratorrolle sein – mit Leseberechtigung für Sicherheitsfunktionen oder Sicherheitsadministrator – zusätzlich dazu, dass der Anwendung die erforderlichen Berechtigungen erteilt wurden.

Wenn Sie die Sicherheits-API aus Graph Explorer aufrufen:

- Der Azure AD-Mandantenadministrator muss explizit die erforderlichen Berechtigungen für die Graph-Explorer-Anwendung gewähren.
- Der Benutzer muss Mitglied einer beschränkten Azure AD-Administratorrolle (mit Leseberechtigung für Sicherheitsfunktionen oder Sicherheitsadministrator) sein.

>**Hinweis**: Graph Explorer unterstützt die Autorisierung auf Anwendungsebene nicht.

Wenn Sie die Sicherheits-API aus einer benutzerdefinierten oder Ihrer eigenen Anwendung angerufen:

- Der Azure AD-Mandantenadministrator muss Ihrer Anwendung explizit zustimmen. Dies ist sowohl für die Autorisierung auf Anwendungsebene als auch für benutzerdelegierte Autorisierung erforderlich.
- Wenn Sie benutzerdelegierte Autorisierung nutzen, muss der Benutzer Mitglied einer beschränkten Azure AD-Administratorrolle mit Leseberechtigung für Sicherheitsfunktionen oder Sicherheitsadministrator sein.

## <a name="manage-authorization-in-security-api-client-applications"></a>Verwalten der Autorisierung in Sicherheits-API-Clientanwendungen

Über die Sicherheits-API in Microsoft Graph bereitgestellte Sicherheitsdaten sind vertraulich und müssen durch entsprechende Authentifizierungs- und Autorisierungsmechanismen geschützt werden. Die folgende Tabelle enthält die Schritte zum Registrieren und Erstellen einer Clientanwendung, die auf die Sicherheits-API zugreifen kann.

| **Wer?** | **Aktion** |
|:---------------------|:------------------|
|Anwendungsentwickler oder -besitzer|Registrieren Sie die Anwendung als eine Enterprise-Anwendung.|
|Mandantenadministrator|Gewähren Sie Ihrer Anwendung entsprechende Berechtigungen.|
|Mandantenadministrator|Zuweisen von Benutzerrollen.|
|Anwendungsentwickler|Melden Sie sich als Benutzer an, und verwenden Sie die Anwendung, um auf die Sicherheit-API zuzugreifen.|

Die Registrierung der Anwendung definiert nur, welche Berechtigungen die Anwendung zum Ausführen braucht. Sie gewährt der Anwendung KEINE Berechtigungen.

Der Azure AD-Mandantenadministrator MUSS der Anwendung die Berechtigungen explizit gewähren. Dies muss pro Mandant erfolgen und muss *jedes Mal durchgeführt werden*, wenn die Anwendungsberechtigungen im Anwendungsregistrierungsportal geändert werden.

Nehmen wir beispielsweise an, dass Sie eine Anwendung, zwei Azure AD-Mandanten, **T1** und **T2**, und zwei Berechtigungen, **P1** und **P2**, haben. Der Autorisierungsprozess sieht folgendermaßen aus:

- Die Anwendung registriert sich, um Berechtigung **P1** anzufordern.
- Wenn Benutzer im Mandanten **T1** ein Azure AD-Token für diese Anwendung erhalten, enthält das Token keine Berechtigungen.
- Azure AD-Administrator des Mandanten **T1** gewährt der Anwendung explizit Berechtigungen. Wenn Benutzer im Mandanten **T1** ein Azure AD-Token für diese Anwendung erhalten, enthält das Token die Berechtigung **P1**.
- Wenn Benutzer im Mandanten **T2** ein Azure AD-Token für diese Anwendung erhalten, enthält das Token keine Berechtigungen, da der Administrator des Mandanten **T2** der Anwendung noch keine Berechtigungen erteilt hat. Berechtigung müssen *pro Mandant* und *pro Anwendung* erteilt werden.
- Die Anwendung hat ihre Registrierung geändert, sodass sie jetzt die Berechtigungen **P1** und **P2** erfordert.
- Wenn Benutzer im Mandanten **T1** ein Azure AD-Token für diese Anwendung erhalten, enthält das Token nur die Berechtigung **P1**. Berechtigungen, die einer Anwendung gewährt werden, werden als Momentaufnahmen dessen, was gewährt wurde, aufgezeichnet. Sie *ändern sich nicht automatisch* nach der (Berechtigungs-)Änderung der Anwendungsregistrierung.
- Der Administrator des Mandanten **T2** erteilt Berechtigungen **P1** und **P2** für die Anwendung. Wenn nun Benutzer im Mandanten **T2** ein Azure AD-Token für diese Anwendung erhalten, enthält das Token die Berechtigungen **P1** und **P2**.

>**Hinweis**: Die Azure AD-Token für die Anwendung im Mandanten **T1** und die Anwendung in Mandant **T2** enthalten verschiedene Berechtigungen, da jeder Mandantenadministrator verschiedene Berechtigungen für die Anwendung erteilt hat.

- Damit die Anwendung erneut in Mandant **T1** funktioniert, muss der Administrator des Mandanten **T1** explizit die Berechtigungen **P1** und **P2** für die Anwendung erteilen.

## <a name="register-an-application-in-the-azure-ad-v20-endpoint"></a>Registrieren einer Anwendung im Azure AD v2.0-Endpunkt

Um eine Anwendung im Azure AD v2.0-Endpunkt zu registrieren, brauchen Sie:

- **Anwendungsname** – Zeichenfolge für den Namen der Anwendung.
- **Umleitungs-URL** – Die URL, an die die Authentifizierungsantwort von Azure AD gesendet wird. Um zu beginnen, können Sie die Homepage der Test Client Web App verwenden.
- **Erforderliche Berechtigungen** – Die Berechtigungen, die die Anwendung erfordert, um Microsoft Graph aufrufen zu können.

So registrieren Sie Ihre Anwendung

1. Gehen Sie auf https://apps.dev.microsoft.com/, und melden Sie sich an.
    >**Hinweis**: Sie müssen kein Mandantenadministrator sein. Sie werden zur Liste **Meine Programme** weitergeleitet.
2. Wählen Sie **App hinzufügen**, und geben Sie einen **Anwendungsnamen** ein, um eine neue Anwendung zu erstellen.
3. Wählen Sie auf der Registrierungsseite für die neue Anwendung **Plattform hinzufügen** > **Web**. Geben Sie im Feld **Umleitungs-URL** die Umleitungs-URL ein.
4. Wählen Sie im Abschnitt **Microsoft Graph-Berechtigungen** unter **Delegierte Berechtigungen** **Hinzufügen** aus. Wählen Sie im Dialogfeld die erforderlichen Berechtigungen. Eine Liste von Berechtigungen finden Sie unter [Sicherheitsberechtigungen](../concepts/permissions_reference.md#security-permissions).

    >Die Sicherheits-API erfordert den Bereich SecurityEvents.Read.All für GET-Abfragen und den Bereich SecurityEvents.ReadWrite.All für PATCH/POST-Abfragen.

5. Wählen Sie **Speichern** aus.

Speichern Sie die folgenden Informationen:

- Anwendungs-ID
- Umleitungs-URL
- Liste der erforderlichen Berechtigungen

Weitere Informationen finden Sie unter: [Registrieren Ihrer App beim Azure AD v2.0-Endpunkt](../concepts/auth_register_app_v2.md).

## <a name="grant-permissions-to-an-application"></a>Gewähren von Berechtigungen für eine Anwendung

Die Anwendungsregistrierung definiert nur, welche Berechtigungen die Anwendung erfordert. Sie gewährt der Anwendung diese Berechtigungen NICHT. Ein Azure AD-Mandantenadministrator muss diese Berechtigungen explizit gewähren, indem er den Endpunkt für die Administratorzustimmung aufruft. Einzelheiten hierzu finden Sie unter [Verwenden des Endpunkts für die Administratorzustimmung](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-v2-scopes#using-the-admin-consent-endpoint).

Um einer Anwendung Berechtigungen zu gewähren, brauchen Sie:

- **Anwendungs-ID** – Die Anwendungs-ID, die Ihrer App vom App-Registrierungsportal zugewiesen wurde.
- **Umleitungs-URL** – Die Zeichenfolge, die Sie im App-Registrierungsportal für die Authentifizierungsantwort festgelegt haben.

So gewähren Sie Berechtigungen

- Erstellen Sie in einem Texteditor die folgende URL-Zeichenfolge:

    `https://login.microsoftonline.com/common/adminconsent?client_id=<Application Id>&state=12345&redirect_uri=<Redirect URL>`

- Rufen Sie in einem Webbrowser diese URL auf, und melden Sie sich als Mandantenadministrator an. Das Dialogfeld zeigt die Liste der Berechtigungen, die die Anwendung erfordert, wie im App-Registrierungsportal eingegeben. Wählen Sie **OK**, um der Anwendung diese Berechtigungen zu erteilen.

> **Hinweis:** Dieser Schritt erteilt Berechtigungen an die Anwendung – nicht an den Benutzer. Das bedeutet, dass alle Benutzer, die zum Azure AD-Mandanten gehören, die diese Anwendung verwenden, diese Berechtigungen erhalten – sogar Benutzer ohne Administratorberechtigung.

## <a name="assign-azure-ad-roles-to-users"></a>Zuweisen von Azure AD-Rollen für Benutzer

Nachdem einer Anwendung Berechtigungen erteilt wurden, erhalten alle Benutzer, die Zugriff auf die Anwendung (d. h. Mitglieder des Azure AD-Mandanten) die Berechtigungen, die erteilt wurden. Um vertrauliche Daten zusätzlich zu schützen, verlangt die Sicherheits-API, dass Benutzern die Azure AD-Rolle **Benutzer mit Leseberechtigung für Sicherheitsfunktionen** zugewiesen wird. Einzelheiten hierzu finden Sie unter [Zuweisen von Administratorrollen](https://docs.microsoft.com/de-DE/azure/active-directory/active-directory-assign-admin-roles-azure-portal) und [Zuweisen eines Benutzers zu Administratorrollen](https://docs.microsoft.com/de-DE/azure/active-directory/active-directory-users-assign-role-azure-portal).

>**Hinweis:** Sie müssen Mandantenadministrator sein, um diesen Schritt auszuführen.

So weisen Sie Benutzern Rollen zu

- Melden Sie sich beim [Azure-Portal](https://portal.azure.com)an.(http://portal.azure.com)
- Wählen Sie im Menü **Azure Active Directory** > **Benutzer**.
- Wählen Sie den Namen des Benutzers aus.
- Wählen Sie **Verwalten** > **Directory-Rolle**.
- Wählen Sie **Eingeschränkter Administrator**, und wählen Sie das Kontrollkästchen **Benutzer mit Leseberechtigung für Sicherheitsfunktionen** aus.
- Wählen Sie **Speichern** aus.

## <a name="create-an-authentication-code"></a>Erstellen eines Authentifizierungscodes

Um einen Authentifizierungscode zu erstellen, brauchen Sie:

- **Anwendungs-ID** – Die Anwendungs-ID, die Ihrer App vom App-Registrierungsportal zugewiesen wurde.
- **Umleitungs-URL** – Die URL, an die die Authentifizierungsantwort von Azure AD gesendet wird. Zum Beginnen können Sie http://localhost oder die Homepage der Test Client Web App verwenden.
- **Anwendungsschlüssel** (optional) — Der Schlüssel der Anwendung. Dies gilt, wenn Sie eine Anwendung entwickeln, die Nur-App-Authentifizierungscodes verwendet (d. h. delegierte Benutzerauthentifizierung nicht unterstützt).

Die folgende Tabelle enthält Ressourcen, die Sie zum Erstellen eines Authentifizierungscodes verwenden können.

|**Art der Anwendung**|**Authentifizierungsbibliothek**|
|------------------------|----------------------------|
|[Desktop-Apps – iOS](https://docs.microsoft.com/de-DE/azure/active-directory/develop/guidedsetups/active-directory-ios)|[MSAL.framework: Microsoft-Authentifizierungsbibliothek (Vorschau) für iOS](https://github.com/AzureAD/microsoft-authentication-library-for-objc)|
|[Desktop-Apps – Android](https://docs.microsoft.com/de-DE/azure/active-directory/develop/guidedsetups/active-directory-android)|[Microsoft-Authentifizierungsbibliothek (MSAL)](http://javadoc.io/doc/com.microsoft.identity.client/msal)|
|[Desktop-Apps – .NET](https://docs.microsoft.com/de-DE/azure/active-directory/develop/guidedsetups/active-directory-windesktop)|[Microsoft-Authentifizierungsbibliothek (MSAL)](https://www.nuget.org/packages/Microsoft.Identity.Client)|
|[Web-Apps — JavaScript SPA](https://docs.microsoft.com/de-DE/azure/active-directory/develop/guidedsetups/active-directory-javascriptspa)|[Microsoft-Authentifizierungsbibliothek für JavaScript (Vorschau)](https://github.com/AzureAD/microsoft-authentication-library-for-js)|
|[Web-Apps — .NET-Webserver](https://docs.microsoft.com/de-DE/azure/active-directory/develop/guidedsetups/active-directory-aspnetwebapp)|OpenIdConnection, Cookies, SystemWeb|
|[Web-Apps - NodeJS-Web-App](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-v2-devquickstarts-node-web)||

Für Anwendungen, die keine der vorhandenen Bibliotheken verwenden, siehe [Im Namen eines Benutzers zugreifen](../concepts/auth_v2_user.md).

1. Abrufen eines Codes von Azure AD. Die Abfrage zum Aufruf enthält die Parameter für die Anwendungs-ID, Umleitungs-URL und **erforderliche Berechtigungen**.
2. Verwenden des Codes zum Abrufen eines Zugriffstokens.

Wenn Sie die OpenID Connect-Bibliothek verwenden, lesen Sie [Authentifizieren mithilfe von Azure Active Directory und OpenID Connect](https://docs.microsoft.com/de-DE/azure/architecture/multitenant-identity/authenticate), und rufen Sie `app.UseOpenIdConnectAuthentication()` auf.

>**Hinweis:** Wenn Sie benutzerdelegierte Authentifizierungstoken anfordern, ist der Parameter für die Bibliothek **angeforderte Bereiche**. Verwenden Sie User.Read für diesen Parameter statt den Anforderungen der registrierten Anwendung. Der Parameter **angeforderte Bereiche** hat keinen Einfluss auf die Berechtigungen, die in den zurückgegebenen Authentifizierungstoken enthalten sind. Diese werden durch die Berechtigungen bestimmt, die der Mandantenadministrator der Anwendung erteilt.

Wenn Sie beispielsweise die Bibliothek .NET MSAL verwenden, rufen Sie die folgenden auf:

`var accessToken = (await client.AcquireTokenAsync(scopes)).AccessToken;`

>**Hinweis:** Dieses Beispiel sollte die geringsten Berechtigungen, z. B. User.Read, verwenden. Das zurückgegebene Zugriffstoken kann jedoch Berechtigungen enthalten, die dem aktuellen Benutzer vom Mandantenadministrator gewährt wurden, z. B. User.Read.All oder User.ReadWrite.All.

Ein Token (Zeichenfolge) wird von Azure AD zurückgegeben, das Ihre Authentifizierungsinformation und die von der Anwendung benötigten Berechtigungen enthält. Weisen Sie dieses Token dem HTTP-Header als Bearer-Token zu, wie im folgenden Beispiel gezeigt.

`request.Headers.Authorization = new AuthenticationHeaderValue("bearer", accessToken);`

Microsoft Graph wird die in diesem Token enthaltenen Informationen überprüfen und den Zugriff gewähren oder ablehnen.

Um die Ansprüche zu sehen, die in den zurückgegebenen Token enthaltenen sind, verwenden Sie die NuGet-Bibliothek System.IdentityModel.Tokens.Jwt.

`JwtSecurityTokenHandler tokenHandler = new JwtSecurityTokenHandler();`</br>
`var securityToken = tokenHandler.ReadToken(accessToken) as JwtSecurityToken;`

Die Antwort von Microsoft Graph enthält eine Kopfzeile, die-Client-Anforderungs-ID heißt und eine GUID ist. Wenn der Zugriff verweigert wird, geben Sie diese GUID bei Supportanfragen in der [Microsoft Tech Community](https://techcommunity.microsoft.com/t5/Microsoft-Graph-Security-API/ct-p/SecurityGraphAPI) an, damit wir Ihnen helfen können, die Ursache für diesen Authentifizierungsfehler zu untersuchen.
