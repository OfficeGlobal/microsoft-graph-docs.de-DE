# <a name="create-mobileappcontent"></a><span data-ttu-id="41f4b-101">Erstellen von „mobileAppContent“</span><span class="sxs-lookup"><span data-stu-id="41f4b-101">Create mobileAppContent</span></span>

> <span data-ttu-id="41f4b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="41f4b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41f4b-103">Diese Methode erstellt ein neues Objekt des Typs [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="41f4b-103">Create a new [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41f4b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="41f4b-104">Prerequisites</span></span>
<span data-ttu-id="41f4b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="41f4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="41f4b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="41f4b-107">Permission type</span></span>|<span data-ttu-id="41f4b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="41f4b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41f4b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="41f4b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="41f4b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41f4b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41f4b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="41f4b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41f4b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41f4b-112">Not supported.</span></span>|
|<span data-ttu-id="41f4b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="41f4b-113">Application</span></span>|<span data-ttu-id="41f4b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41f4b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41f4b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="41f4b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="41f4b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="41f4b-116">Request headers</span></span>
|<span data-ttu-id="41f4b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="41f4b-117">Header</span></span>|<span data-ttu-id="41f4b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="41f4b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41f4b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="41f4b-119">Authorization</span></span>|<span data-ttu-id="41f4b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="41f4b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41f4b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="41f4b-121">Accept</span></span>|<span data-ttu-id="41f4b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="41f4b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41f4b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="41f4b-123">Request body</span></span>
<span data-ttu-id="41f4b-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppContent“ an.</span><span class="sxs-lookup"><span data-stu-id="41f4b-124">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="41f4b-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppContent“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="41f4b-125">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="41f4b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="41f4b-126">Property</span></span>|<span data-ttu-id="41f4b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="41f4b-127">Type</span></span>|<span data-ttu-id="41f4b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41f4b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41f4b-129">id</span><span class="sxs-lookup"><span data-stu-id="41f4b-129">id</span></span>|<span data-ttu-id="41f4b-130">String</span><span class="sxs-lookup"><span data-stu-id="41f4b-130">String</span></span>|<span data-ttu-id="41f4b-131">Version der App-Inhalte</span><span class="sxs-lookup"><span data-stu-id="41f4b-131">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="41f4b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="41f4b-132">Response</span></span>
<span data-ttu-id="41f4b-133">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppContent](../resources/intune_apps_mobileappcontent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="41f4b-133">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41f4b-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="41f4b-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="41f4b-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="41f4b-135">Request</span></span>
<span data-ttu-id="41f4b-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="41f4b-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="41f4b-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="41f4b-137">Response</span></span>
<span data-ttu-id="41f4b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="41f4b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



