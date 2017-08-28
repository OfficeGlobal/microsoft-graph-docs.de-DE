# <a name="getting-started-building-microsoft-graph-apps"></a><span data-ttu-id="15a62-101">Erste Schritte zum Entwickeln von Microsoft Graph-Apps</span><span class="sxs-lookup"><span data-stu-id="15a62-101">Getting started building Microsoft Graph apps</span></span>

<span data-ttu-id="15a62-p101">Die Artikel in diesem Abschnitt bieten detaillierte Angaben dazu, wie Apps erstellt werden, die aus einer Palette von Sprachen und Entwicklungsplattformen mit Microsoft Graph verbunden werden. Jeder Artikel beginnt mit einem Beispiel eines Startprojekts für die entsprechende Plattform und führt Sie schrittweise durch das Hinzufügen von Funktionen, die den Benutzer authentifizieren, und stellt eine Beispielanforderung an Microsoft Graph, aus ihrem Konto eine E-Mail zu senden. Das fertige Projekt ist identisch mit dem [Connect-Beispiel im Microsoft Graph-Repository](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) für die betreffende Plattform.</span><span class="sxs-lookup"><span data-stu-id="15a62-p101">The articles in this section provide detailed guidance on how to build apps that connect to Microsoft Graph across a variety of languages and development platforms. Each article starts with a sample starter project for the appropriate platform, and walks you through adding functionality that authenticates the user and makes a sample request to have Microsoft Graph send an email from their account. The completed project is identical to the [Connect sample in the Microsoft Graph repo](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) for that platform.</span></span>

<span data-ttu-id="15a62-105">Wählen Sie den Artikel, der sich mit dem Authentifizierungsanbieter und der Entwicklungsplattform Ihrer Wahl befasst, und unternehmen Sie die ersten Schritte zum Herstellen einer Verbindung mit Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="15a62-105">Choose the article that covers the authentication provider and development platform of your choice, and get started connecting to Microsoft Graph.</span></span>

