# <a name="assign-action"></a><span data-ttu-id="d2f31-101">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="d2f31-101">assign action</span></span>

> <span data-ttu-id="d2f31-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d2f31-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2f31-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d2f31-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2f31-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d2f31-104">Prerequisites</span></span>
<span data-ttu-id="d2f31-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d2f31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d2f31-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d2f31-107">Permission type</span></span>|<span data-ttu-id="d2f31-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d2f31-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2f31-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d2f31-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d2f31-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2f31-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d2f31-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d2f31-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2f31-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2f31-112">Not supported.</span></span>|
|<span data-ttu-id="d2f31-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d2f31-113">Application</span></span>|<span data-ttu-id="d2f31-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2f31-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2f31-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2f31-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="d2f31-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d2f31-116">Request headers</span></span>
|<span data-ttu-id="d2f31-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d2f31-117">Header</span></span>|<span data-ttu-id="d2f31-118">Wert</span><span class="sxs-lookup"><span data-stu-id="d2f31-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2f31-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2f31-119">Authorization</span></span>|<span data-ttu-id="d2f31-120">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d2f31-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2f31-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d2f31-121">Accept</span></span>|<span data-ttu-id="d2f31-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d2f31-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2f31-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d2f31-123">Request body</span></span>
<span data-ttu-id="d2f31-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Parameters an.</span><span class="sxs-lookup"><span data-stu-id="d2f31-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d2f31-125">Die folgende Tabelle zeigt die Parameter, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="d2f31-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d2f31-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d2f31-126">Property</span></span>|<span data-ttu-id="d2f31-127">Typ</span><span class="sxs-lookup"><span data-stu-id="d2f31-127">Type</span></span>|<span data-ttu-id="d2f31-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2f31-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2f31-129">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="d2f31-129">mobileAppAssignments</span></span>|<span data-ttu-id="d2f31-130">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d2f31-130">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) collection</span></span>|<span data-ttu-id="d2f31-131">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d2f31-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d2f31-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2f31-132">Response</span></span>
<span data-ttu-id="d2f31-133">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d2f31-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d2f31-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d2f31-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2f31-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2f31-135">Request</span></span>
<span data-ttu-id="d2f31-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d2f31-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assign

Content-type: application/json
Content-length: 406

{
  "mobileAppAssignments": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d2f31-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2f31-137">Response</span></span>
<span data-ttu-id="d2f31-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d2f31-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



