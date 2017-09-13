# <a name="getting-started-building-microsoft-graph-apps"></a><span data-ttu-id="92d0f-101">Erste Schritte zum Entwickeln von Microsoft Graph-Apps</span><span class="sxs-lookup"><span data-stu-id="92d0f-101">Getting started building Microsoft Graph apps</span></span>

<span data-ttu-id="92d0f-p101">Die Artikel in diesem Abschnitt bieten detaillierte Angaben dazu, wie Apps erstellt werden, die aus einer Palette von Sprachen und Entwicklungsplattformen mit Microsoft Graph verbunden werden. Jeder Artikel beginnt mit einem Beispiel eines Startprojekts für die entsprechende Plattform und führt Sie schrittweise durch das Hinzufügen von Funktionen, die den Benutzer authentifizieren, und stellt eine Beispielanforderung an Microsoft Graph, aus ihrem Konto eine E-Mail zu senden. Das fertige Projekt ist identisch mit dem [Connect-Beispiel im Microsoft Graph-Repository](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) für die betreffende Plattform.</span><span class="sxs-lookup"><span data-stu-id="92d0f-p101">The articles in this section provide detailed guidance on how to build apps that connect to Microsoft Graph across a variety of languages and development platforms. Each article starts with a sample starter project for the appropriate platform, and walks you through adding functionality that authenticates the user and makes a sample request to have Microsoft Graph send an email from their account. The completed project is identical to the [Connect sample in the Microsoft Graph repo](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) for that platform.</span></span>

