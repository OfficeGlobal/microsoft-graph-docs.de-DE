# <a name="update-mobileappcategory"></a><span data-ttu-id="d2844-101">Aktualisieren von „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="d2844-101">Update mobileAppCategory</span></span>

> <span data-ttu-id="d2844-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d2844-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2844-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="d2844-103">Update the properties of a [calendar](../resources/intune_apps_mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2844-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d2844-104">Prerequisites</span></span>
<span data-ttu-id="d2844-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d2844-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d2844-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d2844-107">Permission type</span></span>|<span data-ttu-id="d2844-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d2844-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2844-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d2844-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d2844-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2844-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d2844-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d2844-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2844-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2844-112">Not supported.</span></span>|
|<span data-ttu-id="d2844-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d2844-113">Application</span></span>|<span data-ttu-id="d2844-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2844-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2844-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2844-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="d2844-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d2844-116">Request headers</span></span>
|<span data-ttu-id="d2844-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d2844-117">Header</span></span>|<span data-ttu-id="d2844-118">Wert</span><span class="sxs-lookup"><span data-stu-id="d2844-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2844-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2844-119">Authorization</span></span>|<span data-ttu-id="d2844-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d2844-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d2844-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d2844-121">Accept</span></span>|<span data-ttu-id="d2844-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d2844-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2844-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d2844-123">Request body</span></span>
<span data-ttu-id="d2844-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) an.</span><span class="sxs-lookup"><span data-stu-id="d2844-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_mobileappcategory.md) object.</span></span>

<span data-ttu-id="d2844-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="d2844-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="d2844-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d2844-126">Property</span></span>|<span data-ttu-id="d2844-127">Typ</span><span class="sxs-lookup"><span data-stu-id="d2844-127">Type</span></span>|<span data-ttu-id="d2844-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2844-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2844-129">id</span><span class="sxs-lookup"><span data-stu-id="d2844-129">id</span></span>|<span data-ttu-id="d2844-130">String</span><span class="sxs-lookup"><span data-stu-id="d2844-130">String</span></span>|<span data-ttu-id="d2844-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d2844-131">The key of the setting.</span></span>|
|<span data-ttu-id="d2844-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d2844-132">displayName</span></span>|<span data-ttu-id="d2844-133">String</span><span class="sxs-lookup"><span data-stu-id="d2844-133">String</span></span>|<span data-ttu-id="d2844-134">Name der App-Kategorie</span><span class="sxs-lookup"><span data-stu-id="d2844-134">The name of the app.</span></span>|
|<span data-ttu-id="d2844-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2844-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d2844-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2844-136">DateTimeOffset</span></span>|<span data-ttu-id="d2844-137">Datum und Uhrzeit der letzten Änderung des Objekts des Typs „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="d2844-137">The date and time when the attachment was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="d2844-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2844-138">Response</span></span>
<span data-ttu-id="d2844-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d2844-139">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2844-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d2844-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2844-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2844-141">Request</span></span>
<span data-ttu-id="d2844-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d2844-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 107

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="d2844-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2844-143">Response</span></span>
<span data-ttu-id="d2844-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d2844-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



