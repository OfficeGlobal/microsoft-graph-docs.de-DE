# <a name="assign-action"></a><span data-ttu-id="65fd3-101">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="65fd3-101">assign action</span></span>

> <span data-ttu-id="65fd3-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="65fd3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65fd3-103">Diese Aktion ist noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="65fd3-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="65fd3-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="65fd3-104">Prerequisites</span></span>
<span data-ttu-id="65fd3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="65fd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="65fd3-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="65fd3-107">Permission type</span></span>|<span data-ttu-id="65fd3-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="65fd3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65fd3-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="65fd3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="65fd3-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65fd3-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65fd3-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="65fd3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65fd3-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65fd3-112">Not supported.</span></span>|
|<span data-ttu-id="65fd3-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="65fd3-113">Application</span></span>|<span data-ttu-id="65fd3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65fd3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65fd3-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="65fd3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="65fd3-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="65fd3-116">Request headers</span></span>
|<span data-ttu-id="65fd3-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="65fd3-117">Header</span></span>|<span data-ttu-id="65fd3-118">Wert</span><span class="sxs-lookup"><span data-stu-id="65fd3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65fd3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="65fd3-119">Authorization</span></span>|<span data-ttu-id="65fd3-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="65fd3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65fd3-121">Accept</span><span class="sxs-lookup"><span data-stu-id="65fd3-121">Accept</span></span>|<span data-ttu-id="65fd3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="65fd3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65fd3-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="65fd3-123">Request body</span></span>
<span data-ttu-id="65fd3-124">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="65fd3-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="65fd3-125">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="65fd3-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="65fd3-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="65fd3-126">Property</span></span>|<span data-ttu-id="65fd3-127">Typ</span><span class="sxs-lookup"><span data-stu-id="65fd3-127">Type</span></span>|<span data-ttu-id="65fd3-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65fd3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65fd3-129">assignments</span><span class="sxs-lookup"><span data-stu-id="65fd3-129">assignments</span></span>|<span data-ttu-id="65fd3-130">Collection von Objekten des Typs [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="65fd3-130">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="65fd3-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="65fd3-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="65fd3-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="65fd3-132">Response</span></span>
<span data-ttu-id="65fd3-133">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="65fd3-133">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65fd3-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="65fd3-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="65fd3-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65fd3-135">Request</span></span>
<span data-ttu-id="65fd3-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="65fd3-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 277

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="65fd3-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="65fd3-137">Response</span></span>
<span data-ttu-id="65fd3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65fd3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



