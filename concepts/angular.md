# <a name="get-started-with-microsoft-graph-in-an-angularjs-app"></a><span data-ttu-id="f65be-101">Erste Schritte mit Microsoft Graph in einer Angular JS-App</span><span class="sxs-lookup"><span data-stu-id="f65be-101">Get started with Microsoft Graph in an AngularJS app</span></span>

<span data-ttu-id="f65be-p101">Dieser Artikel beschreibt die erforderlichen Aufgaben zum Abrufen eines Zugriffstokens vom Azure AD v2.0-Endpunkt und zum Aufrufen von Microsoft Graph. Sie werden durch die Erstellung des [Microsoft Connect-Beispiels für Angular JS](https://github.com/microsoftgraph/angular-connect-rest-sample) geführt und erhalten Informationen zu den Hauptkonzepten, die Sie zur Verwendung von Microsoft Graph implementieren. In diesem Artikel wird auch beschrieben, wie Sie mithilfe des [Microsoft Graph-SDKs für JavaScript](https://github.com/microsoftgraph/msgraph-sdk-javascript) oder reinen REST-Aufrufen auf Microsoft Graph zugreifen.</span><span class="sxs-lookup"><span data-stu-id="f65be-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Microsoft Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample) and explains the main concepts that you implement to use Microsoft Graph. The article also describes how to access Microsoft Graph by using either the [Microsoft Graph JavaScript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) or raw REST calls.</span></span>

<span data-ttu-id="f65be-105">In der folgenden Abbildung ist die App dargestellt, die Sie erstellen.</span><span class="sxs-lookup"><span data-stu-id="f65be-105">The following image shows the app you'll create.</span></span> 

![Die Web-App nach der Anmeldung mit der Schaltfläche „E-Mail senden“](./images/angular-connect-sample.png)


<span data-ttu-id="f65be-p102">**Sie möchten keine App erstellen?** Verwenden Sie für einen schnellen Einstieg den [Schnellstart Microsoft Graph](https://graph.microsoft.io/de-DE/getting-started).</span><span class="sxs-lookup"><span data-stu-id="f65be-p102">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/de-DE/getting-started) to get up and running fast.</span></span>

<span data-ttu-id="f65be-109">Zum Herunterladen einer Version des Connect-Beispiels, das den Endpunkt Azure AD verwendet, siehe [Microsoft Graph Connect-Beispiel für Angular JS](https://github.com/microsoftgraph/angular-connect-rest-sample/releases/tag/last_v1_auth).</span><span class="sxs-lookup"><span data-stu-id="f65be-109">To download a version of the Connect sample that uses the Azure AD endpoint, see [Microsoft Graph Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample/releases/tag/last_v1_auth).</span></span>


## <a name="prerequisites"></a><span data-ttu-id="f65be-110">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f65be-110">Prerequisites</span></span>

<span data-ttu-id="f65be-111">Für die ersten Schritte benötigen Sie:</span><span class="sxs-lookup"><span data-stu-id="f65be-111">To get started, you'll need:</span></span> 

- <span data-ttu-id="f65be-112">Ein [Microsoft-Konto](https://www.outlook.com/) oder ein [Geschäfts- oder Schulkonto](https://docs.microsoft.com/de-DE/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="f65be-112">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/de-DE/office/developer-program/office-365-developer-program-faq#account-types)</span></span>
- [<span data-ttu-id="f65be-113">Node.js with npm</span><span class="sxs-lookup"><span data-stu-id="f65be-113">Node.js with npm</span></span>](https://nodejs.org/en/download/)
- [<span data-ttu-id="f65be-114">Bower</span><span class="sxs-lookup"><span data-stu-id="f65be-114">Bower</span></span>](https://bower.io)
- <span data-ttu-id="f65be-p103">Das [Microsoft Connect-Beispiel für AngularJS](https://github.com/microsoftgraph/angular-connect-sample). Für diese exemplarische Vorgehensweise verwenden Sie den Ordner **Startprojekt** in den Beispieldateien.</span><span class="sxs-lookup"><span data-stu-id="f65be-p103">The [Microsoft Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-sample). You'll use the **starter-project** folder in the sample files for this walkthrough.</span></span>

## <a name="register-the-application"></a><span data-ttu-id="f65be-117">Registrieren der App</span><span class="sxs-lookup"><span data-stu-id="f65be-117">Register the application</span></span>
<span data-ttu-id="f65be-p104">Registrieren Sie eine App im Microsoft App-Registrierungsportal. Dadurch werden die APP-ID und das Kennwort generiert, mit der bzw. dem Sie die App in Visual Studio konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="f65be-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app in Visual Studio.</span></span>

1. <span data-ttu-id="f65be-120">Melden Sie sich beim [Microsoft-App-Registrierungsportal](https://apps.dev.microsoft.com/) entweder mit Ihrem persönlichen oder geschäftlichen Konto oder mit Ihrem Schulkonto an.</span><span class="sxs-lookup"><span data-stu-id="f65be-120">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="f65be-121">Klicken Sie auf **App hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="f65be-121">Choose **Add an app**.</span></span>

3. <span data-ttu-id="f65be-122">Geben Sie einen Namen für die App ein, und wählen Sie **Anwendung erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="f65be-122">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="f65be-123">Die Registrierungsseite wird angezeigt, und die Eigenschaften der App werden aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="f65be-123">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="f65be-p105">Kopieren Sie die Anwendungs-ID: Hierbei handelt es sich um einen eindeutigen Bezeichner, die Sie für die Konfiguration der App verwenden werden.</span><span class="sxs-lookup"><span data-stu-id="f65be-p105">Copy the application ID. This is the unique identifier for your app that you'll use to configure the app.</span></span>

5. <span data-ttu-id="f65be-126">Wählen Sie unter **Plattformen** die Option **Plattform hinzufügen** > **Web** aus.</span><span class="sxs-lookup"><span data-stu-id="f65be-126">Under **Platforms**, choose **Add Platform** > **Web**.</span></span>

6. <span data-ttu-id="f65be-127">Vergewissern Sie sich, dass das Kontrollkästchen **Impliziten Fluss zulassen** aktiviert ist, und geben Sie als Umleitungs-URI *http://localhost:8080* ein.</span><span class="sxs-lookup"><span data-stu-id="f65be-127">Make sure the Allow Implicit Flow check box is selected, and enter http://localhost:8080 as the Redirect URI.</span></span> 

7. <span data-ttu-id="f65be-128">Wählen Sie **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="f65be-128">Choose **Save**.</span></span>


## <a name="configure-the-project"></a><span data-ttu-id="f65be-129">Konfigurieren des Projekts</span><span class="sxs-lookup"><span data-stu-id="f65be-129">Configure the project</span></span>
1. <span data-ttu-id="f65be-130">Öffnen Sie den Ordner **Startprojekt** in den Beispieldateien.</span><span class="sxs-lookup"><span data-stu-id="f65be-130">Open the **starter-project** folder in the sample files.</span></span>
2. <span data-ttu-id="f65be-p106">Führen Sie die folgenden Befehle in einem Eingabeaufforderungsfenster im Stammverzeichnis des Startprojekts aus. Dadurch werden die Projekt-Abhängigkeiten installiert.</span><span class="sxs-lookup"><span data-stu-id="f65be-p106">In a command prompt, run the following commands in the root directory of the starter project. This installs the project dependencies.</span></span>

        npm install  
        bower install
    
3. <span data-ttu-id="f65be-133">Öffnen Sie in den Startprojektdateien im Ordner **Öffentlich/Skripts** config.js.</span><span class="sxs-lookup"><span data-stu-id="f65be-133">In the starter project files, in the **public/scripts** folder, open config.js.</span></span>
4. <span data-ttu-id="f65be-134">Ersetzen Sie im Feld **Client-ID** den Platzhalterwert **ENTER_YOUR_CLIENT_ID** durch die Anwendungs-ID, die Sie gerade kopiert haben.</span><span class="sxs-lookup"><span data-stu-id="f65be-134">In the **clientID** field, replace the **ENTER_YOUR_CLIENT_ID** placeholder value with the application ID you just copied.</span></span>

## <a name="call-microsoft-graph-with-the-sdk"></a><span data-ttu-id="f65be-135">Aufrufen von Microsoft Graph mit dem SDK</span><span class="sxs-lookup"><span data-stu-id="f65be-135">Call Microsoft Graph with the SDK</span></span>
<span data-ttu-id="f65be-p107">Die App ruft Microsoft Graph auf, um Benutzerinformationen abzurufen und eine E-Mail-Nachricht im Auftrag des Benutzers zu senden. Diese Anrufe werden vom Maincontroller als Antwort auf UI-Ereignisse initiiert.</span><span class="sxs-lookup"><span data-stu-id="f65be-p107">The app calls Microsoft Graph to get user information and to send an email on the user's behalf. These calls are initiated from the MainController in response to UI events.</span></span>

<span data-ttu-id="f65be-p108">Öffnen Sie „app.js“, und fügen Sie den folgenden Code an das Ende der Datei an. Dadurch wird das SDK initialisiert.</span><span class="sxs-lookup"><span data-stu-id="f65be-p108">Open app.js and add the following code to the bottom of the file. This initializes the SDK.</span></span>

    var authToken;
    var graphClient = MicrosoftGraph.Client.init({
        authProvider: function(done) {
        if (typeof authToken === "undefined") {
          done({err: "No auth token"})
        } else {
          done(null, authToken); //first parameter takes an error if you can't get an access token
        }
        }
    });

### <a name="using-the-sdk"></a><span data-ttu-id="f65be-140">Verwenden des SDK</span><span class="sxs-lookup"><span data-stu-id="f65be-140">Using the SDK</span></span>
1. <span data-ttu-id="f65be-p109">Ersetzen Sie in „graphHelper.js“ *//Profil des aktuellen Benutzers abrufen* durch folgenden Code. Dadurch wird die GET-Anforderung konfiguriert und an den Endpunkt */me* gesendet und die Antwort verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="f65be-p109">In graphHelper.js, replace *// Get the profile of the current user* with the following code. This configures and sends the GET request to the */me* endpoint, and processes the response.</span></span>

        // Get the profile of the current user.
        me: function me() {
          return graphClient.api('/me').get();
        },
  
2. <span data-ttu-id="f65be-p110">Ersetzen Sie *//Eine E-Mail im Namen des aktuellen Benutzers senden* durch folgenden Code. Dadurch wird die POST-Anforderung konfiguriert und an den Endpunkt */me/sendMail* gesendet und die Antwort verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="f65be-p110">Replace *// Send an email on behalf of the current user* with the following code. This configures and sends the POST request to the */me/sendMail* endpoint, and processes the response.</span></span>

        // Send an email on behalf of the current user.
        sendMail: function sendMail(email) {
          return graphClient.api('/me/sendMail').post({ 'message' : email, 'saveToSentItems': true });
        }

3. <span data-ttu-id="f65be-145">Öffnen Sie im Ordner **Öffentlich/Controller** „mainController.js“.</span><span class="sxs-lookup"><span data-stu-id="f65be-145">In the **public/controllers** folder, open mainController.js.</span></span>

4. <span data-ttu-id="f65be-p111">Ersetzen Sie *//Standard-Header und Benutzereigenschaften festlegen* durch folgenden Code. Dadurch wird das Zugriffstoken zu der HTTP-Anforderung hinzugefügt, das Profil des aktuellen Benutzers von **GraphHelper.me** abgerufen und die Antwort verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="f65be-p111">Replace *// Set the default headers and user properties* with the following code. This adds the access token to the HTTP request, calls **GraphHelper.me** to get the current user's profile, and processes the response.</span></span>

        // Set the default headers and user properties.
        function processAuth() {

        // let the authProvider access the access token
        authToken = localStorage.token;

        if (localStorage.getItem('user') === null) {

          // Get the profile of the current user.
          GraphHelper.me().then(function(user) {

            // Save the user to localStorage.
            localStorage.setItem('user', angular.toJson(user));

            vm.displayName = user.displayName;
            vm.emailAddress = user.mail || user.userPrincipalName;
          });
        } else {
          let user = angular.fromJson(localStorage.user);

          vm.displayName = user.displayName;
          vm.emailAddress = user.mail || user.userPrincipalName;
        }

        }

5. <span data-ttu-id="f65be-p112">Ersetzen Sie *//Eine E-Mail im Namen des aktuellen Benutzers senden* durch folgenden Code. Dadurch wird die E-Mail-Nachricht erstellt , **GraphHelper.sendMail** aufgerufen und die Antwort verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="f65be-p112">Replace *// Send an email on behalf of the current user* with the following code. This builds the email message, calls **GraphHelper.sendMail**, and processes the response.</span></span>

        // Send an email on behalf of the current user.
        function sendMail() {

          authToken = localStorage.token;       

          // Build the HTTP request payload (the Message object).
          var email = {
          Subject: 'Welcome to Microsoft Graph development with Angular and the Microsoft Graph Connect sample',
          Body: {
            ContentType: 'HTML',
            Content: getEmailContent()
          },
          ToRecipients: [
            {
              EmailAddress: {
            Address: vm.emailAddress
              }
            }
          ]
          };

          // Save email address so it doesn't get lost with two way data binding.
          vm.emailAddressSent = vm.emailAddress;
          GraphHelper.sendMail(email)
        .then(function (response) {
          $log.debug('HTTP request to the Microsoft Graph API returned successfully.', response);
          vm.requestSuccess = true;
          vm.requestFinished = true;
          $scope.$apply();
        }, function (error) {
          $log.error('HTTP request to the Microsoft Graph API failed.');
          vm.requestSuccess = false;
          vm.requestFinished = true;
          $scope.$apply();
        });

        };

6. <span data-ttu-id="f65be-150">Speichern Sie all Ihre Änderungen.</span><span class="sxs-lookup"><span data-stu-id="f65be-150">Save all your changes.</span></span>

## <a name="run-the-app"></a><span data-ttu-id="f65be-151">Ausführen der App</span><span class="sxs-lookup"><span data-stu-id="f65be-151">Run the app</span></span>

1. <span data-ttu-id="f65be-152">Führen Sie den folgenden Befehl in einem Eingabeaufforderungsfenster im Stammverzeichnis des Startprojekts aus.</span><span class="sxs-lookup"><span data-stu-id="f65be-152">In a command prompt, run the following command in the root directory of the starter project.</span></span>

        npm start

2. <span data-ttu-id="f65be-153">Navigieren Sie in einem Browser zu *http://localhost:8080*, und wählen Sie die Schaltfläche **Verbinden** aus.</span><span class="sxs-lookup"><span data-stu-id="f65be-153">In a browser, navigate to http://localhost:8080 and choose the Connect button.</span></span>

3. <span data-ttu-id="f65be-154">Melden Sie sich an, und erteilen Sie die erforderlichen Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="f65be-154">Sign in and grant the requested permissions.</span></span> 

4. <span data-ttu-id="f65be-p113">Optional können Sie die E-Mail-Adresse des Empfängers bearbeiten. Klicken Sie dann auf die Schaltfläche **E-Mail senden**. Nachdem die E-Mail gesendet wurde, wird unter der Schaltfläche eine Erfolgsmeldung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f65be-p113">Optionally edit the recipient's email address, and then choose the **Send mail** button. When the mail is sent, a Success message is displayed below the button.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="f65be-157">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="f65be-157">Next steps</span></span>
- <span data-ttu-id="f65be-158">Testen Sie die REST-API mithilfe des [Graph-Explorers](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="f65be-158">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="f65be-159">Weitere [AngularJS-Proben](https://github.com/search?utf8=%E2%9C%93&q=angular+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) finden Sie auf GitHub.</span><span class="sxs-lookup"><span data-stu-id="f65be-159">Explore our other [AngularJS samples](https://github.com/search?utf8=%E2%9C%93&q=angular+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) on GitHub.</span></span>


## <a name="see-also"></a><span data-ttu-id="f65be-160">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="f65be-160">See also</span></span>
- [<span data-ttu-id="f65be-161">Azure AD v2.0-Protokolle</span><span class="sxs-lookup"><span data-stu-id="f65be-161">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="f65be-162">Azure AD v2.0-Tokens</span><span class="sxs-lookup"><span data-stu-id="f65be-162">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-v2-tokens/)