<span data-ttu-id="15a62-106">Sie können die Schritte in diesem Artikel ausführen, der sich mit der Entwicklungsplattform befasst, die Sie auswählen, oder die [Schnellstart](https://developer.microsoft.com/graph/quick-start)-Erfahrung ausprobieren und schnell eine funktionsfähige Lösung einrichten und  ausführen.</span><span class="sxs-lookup"><span data-stu-id="15a62-106">You can follow the steps in the article that covers the development platform that you choose, or, to quickly get a working solution up and running, try out the [quick start](https://developer.microsoft.com/graph/quick-start) experience.</span></span>

<span data-ttu-id="15a62-p102">Wenn Sie die fertigen Connect-Beispiele ansehen möchten, besuchen Sie das [Microsoft Graph Repository](https://github.com/microsoftgraph) auf GitHub. In der folgenden Tabelle sind die Beispiele nach Authentifizierungsanbieter und Plattform mit einem Vermerk aufgeführt, ob sie bei der Verbindung mit Microsoft Graph REST oder eine Microsoft Graph-Client-Bibliothek verwenden.</span><span class="sxs-lookup"><span data-stu-id="15a62-p102">To explore the finished Connect samples, see [Microsoft Graph](https://github.com/microsoftgraph) in GitHub. The following table lists the samples by authentication provider and platform, and notes whether they connect to Microsoft Graph using REST or a Microsoft Graph client library.</span></span>

<table>
  <tr>
    <th><span data-ttu-id="15a62-109">Plattform</span><span class="sxs-lookup"><span data-stu-id="15a62-109">Platform</span></span></th>
    <th><span data-ttu-id="15a62-110">Dem Azure AD-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="15a62-110">Azure AD endpoint</span></span></th> 
    <th><span data-ttu-id="15a62-111">Dem Azure AD v2.0-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="15a62-111">Azure AD v2.0 endpoint</span></span></th>
  </tr>
  <tr>
    <td><span data-ttu-id="15a62-112">Android</span><span class="sxs-lookup"><span data-stu-id="15a62-112">Android</span></span></td>
    <td><span data-ttu-id="15a62-113">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-113">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK sample</a>
    </span></span></td> 
        <td><span data-ttu-id="15a62-114">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK-Beispiel</a> oder ¶<a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-114">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="15a62-115">AngularJS</span><span class="sxs-lookup"><span data-stu-id="15a62-115">AngularJS</span></span></td>
    <td><span data-ttu-id="15a62-116">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-116">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td> 
        <td><span data-ttu-id="15a62-117">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">SDK-Beispiel</a> oder ¶<a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-117">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="15a62-118">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="15a62-118">ASP.NET</span></span></td>
    <td><span data-ttu-id="15a62-119">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-119">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="15a62-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK-Beispiel</a> oder ¶<a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="15a62-121">iOS (Obj-C)</span><span class="sxs-lookup"><span data-stu-id="15a62-121">iOS (Obj-C)</span></span></td>
    <td><span data-ttu-id="15a62-122">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-122">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="15a62-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="15a62-124">iOS (Swift)</span><span class="sxs-lookup"><span data-stu-id="15a62-124">iOS (Swift)</span></span></td>
    <td><span data-ttu-id="15a62-125">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-125">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="15a62-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="15a62-127">NodeJS</span><span class="sxs-lookup"><span data-stu-id="15a62-127">NodeJS</span></span></td>
    <td><span data-ttu-id="15a62-128">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-128">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td>    
        <span data-ttu-id="15a62-129"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK-Beispiel</a> oder <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-129"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="15a62-130">PHP</span><span class="sxs-lookup"><span data-stu-id="15a62-130">PHP</span></span></td>
    <td><span data-ttu-id="15a62-131">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-131">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="15a62-132">
            <a href="https://github.com/microsoftgraph/php-connect-sample">SDK-Beispiel</a> oder ¶<a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-132">
            <a href="https://github.com/microsoftgraph/php-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="15a62-133">Python</span><span class="sxs-lookup"><span data-stu-id="15a62-133">Python</span></span></td>
    <td><span data-ttu-id="15a62-134">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-134">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td>
    </td> 
  </tr>
  <tr>
    <td><span data-ttu-id="15a62-135">Ruby</span><span class="sxs-lookup"><span data-stu-id="15a62-135">Ruby</span></span></td>
    <td><span data-ttu-id="15a62-136">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-136">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="15a62-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="15a62-138">UWP</span><span class="sxs-lookup"><span data-stu-id="15a62-138">UWP</span></span></td>
    <td><span data-ttu-id="15a62-139">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-139">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="15a62-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK-Beispiel</a> oder ¶<a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="15a62-141">Xamarin</span><span class="sxs-lookup"><span data-stu-id="15a62-141">Xamarin</span></span></td>
    <td>
    </td>     
    <td><span data-ttu-id="15a62-142">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK-Beispiel</a>
    </span><span class="sxs-lookup"><span data-stu-id="15a62-142">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
</table>

## <a name="see-also"></a><span data-ttu-id="15a62-143">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="15a62-143">See also</span></span>
- <span data-ttu-id="15a62-144">Testen Sie beispielhafte REST-Aufrufe in unserem [API Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="15a62-144">Try out sample REST calls in our [API Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- [<span data-ttu-id="15a62-145">Azure AD-Endpunkt-Dokumentation</span><span class="sxs-lookup"><span data-stu-id="15a62-145">Azure AD endpoint documentation</span></span>](https://azure.microsoft.com/documentation/services/active-directory/)
- [<span data-ttu-id="15a62-146">Azure AD v2.0-Endpunkt-Dokumentation</span><span class="sxs-lookup"><span data-stu-id="15a62-146">Azure AD v2.0 endpoint documentation</span></span>](https://azure.microsoft.com/documentation/articles/?service=active-directory&term=azure+ad+v2.0)