<span data-ttu-id="92d0f-105">Wählen Sie den Artikel, der sich mit dem Authentifizierungsanbieter und der Entwicklungsplattform Ihrer Wahl befasst, und unternehmen Sie die ersten Schritte zum Herstellen einer Verbindung mit Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="92d0f-105">Choose the article that covers the authentication provider and development platform of your choice, and get started connecting to Microsoft Graph.</span></span> <span data-ttu-id="92d0f-106">Weitere Informationen finden Sie unter [Wo liegen die Unterschiede beim v2.0-Endpunkt?](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-compare)</span><span class="sxs-lookup"><span data-stu-id="92d0f-106">For more information about differences between the Azure AD v2.0 endpoint and the Azure AD endpoint, see [What's different about the v2.0 endpoint?](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-compare).</span></span>

<span data-ttu-id="92d0f-107">Sie können die Schritte in diesem Artikel ausführen, der sich mit der Entwicklungsplattform befasst, die Sie auswählen, oder die [Schnellstart](https://developer.microsoft.com/graph/quick-start)-Erfahrung ausprobieren und schnell eine funktionsfähige Lösung einrichten und  ausführen.</span><span class="sxs-lookup"><span data-stu-id="92d0f-107">You can follow the steps in the article that covers the development platform that you choose, or, to quickly get a working solution up and running, try out the [quick start](https://developer.microsoft.com/graph/quick-start) experience.</span></span>

<span data-ttu-id="92d0f-p103">Wenn Sie die fertigen Connect-Beispiele ansehen möchten, besuchen Sie das [Microsoft Graph Repository](https://github.com/microsoftgraph) auf GitHub. In der folgenden Tabelle sind die Beispiele nach Authentifizierungsanbieter und Plattform mit einem Vermerk aufgeführt, ob sie bei der Verbindung mit Microsoft Graph REST oder eine Microsoft Graph-Client-Bibliothek verwenden.</span><span class="sxs-lookup"><span data-stu-id="92d0f-p103">To explore the finished Connect samples, see [Microsoft Graph](https://github.com/microsoftgraph) in GitHub. The following table lists the samples by authentication provider and platform, and notes whether they connect to Microsoft Graph using REST or a Microsoft Graph client library.</span></span>

<table>
  <tr>
    <th><span data-ttu-id="92d0f-110">Plattform</span><span class="sxs-lookup"><span data-stu-id="92d0f-110">Platform</span></span></th>
    <th><span data-ttu-id="92d0f-111">Dem Azure AD-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="92d0f-111">Azure AD endpoint</span></span></th> 
    <th><span data-ttu-id="92d0f-112">Dem Azure AD v2.0-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="92d0f-112">Azure AD v2.0 endpoint</span></span></th>
  </tr>
  <tr>
    <td><span data-ttu-id="92d0f-113">Android</span><span class="sxs-lookup"><span data-stu-id="92d0f-113">Android</span></span></td>
    <td><span data-ttu-id="92d0f-114">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-114">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK sample</a>
    </span></span></td> 
        <td><span data-ttu-id="92d0f-115">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK-Beispiel</a> oder ¶<a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-115">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="92d0f-116">AngularJS</span><span class="sxs-lookup"><span data-stu-id="92d0f-116">AngularJS</span></span></td>
    <td><span data-ttu-id="92d0f-117">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-117">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td> 
        <td><span data-ttu-id="92d0f-118">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">SDK-Beispiel</a> oder ¶<a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-118">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="92d0f-119">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="92d0f-119">ASP.NET</span></span></td>
    <td><span data-ttu-id="92d0f-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="92d0f-121">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK-Beispiel</a> oder ¶<a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-121">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="92d0f-122">iOS (Obj-C)</span><span class="sxs-lookup"><span data-stu-id="92d0f-122">iOS (Obj-C)</span></span></td>
    <td><span data-ttu-id="92d0f-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="92d0f-124">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-124">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="92d0f-125">iOS (Swift)</span><span class="sxs-lookup"><span data-stu-id="92d0f-125">iOS (Swift)</span></span></td>
    <td><span data-ttu-id="92d0f-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="92d0f-127">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-127">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="92d0f-128">NodeJS</span><span class="sxs-lookup"><span data-stu-id="92d0f-128">NodeJS</span></span></td>
    <td><span data-ttu-id="92d0f-129">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-129">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td>    
        <span data-ttu-id="92d0f-130"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK-Beispiel</a> oder <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-130"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="92d0f-131">PHP</span><span class="sxs-lookup"><span data-stu-id="92d0f-131">PHP</span></span></td>
    <td><span data-ttu-id="92d0f-132">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-132">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="92d0f-133">
            <a href="https://github.com/microsoftgraph/php-connect-sample">SDK-Beispiel</a> oder ¶<a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-133">
            <a href="https://github.com/microsoftgraph/php-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="92d0f-134">Python</span><span class="sxs-lookup"><span data-stu-id="92d0f-134">Python</span></span></td>
    <td><span data-ttu-id="92d0f-135">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-135">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td>
    </td> 
  </tr>
  <tr>
    <td><span data-ttu-id="92d0f-136">Ruby</span><span class="sxs-lookup"><span data-stu-id="92d0f-136">Ruby</span></span></td>
    <td><span data-ttu-id="92d0f-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="92d0f-138">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-138">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="92d0f-139">UWP</span><span class="sxs-lookup"><span data-stu-id="92d0f-139">UWP</span></span></td>
    <td><span data-ttu-id="92d0f-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="92d0f-141">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK-Beispiel</a> oder ¶<a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-141">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="92d0f-142">Xamarin</span><span class="sxs-lookup"><span data-stu-id="92d0f-142">Xamarin</span></span></td>
    <td>
    </td>     
    <td><span data-ttu-id="92d0f-143">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="92d0f-143">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
</table>

## <a name="see-also"></a><span data-ttu-id="92d0f-144">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="92d0f-144">See also</span></span>

- <span data-ttu-id="92d0f-145">Testen Sie beispielhafte REST-Aufrufe in unserem [API Explorer](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="92d0f-145">Try out sample REST calls in our [API Explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- [<span data-ttu-id="92d0f-146">Azure AD-Endpunkt-Dokumentation</span><span class="sxs-lookup"><span data-stu-id="92d0f-146">Azure AD endpoint documentation</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-developers-guide)
- [<span data-ttu-id="92d0f-147">Azure AD v2.0-Endpunkt-Dokumentation</span><span class="sxs-lookup"><span data-stu-id="92d0f-147">Azure AD v2.0 endpoint documentation</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-appmodel-v2-overview)
