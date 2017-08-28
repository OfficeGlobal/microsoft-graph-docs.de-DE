# <a name="get-started-with-microsoft-graph-in-an-android-app"></a><span data-ttu-id="927fd-101">Erste Schritte mit Microsoft Graph in einer Android-App</span><span class="sxs-lookup"><span data-stu-id="927fd-101">Get started with Microsoft Graph in an Android app</span></span>

> <span data-ttu-id="927fd-p101">**Sie erstellen Apps für Unternehmenskunden?** Ihre App funktioniert möglicherweise nicht, wenn Ihr Unternehmenskunde Enterprise Mobility-Sicherheitsfunktionen wie <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">bedingten Gerätezugriff</a> aktiviert. In diesem Fall treten bei Ihren Kunden möglicherweise Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="927fd-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="927fd-p102">Zur Unterstützung **aller Unternehmenskunden** über **alle Unternehmensszenarien** hinweg müssen Sie den Azure AD-Endpunkt verwenden und Ihr Apps mithilfe des [Azure-Verwaltungsportals](https://aka.ms/aadapplist) verwalten. Weitere Informationen finden Sie unter [Entscheiden zwischen dem Azure AD- und dem Azure AD v2.0-Endpunkt](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span><span class="sxs-lookup"><span data-stu-id="927fd-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure Management Portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="927fd-p103">Dieser Artikel beschreibt die erforderlichen Aufgaben zum Abrufen eines Zugriffstokens vom Azure AD v2.0-Endpunkt und zum Aufrufen von Microsoft Graph. Sie werden durch die Erstellung der [Connect-Beispiels für Android](https://github.com/microsoftgraph/android-java-connect-sample) geführt und erhalten Informationen zu den Hauptkonzepten, die Sie zur Verwendung von Microsoft Graph in Ihrer App für Android implementieren. In diesem Artikel wird auch beschrieben, wie Sie mithilfe des [Microsoft Graph-SDKs für Android](https://github.com/microsoftgraph/msgraph-sdk-android) oder reinen REST-Aufrufen auf Microsoft Graph zugreifen.</span><span class="sxs-lookup"><span data-stu-id="927fd-p103">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) and explains the main concepts that you implement to use Microsoft Graph in your app for Android. The article also describes how to access Microsoft Graph by using either the [Microsoft Graph SDK for Android](https://github.com/microsoftgraph/msgraph-sdk-android) or raw REST calls.</span></span>

<span data-ttu-id="927fd-110">Um Microsoft Graph in Ihrer App für Android zu verwenden, müssen Sie für Benutzer die Microsoft-Anmeldeseite anzeigen, wie im folgenden Screenshot dargestellt.</span><span class="sxs-lookup"><span data-stu-id="927fd-110">To use Microsoft Graph in your app for Android, you need to show the Microsoft sign in page to your users, as shown in the following screenshot.</span></span>

![Anmeldeseite für Microsoft-Konten auf Android](images/AndroidConnect.png)

<span data-ttu-id="927fd-p104">**Sie möchten keine App erstellen?** Laden Sie sich für einen Schnelleinstieg das [Connect-Beispiel für Android](https://github.com/microsoftgraph/android-java-connect-sample) herunter, auf dem dieser Artikel basiert.</span><span class="sxs-lookup"><span data-stu-id="927fd-p104">**Don't feel like building an app?** Get up and running fast by downloading the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) that this article is based on.</span></span>


## <a name="prerequisites"></a><span data-ttu-id="927fd-114">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="927fd-114">Prerequisites</span></span>

<span data-ttu-id="927fd-115">Für die ersten Schritte benötigen Sie:</span><span class="sxs-lookup"><span data-stu-id="927fd-115">To get started, you'll need:</span></span> 

- <span data-ttu-id="927fd-116">Ein [Microsoft-Konto](https://www.outlook.com/) oder ein [Geschäfts-, Schul- oder Unikonto](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="927fd-116">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
- <span data-ttu-id="927fd-117">Android Studio 2.0 oder eine höhere Version</span><span class="sxs-lookup"><span data-stu-id="927fd-117">Android Studio 2.0 or newer version</span></span>


## <a name="configure-a-new-project"></a><span data-ttu-id="927fd-118">Konfigurieren eines neuen Projekts</span><span class="sxs-lookup"><span data-stu-id="927fd-118">Configure a new project</span></span>

<span data-ttu-id="927fd-119">Wenn Sie das [Connect-Beispiel für Android](https://github.com/microsoftgraph/android-java-connect-sample) heruntergeladen haben, überspringen Sie diesen Schritt.</span><span class="sxs-lookup"><span data-stu-id="927fd-119">If you have downloaded the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample), skip this step.</span></span> 

<span data-ttu-id="927fd-p105">Starten Sie ein neues Projekt in Android Studio. Für den Großteil des Assistenten können Sie die Standardwerte belassen, stellen Sie aber sicher, dass Sie die folgenden Optionen auswählen:</span><span class="sxs-lookup"><span data-stu-id="927fd-p105">Start a new project in Android Studio. You can leave the default values for most of the wizard, just make sure to choose the following options:</span></span>

* <span data-ttu-id="927fd-122">Ziel-Android-Geräte **Telefon und Tablet**</span><span class="sxs-lookup"><span data-stu-id="927fd-122">Target Android Devices - **Phone and Tablet**</span></span>
    * <span data-ttu-id="927fd-123">Minimales SDK - **API 16: Android 4.1 (Jelly Bean)**</span><span class="sxs-lookup"><span data-stu-id="927fd-123">Minimum SDK - **API 16: Android 4.1 (Jelly Bean)**</span></span>
* <span data-ttu-id="927fd-124">Hinzufügen einer Aktivität zu Mobile - **Grundlegende Aktivität**</span><span class="sxs-lookup"><span data-stu-id="927fd-124">Add an Activity to Mobile - **Basic Activity**</span></span>
 
<span data-ttu-id="927fd-125">Auf diese Weise erhalten Sie ein Android-Projekt mit einer Aktivität und einer Schaltfläche, die Sie zum Authentifizieren des Benutzers verwenden können.</span><span class="sxs-lookup"><span data-stu-id="927fd-125">This provides you with an Android project with an activity and a button that you can use to authenticate the user.</span></span>


## <a name="register-the-application"></a><span data-ttu-id="927fd-126">Registrieren der App</span><span class="sxs-lookup"><span data-stu-id="927fd-126">Register the application</span></span>

<span data-ttu-id="927fd-127">Sie müssen Ihre App im [Microsoft-App-Registrierungsportal](https://apps.dev.microsoft.com/) registrieren, unabhängig davon, ob Sie das Connect-Beispiel heruntergeladen oder ein neues Projekt erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="927fd-127">You need to register your app on the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) whether you've downloaded the connect sample or created a new project.</span></span>

<span data-ttu-id="927fd-p106">Registrieren Sie eine App im Microsoft-App-Registrierungsportal. Dadurch wird die App-ID generiert, mit der Sie die App konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="927fd-p106">Register an app on the Microsoft App Registration Portal. This generates the app ID that you'll use to configure the app.</span></span>

1. <span data-ttu-id="927fd-130">Melden Sie sich beim [Microsoft-App-Registrierungsportal](https://apps.dev.microsoft.com/) entweder mit Ihrem persönlichen oder geschäftlichen Konto oder mit Ihrem Schulkonto an.</span><span class="sxs-lookup"><span data-stu-id="927fd-130">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="927fd-131">Klicken Sie auf **App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="927fd-131">Choose **Add an app**.</span></span>

><span data-ttu-id="927fd-132">Tipp:  Wenn Sie das [Connect-Beispiel für Android](https://github.com/microsoftgraph/android-java-connect-sample) heruntergeladen haben und dieses lediglich registrieren möchten, deaktivieren Sie **Guided Setup**, bevor Sie auf die Schaltfläche **Create** klicken.</span><span class="sxs-lookup"><span data-stu-id="927fd-132">Tip: If you have downloaded the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) and are just creating a registration for it, uncheck **Guided Setup** before chosing the **Create** button.</span></span>

3. <span data-ttu-id="927fd-133">Geben Sie einen Namen für die App ein, und wählen Sie **Create**.</span><span class="sxs-lookup"><span data-stu-id="927fd-133">Enter a name for the app, and choose **Create**.</span></span> 
    
    <span data-ttu-id="927fd-134">Für den Fluss **Guided Setup**:</span><span class="sxs-lookup"><span data-stu-id="927fd-134">For the  **Guided Setup** flow:</span></span>
 
    <span data-ttu-id="927fd-p107">a. Wählen Sie **Mobile and Desktop App**, um den Typ der App zu definieren, die Sie erstellen.</span><span class="sxs-lookup"><span data-stu-id="927fd-p107">a. Choose **Mobile and Desktop App** to define the kind of app you are creating.</span></span>

    <span data-ttu-id="927fd-p108">b. Wählen Sie **Android**, um die verwendete Mobiltechnologie zu definieren.</span><span class="sxs-lookup"><span data-stu-id="927fd-p108">b. Choose **Android** to define the mobile technology you are using.</span></span>

    <span data-ttu-id="927fd-p109">c. Lesen Sie das einleitende Thema, und klicken Sie abschließend auf die Schaltfläche **Setup** am Ende der Seite.</span><span class="sxs-lookup"><span data-stu-id="927fd-p109">c. Review the introductory topic and when finished, click the **Setup** button at the end of the page.</span></span>

    <span data-ttu-id="927fd-p110">d. Befolgen Sie die Anweisungen im Schritt **Setup**, um die MSAL-Bibliothek zu Datei „build.gradle“ der App hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="927fd-p110">d. Follow the instructions on the **Setup** step to add the MSAL library to your app build.gradle.</span></span>

    <span data-ttu-id="927fd-p111">e. Befolgen Sie die Anweisungen im Schritt **Use**, um Ihrem neuen Projekt MSAL-Logik hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="927fd-p111">e. Follow the directions on the **Use** step to add MSAL logic to your new project</span></span>

    <span data-ttu-id="927fd-p112">f. Auf der Seite **Configure** hat das Portal eine eindeutige Anwendungs-ID für Sie erstellt. Verwenden Sie diese, um Ihre App zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="927fd-p112">f. On the **Configure** page, the portal has created a unique application ID for you. Use it to configure your app.</span></span>

    <span data-ttu-id="927fd-148">Für den Fluss ohne Anleitung:</span><span class="sxs-lookup"><span data-stu-id="927fd-148">For the unguided flow:</span></span>

    <span data-ttu-id="927fd-149">Die Registrierungsseite wird angezeigt, und die Eigenschaften der App werden aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="927fd-149">The registration page displays, listing the properties of your app.</span></span>

    <span data-ttu-id="927fd-p113">a. Kopieren Sie die Anwendungs-ID. Dies ist der eindeutige Bezeichner für Ihre App.</span><span class="sxs-lookup"><span data-stu-id="927fd-p113">a. Copy the application ID. This is the unique identifier for your app.</span></span> 

    <span data-ttu-id="927fd-p114">b. Wählen Sie **Plattform hinzufügen** und **Systemeigene Anwendung** aus.</span><span class="sxs-lookup"><span data-stu-id="927fd-p114">b. Choose **Add Platform** and **Native Application**.</span></span>

    > <span data-ttu-id="927fd-p115">**Hinweis:** Das App-Registrierungsportal stellt einen Umleitungs-URI mit dem Wert *msalYOUR NEW APP ID://auth* bereit. Verwenden Sie nicht die integrierten Umleitungs-URIs. Das [Connect-Beispiel für Android](https://github.com/microsoftgraph/android-java-connect-sample) implementiert die MSAL-Authentifizierungsbibliothek, die diesen Umleitungs-URI erfordert. Bei Verwendung einer [unterstützten Drittanbieterbibliothek](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-libraries#compatible-client-libraries) oder der **ADAL**-Bibliothek müssen Sie die integrierten Umleitungs-URIs verwenden.</span><span class="sxs-lookup"><span data-stu-id="927fd-p115">**Note:** The Application Registration Portal provides a Redirect URI with a value of *msalYOUR NEW APP ID://auth*. Do not use the built-in redirect URIs. The [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) implements the MSAL authentication library which requires this redirect URI. If using a [supported third party library](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-libraries#compatible-client-libraries) or the **ADAL** library then you must use the built-in redirect URIs.</span></span>

    <span data-ttu-id="927fd-158">Für den Fluss „Guided Setup“ und den Fluss ohne Anleitung</span><span class="sxs-lookup"><span data-stu-id="927fd-158">For Guided Setup flow and unguided flow</span></span>

    <span data-ttu-id="927fd-p116">a. Fügen Sie delegierte Berechtigungen hinzu. Sie benötigen die Berechtigungen **profile**, **Mail.ReadWrite**, **Mail.Send**, **Files.ReadWrite** und **User.ReadBasic.All**.</span><span class="sxs-lookup"><span data-stu-id="927fd-p116">a. Add delegated permissions. You'll need **profile**, **Mail.ReadWrite**, **Mail.Send**, **Files.ReadWrite**, and **User.ReadBasic.All**.</span></span> 
   
    <span data-ttu-id="927fd-p117">b. Wählen Sie **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="927fd-p117">b. Choose **Save**.</span></span>


## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="927fd-164">Authentifizierung des Benutzers und Abrufen eines Zugriffstokens</span><span class="sxs-lookup"><span data-stu-id="927fd-164">Authenticate the user and get an access token</span></span>

> <span data-ttu-id="927fd-p118">**Hinweis:** Wenn Sie die Anweisungen im Fluss **Guided Setup** des App-Registrierungsportals ausgeführt haben, um eine neue Anwendung zu erstellen, können Sie diese Schritte überspringen. Wechseln Sie zu [Aufrufen von Microsoft Graph mit dem Microsoft Graph-SDK](#call-microsoft-graph-using-the-microsoft-graph-sdk), um mehr über die Graph-API zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="927fd-p118">**Note:** If you followed the instructions in the **Guided Setup** flow from the application registration portal to create a new application, you can skip these steps. Go to [Call Microsoft Graph using the Microsoft Graph SDK](#call-microsoft-graph-using-the-microsoft-graph-sdk) to learn more about the Graph API.</span></span>

<span data-ttu-id="927fd-167">Wir wollen nun das [Connect-Beispiel für Android](https://github.com/microsoftgraph/android-java-connect-sample) durcharbeiten, um mehr über den MSAL- und Microsoft Graph-Code zu erfahren, den wir hinzugefügt haben.</span><span class="sxs-lookup"><span data-stu-id="927fd-167">Let's walk through the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) to learn about the MSAL and Microsoft Graph code we've added.</span></span>

### <a name="add-the-dependency-to-appbuildgradle"></a><span data-ttu-id="927fd-168">Hinzufügen der Abhängigkeit zu „app/build.gradle“</span><span class="sxs-lookup"><span data-stu-id="927fd-168">Add the dependency to app/build.gradle</span></span>

<span data-ttu-id="927fd-169">Öffnen Sie die Datei `build.gradle` im App-Modul, und suchen Sie nach der folgenden Abhängigkeit:</span><span class="sxs-lookup"><span data-stu-id="927fd-169">Open the `build.gradle` file in the app module and find the following dependency:</span></span>

```gradle
    compile ('com.microsoft.identity.client:msal:0.1.+') {
        exclude group: 'com.android.support', module: 'appcompat-v7'
    }
    compile 'com.android.volley:volley:1.0.0'

```

### <a name="start-the-authentication-flow"></a><span data-ttu-id="927fd-170">Starten des Authentifizierungsflusses</span><span class="sxs-lookup"><span data-stu-id="927fd-170">Start the authentication flow</span></span>

1. <span data-ttu-id="927fd-171">Öffnen Sie die Datei **AuthenticationManager**, und suchen Sie nach der Objektdeklaration **PublicClientApplication** und dann nach der Instantiierung der **getInstance**-Methode.</span><span class="sxs-lookup"><span data-stu-id="927fd-171">Open the **AuthenticationManager** file and find the **PublicClientApplication** object declaration and then the instation in the **getInstance** method.</span></span>

   ```java
    private static PublicClientApplication mPublicClientApplication;
    ....

    public static synchronized AuthenticationManager getInstance() {
        if (INSTANCE == null) {
            INSTANCE = new AuthenticationManager();
            if (mPublicClientApplication == null) {
                mPublicClientApplication = new PublicClientApplication(Connect.getInstance());
            }
        }
        return INSTANCE;
    }

   ```


2. <span data-ttu-id="927fd-p119">Suchen Sie in der Klasse **ConnectActivity** nach dem Ereignishandler für das Klick-Ereignis von **mConnectButton**. Suchen Sie die **OnClick**-Methode, und überprüfen Sie den relevanten Code.</span><span class="sxs-lookup"><span data-stu-id="927fd-p119">In the **ConnectActivity** class, locate the event handler for the click event of the **mConnectButton**. Find the **onClick** method and review relevant code.</span></span>
  
    <span data-ttu-id="927fd-p120">Die **connect**-Methode aktiviert die Protokollierung von personenbezogenen Informationen (PII), ruft eine Instanz der Beispiel-Hilfsklasse **CustomTargetNameDictionary** ab und ruft die Benutzersammlung des MSAL-Plattformobjekts ab. Wenn keine Benutzer vorhanden sind, wird der neue Benutzer zum Azure AD-Authentifizierungs- und Autorisierungsfluss geleitet. Andernfalls wird ein Authentifizierungstoken im Hintergrund abgerufen.</span><span class="sxs-lookup"><span data-stu-id="927fd-p120">The **connect** method enables personally identifyable information (PII) logging, gets an instance of the sample helper class **AuthenticationManager**, and gets the MSAL platform object users collection. If there are no users, the new user is taken to the Azure AD authentication and authorization flow. Otherwise, an authentication token is obtained silently.</span></span>

   ```java
    @Override
    public void onClick(View view) {
        ....
        connect();
    }

        private void connect() {

        if (mEnablePiiLogging) {
            Logger.getInstance().setEnablePII(true);
        } else {
            Logger.getInstance().setEnablePII(false);
        }

        AuthenticationManager mgr = AuthenticationManager.getInstance();

        List<User> users = null;

        try {
            users = mgr.getPublicClient().getUsers();

            if (users != null && users.size() == 1) {
                mUser = users.get(0);
                mgr.callAcquireTokenSilent(mUser, true, this);
            } else {
                mgr.callAcquireToken(
                        this,
                        this);
            }
        } catch (MsalClientException e) {
            Log.d(TAG, "MSAL Exception Generated while getting users: " + e.toString());

        } catch (IndexOutOfBoundsException e) {
            Log.d(TAG, "User at this position does not exist: " + e.toString());
        }
    }

   ```
3. <span data-ttu-id="927fd-p121">Suchen Sie den Ereignishandler, der die Azure AD-Umleitungsantwort verarbeitet, die von Azure AD generiert wird, wenn der Benutzer das Authentifizierungsdialogfeld schließt. Dieser Handler befindet sich in der Klasse **ConnectActivity**.</span><span class="sxs-lookup"><span data-stu-id="927fd-p121">Find the event handler that processes the Azure AD redirect response generated by Azure AD when the user closes the authintication dialog. This handler is in the **ConnectActivity** class.</span></span>

   ```java
       /**
     * Handles redirect response from https://login.microsoftonline.com/common and
     * notifies the MSAL library that the user has completed the authentication
     * dialog
     * @param requestCode
     * @param resultCode
     * @param data
     */
    @Override
    protected void onActivityResult(int requestCode, int resultCode, Intent data) {
        super.onActivityResult(requestCode, resultCode, data);
        if (AuthenticationManager
                .getInstance()
                .getPublicClient() != null) {
            AuthenticationManager
                    .getInstance()
                    .getPublicClient()
                    .handleInteractiveRequestRedirect(requestCode, resultCode, data);
        }
    }

   ```    
3. <span data-ttu-id="927fd-179">Suchen Sie die Rückrufmethode der Authentifizierung, die das Authentifizierungstoken zwischenspeichert, das in Aufrufen der Graph-API verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="927fd-179">Find the authentication callback method that caches the authentication token that is used in Graph API calls.</span></span>

 

```java
    /* Callback used for interactive request.  If succeeds we use the access
         * token to call the Microsoft Graph. Does not check cache
         */
    private AuthenticationCallback getAuthInteractiveCallback() {
        return new AuthenticationCallback() {
            @Override
            public void onSuccess(AuthenticationResult authenticationResult) {
            /* Successfully got a token, call graph now */
                Log.d(TAG, "Successfully authenticated");
                Log.d(TAG, "ID Token: " + authenticationResult.getIdToken());

            /* Store the auth result */
                mAuthResult = authenticationResult;
                if (mActivityCallback != null)
                    mActivityCallback.onSuccess(mAuthResult);
            }

            @Override
            public void onError(MsalException exception) {
            /* Failed to acquireToken */
                Log.d(TAG, "Authentication failed: " + exception.toString());
                if (mActivityCallback != null)
                    mActivityCallback.onError(exception);
            }

            @Override
            public void onCancel() {
            /* User canceled the authentication */
                Log.d(TAG, "User cancelled login.");
            }
        };
    }

```
    
<span data-ttu-id="927fd-p122">In der Hauptaktivität der Connect-Beispiel-App befindet sich eine Schaltfläche **Connect**. Wenn Sie zum ersten Mal auf die Schaltfläche klicken, wird in der App eine Authentifizierungsseite über den Browser des Geräts angezeigt. Der nächste Schritt besteht darin, den Code zu behandeln, den der Autorisierungsserver an den Umleitung-URI sendet, und diesen durch ein Zugriffstoken zu ersetzen.</span><span class="sxs-lookup"><span data-stu-id="927fd-p122">The connect sample app has a **Connect** button on the main activity. If you press the button, on first use, the app presents an authentication page using the device's browser. The next step is to handle the code that the authorization server sends to the redirect URI and exchange it for an access token.</span></span>

### <a name="exchange-the-authorization-code-for-an-access-token"></a><span data-ttu-id="927fd-183">Ersetzen des Autorisierungscodes durch ein Zugriffstoken</span><span class="sxs-lookup"><span data-stu-id="927fd-183">Exchange the authorization code for an access token</span></span>

<span data-ttu-id="927fd-184">Sie müssen Ihre App so vorbereiten, dass die Antwort des Autorisierungsservers verarbeitet wird, die einen Code enthält, der durch ein Zugriffstoken ersetzt werden kann.</span><span class="sxs-lookup"><span data-stu-id="927fd-184">You need to make your app ready to handle the authorization server response, which contains a code that you can exchange for an access token.</span></span>

1. <span data-ttu-id="927fd-p123">Wir müssen dem Android-System mitteilen, dass die Connect-App Anforderungen an den Umleitungs-URI verarbeiten kann, der bei der Registrierung der Anwendung konfiguriert wurde. Öffnen Sie hierzu die Datei **AndroidManifest**, und fügen sie dem Element **\<application/\>** des Projekts die folgenden untergeordneten Elemente hinzu.</span><span class="sxs-lookup"><span data-stu-id="927fd-p123">We need to tell the Android system that Connect app can handle requests to the redirect URL configured in the application registration. To do this open the **AndroidManifest** file and add the following children to the projects  **\<application/\>** element.</span></span>
    ```xml
        <uses-sdk tools:overrideLibrary="com.microsoft.identity.msal" />
        <application ...>
            ...
            <activity
                android:name="com.microsoft.identity.client.BrowserTabActivity">
                <intent-filter>
                    <action android:name="android.intent.action.VIEW" />
                    <category android:name="android.intent.category.DEFAULT" />
                    <category android:name="android.intent.category.BROWSABLE" />
                    <data android:scheme="msalENTER_YOUR_CLIENT_ID"
                        android:host="auth" />
                </intent-filter>
            </activity>
            <meta-data
                android:name="https://login.microsoftonline.com/common"
                android:value="authority string"/>
            <meta-data
                android:name="com.microsoft.identity.client.ClientId"
                android:value="ENTER_YOUR_CLIENT_ID"/>
        </application>
    ```
2. <span data-ttu-id="927fd-p124">Die **MSAL**-Bibliothek benötigt Zugriff auf die vom Registrierungsportal zugewiesene Anwendungs-ID. **Die MSAL-Bibliothek bezeichnet die Anwendungs-ID als „Client-ID“**. Sie ruft die Anwendungs-ID (Client-ID) aus dem Anwendungskontext ab, den Sie im Bibliothekskonstruktor übergeben.</span><span class="sxs-lookup"><span data-stu-id="927fd-p124">The **MSAL** library needs access to the application Id assigned by the registration portal. **The MSAL library refers to the application Id as the "Client Id"**. It gets the application Id (Client Id) from the application context that you pass in the library constructor.</span></span> 

   ><span data-ttu-id="927fd-190">Hinweis: Sie können die Client-ID auch zur Laufzeit angeben, indem Sie einen Zeichenfolgeparameter an den Konstruktor übergeben.</span><span class="sxs-lookup"><span data-stu-id="927fd-190">Note: You can also provide the client Id at run-time by passing a string parameter to the constructor.</span></span> 

3. <span data-ttu-id="927fd-p125">Die Aktivität wird aufgerufen, wenn der Autorisierungsserver eine Antwort sendet. Fordern Sie ein Zugriffstoken mit der Antwort vom Autorisierungsserver an. Wechseln Sie zur Klasse **AuthenticationManager**, und suchen Sie den folgenden Code.</span><span class="sxs-lookup"><span data-stu-id="927fd-p125">The activity is invoked when the authorization server sends a response. Request an access token with the response from the authorization server. Go to your **AuthenticationManager** and find the following code in the class.</span></span>

   ```java
    /**
     * Authenticates the user and lets the user authorize the app for the requested permissions.
     * An authentication token is returned via the getAuthInteractiveCalback method
     * @param activity
     * @param authenticationCallback
     */
    public void connect(Activity activity, final MSALAuthenticationCallback authenticationCallback){
        mActivityCallback = authenticationCallback;
        mPublicClientApplication.acquireToken(
                activity, Constants.SCOPES, getAuthInteractiveCallback());
    }


     /* Callback used for interactive request.  If succeeds we use the access
         * token to call the Microsoft Graph. Does not check cache
         */
    private AuthenticationCallback getAuthInteractiveCallback() {
        return new AuthenticationCallback() {
            @Override
            public void onSuccess(AuthenticationResult authenticationResult) {
            /* Successfully got a token, call graph now */
                Log.d(TAG, "Successfully authenticated");
                Log.d(TAG, "ID Token: " + authenticationResult.getIdToken());

            /* Store the auth result */
                mAuthResult = authenticationResult;
                if (mActivityCallback != null)
                    mActivityCallback.onSuccess(mAuthResult);
            }

            @Override
            public void onError(MsalException exception) {
            /* Failed to acquireToken */
                Log.d(TAG, "Authentication failed: " + exception.toString());
                if (mActivityCallback != null)
                    mActivityCallback.onError(exception);
            }

            @Override
            public void onCancel() {
            /* User canceled the authentication */
                Log.d(TAG, "User cancelled login.");
            }
        };
    }

     /**
     * Returns the access token obtained in authentication
     *
     * @return mAccessToken
     */
    public String getAccessToken() throws AuthenticatorException, IOException, OperationCanceledException {
        return  mAuthResult.getAccessToken();
    }

   ```


## <a name="call-microsoft-graph"></a><span data-ttu-id="927fd-194">Aufrufen von Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="927fd-194">Call Microsoft Graph</span></span>
<span data-ttu-id="927fd-195">Zum Aufrufen von Microsoft Graph können Sie [das Microsoft Graph-SDK](#call-microsoft-graph-using-the-microsoft-graph-sdk) oder die [Microsoft Graph-REST-API](#call-microsoft-graph-using-the-microsoft-graph-rest-api) verwenden.</span><span class="sxs-lookup"><span data-stu-id="927fd-195">You can [use the Microsoft Graph SDK](#call-microsoft-graph-using-the-microsoft-graph-sdk) or the [Microsoft Graph REST API](#call-microsoft-graph-using-the-microsoft-graph-rest-api) to call Microsoft Graph.</span></span>

### <a name="call-microsoft-graph-using-the-microsoft-graph-sdk"></a><span data-ttu-id="927fd-196">Aufrufen von Microsoft Graph mit dem Microsoft Graph-SDK</span><span class="sxs-lookup"><span data-stu-id="927fd-196">Call Microsoft Graph using the Microsoft Graph SDK</span></span>
<span data-ttu-id="927fd-p126">Das [Microsoft Graph-SDK für Android](https://github.com/microsoftgraph/msgraph-sdk-android) stellt Klassen bereit, aus denen Anforderungen und Prozessergebnisse aus Microsoft Graph erstellt werden. Führen Sie die folgenden Schritte aus, um das Microsoft Graph-SDK zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="927fd-p126">The [Microsoft Graph SDK for Android](https://github.com/microsoftgraph/msgraph-sdk-android) provides classes that build requests and process results from Microsoft Graph. Follow these steps to use the Microsoft Graph SDK.</span></span>

1. <span data-ttu-id="927fd-p127">Gewähren Sie Ihrer Anwendung entsprechende Internetberechtigungen. Öffnen Sie die Datei **AndroidManifest**, und fügen Sie das folgende untergeordnete Element zum Manifest hinzu.</span><span class="sxs-lookup"><span data-stu-id="927fd-p127">Add Internet permissions to your app. Open the **AndroidManifest** file and add the following child to the manifest element.</span></span>
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
    <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />

    ```

2. <span data-ttu-id="927fd-201">Fügen Sie Abhängigkeiten zum Microsoft Graph-SDK und zu GSON hinzu.</span><span class="sxs-lookup"><span data-stu-id="927fd-201">Add dependencies to the Microsoft Graph SDK and GSON.</span></span>
   ```gradle
    compile 'com.microsoft.graph:msgraph-sdk-android:1.3.2'
    compile 'com.google.code.gson:gson:2.7'
   ```


3. <span data-ttu-id="927fd-p128">Verwenden Sie die Hilfsmethode **authenticateRequest**, um Authentifizierungstoken zu neuen Anforderungen hinzuzufügen. Diese Methode implementiert die gleiche Methode aus der Microsoft Graph-Authentifizierungsoberfläche **IAuthenticationProvider**.</span><span class="sxs-lookup"><span data-stu-id="927fd-p128">Add authentication token to new requests using the **uthenticateRequest** helper method. This method implements the same method from the Microsoft Graph Authentication **IAuthenticationProvider** interface</span></span>
    
   ```java
    /**
     * Appends an access token obtained from the {@link AuthenticationManager} class to the
     * Authorization header of the request.
     * @param request
     */
    @Override
    public void authenticateRequest(IHttpRequest request)  {
        try {
            request.addHeader("Authorization", "Bearer "
                    + AuthenticationManager.getInstance()
                    .getAccessToken());
            // This header has been added to identify this sample in the Microsoft Graph service.
            // If you're using this code for your project please remove the following line.
            request.addHeader("SampleID", "android-java-connect-sample");
        } catch (AuthenticatorException e) {
            e.printStackTrace();
        } catch (IOException e) {
            e.printStackTrace();
        }  catch (OperationCanceledException e) {
            e.printStackTrace();
        } catch (NullPointerException e) {
            e.printStackTrace();
        }
    }
   ```

4. <span data-ttu-id="927fd-204">Erstellen Sie einen E-Mail-Entwurf, und senden Sie ihn mit den folgenden Hilfsmethoden aus der Hilfsklasse **GraphServiceController**.</span><span class="sxs-lookup"><span data-stu-id="927fd-204">Create a draft email and send it using the following helper methods from the **GraphServiceController** helper class.</span></span>

   ```java
    /**
     * Creates a draft email message using the Microsoft Graph API on Office 365. The mail is sent
     * from the address of the signed in user.
     *
     * @param senderPreferredName The mail senders principal user name (email addr)
     * @param emailAddress        The recipient email address.
     * @param subject             The subject to use in the mail message.
     * @param body                The body of the message.
     * @param callback            The callback method to invoke on completion of the POST request
     */
    public void createDraftMail(
            final String senderPreferredName,
            final String emailAddress,
            final String subject,
            final String body,
            ICallback<Message> callback
    ) {
        try {
            // create the email message
            Message message = createMessage(subject, body, emailAddress);
            mGraphServiceClient
                    .getMe()
                    .getMessages()
                    .buildRequest()
                    .post(message, callback);

        } catch (Exception ex) {
            showException(ex, "exception on send mail","Send mail failed", "The send mail method failed");
        }
    }

        /**
     * Creates a new Message object 
     */
    Message createMessage(
            String subject,
            String body,
            String address) {

        if (address == null || address.isEmpty()) {
            throw new IllegalArgumentException("The address parameter can't be null or empty.");
        } else {
            // perform a simple validation of the email address
            String addressParts[] = address.split("@");
            if (addressParts.length != 2 || addressParts[0].length() == 0 || addressParts[1].indexOf('.') == -1) {
                throw new IllegalArgumentException(
                        String.format("The address parameter must be a valid email address {0}", address)
                );
            }
        }
        Message message = new Message();
        EmailAddress emailAddress = new EmailAddress();
        emailAddress.address = address;
        Recipient recipient = new Recipient();
        recipient.emailAddress = emailAddress;
        message.toRecipients = Collections.singletonList(recipient);
        ItemBody itemBody = new ItemBody();
        itemBody.content = body;
        itemBody.contentType = BodyType.html;
        message.body = itemBody;
        message.subject = subject;
        return message;
    }
    /**
     * Sends a draft message to the specified recipients
     *
     * @param messageId String. The id of the message to send
     * @param callback
     */
    public void sendDraftMessage(String messageId,
                                 ICallback<Void> callback) {
        try {

            mGraphServiceClient
                    .getMe()
                    .getMessages(messageId)
                    .getSend()
                    .buildRequest()
                    .post(callback);

        } catch (Exception ex) {
            showException(ex, "exception on send draft message ","Send draft mail failed", "The send draft mail method failed");
        }
    }

   ```
### <a name="call-microsoft-graph-using-the-microsoft-graph-rest-api"></a><span data-ttu-id="927fd-205">Aufrufen von Microsoft Graph mit der Microsoft Graph-REST-API</span><span class="sxs-lookup"><span data-stu-id="927fd-205">Call Microsoft Graph using the Microsoft Graph REST API</span></span>
<span data-ttu-id="927fd-p129">Die [Microsoft Graph-REST-API](http://developer.microsoft.com/en-us/graph/docs) macht mehrere APIs aus Microsoft-Clouddiensten über einen einzelnen REST-API-Endpunkt verfügbar. Gehen Sie folgendermaßen vor, um die REST-API zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="927fd-p129">The [Microsoft Graph REST API](http://developer.microsoft.com/en-us/graph/docs) exposes multiple APIs from Microsoft cloud services through a single REST API endpoint. Follow these steps to use the REST API.</span></span>

1. <span data-ttu-id="927fd-p130">Gewähren Sie Ihrer Anwendung entsprechende Internetberechtigungen. Öffnen Sie die Datei **AndroidManifest**, und fügen Sie das folgende untergeordnete Element zum Manifest hinzu.</span><span class="sxs-lookup"><span data-stu-id="927fd-p130">Add Internet permissions to your app. Open the **AndroidManifest** file and add the following child to the manifest element.</span></span>
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    ```

2. <span data-ttu-id="927fd-210">Fügen Sie der Volley HTTP-Bibliothek eine Abhängigkeit hinzu.</span><span class="sxs-lookup"><span data-stu-id="927fd-210">Add a dependency to the Volley HTTP library.</span></span>

    ```gradle
    compile 'com.android.volley:volley:1.0.0'
    ```
   
3. <span data-ttu-id="927fd-p131">Ersetzen Sie die Zeile `String accessToken = tokenResponse.accessToken;` durch den folgenden Code. Fügen Sie Ihre E-Mail-Adresse in den Platzhalter ein, der mit **\<YOUR_EMAIL_ADDRESS\>** markiert ist.</span><span class="sxs-lookup"><span data-stu-id="927fd-p131">Replace the line `String accessToken = tokenResponse.accessToken;` with the following code. Insert your email address in the placeholder marked with **\<YOUR_EMAIL_ADDRESS\>**.</span></span>
   ```java
    final String accessToken = tokenResponse.accessToken;

    final RequestQueue queue = Volley.newRequestQueue(getApplicationContext());
    String url ="https://graph.microsoft.com/v1.0/me/sendMail";
    final String body = "{" +
        "  Message: {" +
        "    subject: 'Sent using the Microsoft Graph REST API'," +
        "    body: {" +
        "      contentType: 'text'," +
        "      content: 'This is the email body'" +
        "    }," +
        "    toRecipients: [" +
        "      {" +
        "        emailAddress: {" +
        "          address: '<YOUR_EMAIL_ADDRESS>'" +
        "        }" +
        "      }" +
        "    ]}" +
        "}";

    final StringRequest stringRequest = new StringRequest(Request.Method.POST, url,
        new Response.Listener<String>() {
            @Override
            public void onResponse(String response) {
                Log.d("Response", response);
            }
        },
        new Response.ErrorListener() {
            @Override
            public void onErrorResponse(VolleyError error) {
                Log.d("ERROR","error => " + error.getMessage());
            }
        }
    ) {
        @Override
        public Map<String, String> getHeaders() throws AuthFailureError {
            Map<String,String> params = new HashMap<>();
            params.put("Authorization", "Bearer " + accessToken);
            params.put("Content-Length", String.valueOf(body.getBytes().length));
            return params;
        }
        @Override
        public String getBodyContentType() {
            return "application/json";
        }
        @Override
        public byte[] getBody() throws AuthFailureError {
            return body.getBytes();
        }
    };

    AsyncTask.execute(new Runnable() {
        @Override
        public void run() {
            queue.add(stringRequest);
        }
    });
   ```

## <a name="run-the-app"></a><span data-ttu-id="927fd-213">Ausführen der App</span><span class="sxs-lookup"><span data-stu-id="927fd-213">Run the app</span></span>
<span data-ttu-id="927fd-214">Sie können Ihre Android-App nun testen.</span><span class="sxs-lookup"><span data-stu-id="927fd-214">You're ready to try your Android app.</span></span>

1. <span data-ttu-id="927fd-215">Starten Sie Ihren Android-Emulator, oder schließen Sie das Gerät an Ihren Computer an.</span><span class="sxs-lookup"><span data-stu-id="927fd-215">Start your Android emulator or connect your physical device to your computer.</span></span>
2. <span data-ttu-id="927fd-216">Drücken Sie in Android Studio UMSCHALT+F10, um die App auszuführen.</span><span class="sxs-lookup"><span data-stu-id="927fd-216">In Android Studio, press Shift + F10 to run your app.</span></span>
3. <span data-ttu-id="927fd-217">Wählen Sie im Dialogfeld für die Bereitstellung Ihren Android-Emulator oder das Android-Gerät aus.</span><span class="sxs-lookup"><span data-stu-id="927fd-217">Choose your Android emulator or device from the deployment dialog box.</span></span>
4. <span data-ttu-id="927fd-218">Tippen Sie in der Hauptaktivität auf die Floating-Action-Button.</span><span class="sxs-lookup"><span data-stu-id="927fd-218">Tap the Floating Action Button on the main activity.</span></span>
5. <span data-ttu-id="927fd-219">Melden Sie sich mit Ihrem persönlichen Konto oder mit Ihrem Geschäfts- oder Schulkonto an, und gewähren Sie die erforderlichen Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="927fd-219">Sign in with your personal or work or school account and grant the requested permissions.</span></span>
6. <span data-ttu-id="927fd-220">Tippen Sie im App-Auswahldialogfeld auf die App, um fortzufahren.</span><span class="sxs-lookup"><span data-stu-id="927fd-220">In the app selection dialog, tap your app to continue.</span></span>

<span data-ttu-id="927fd-p132">Überprüfen Sie den Posteingang der E-Mail-Adresse, die Sie im Abschnitt [Aufrufen von Microsoft Graph](#call-microsoft-graph) konfiguriert haben. Dort sollten Sie eine E-Mail von dem Konto vorfinden, das Sie zum Anmelden bei der App verwendet haben.</span><span class="sxs-lookup"><span data-stu-id="927fd-p132">Check the inbox of the email address that you configured in [Call Microsoft Graph](#call-microsoft-graph). You should have an email from the account that you used to sign in to the app.</span></span>

## <a name="next-steps"></a><span data-ttu-id="927fd-223">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="927fd-223">Next steps</span></span>
- <span data-ttu-id="927fd-224">Testen Sie den [Microsoft Graph-Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="927fd-224">Try out the [Microsoft Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="927fd-225">Beispiele für allgemeine Vorgänge finden Sie im [Codeausschnittbeispiel für Android](https://github.com/microsoftgraph/android-java-snippets-sample). Sie können auch unsere anderen [Android-Beispiele](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=android) auf GitHub erkunden.</span><span class="sxs-lookup"><span data-stu-id="927fd-225">Find examples of common operations in the [Snippets Sample for Android](https://github.com/microsoftgraph/android-java-snippets-sample), or explore our other [Android samples](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=android) on GitHub.</span></span>


## <a name="see-also"></a><span data-ttu-id="927fd-226">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="927fd-226">See also</span></span>
- [<span data-ttu-id="927fd-227">Microsoft Graph-SDK für Android</span><span class="sxs-lookup"><span data-stu-id="927fd-227">Microsoft Graph SDK for Android</span></span>](https://github.com/microsoftgraph/msgraph-sdk-android) 
- [<span data-ttu-id="927fd-228">Abrufen von Zugriffstoken zum Aufrufen von Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="927fd-228">Get access tokens to call Microsoft Graph</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [<span data-ttu-id="927fd-229">Im Namen eines Benutzers zugreifen</span><span class="sxs-lookup"><span data-stu-id="927fd-229">Get access on behalf of a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [<span data-ttu-id="927fd-230">Ohne Benutzer zugreifen</span><span class="sxs-lookup"><span data-stu-id="927fd-230">Get access without a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)
