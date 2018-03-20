# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="83b36-101">enrollmentConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="83b36-101">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="83b36-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="83b36-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83b36-103">Erstellen eines neuen [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="83b36-103">Create a new [plannerBucket](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83b36-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="83b36-104">Prerequisites</span></span>
<span data-ttu-id="83b36-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="83b36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="83b36-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="83b36-107">Permission type</span></span>|<span data-ttu-id="83b36-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="83b36-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83b36-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="83b36-109">Delegated (work or school account)</span></span>|<span data-ttu-id="83b36-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b36-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="83b36-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="83b36-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83b36-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83b36-112">Not supported.</span></span>|
|<span data-ttu-id="83b36-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="83b36-113">Application</span></span>|<span data-ttu-id="83b36-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83b36-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83b36-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="83b36-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="83b36-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="83b36-116">Request headers</span></span>
|<span data-ttu-id="83b36-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="83b36-117">Header</span></span>|<span data-ttu-id="83b36-118">Wert</span><span class="sxs-lookup"><span data-stu-id="83b36-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83b36-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="83b36-119">Authorization</span></span>|<span data-ttu-id="83b36-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="83b36-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="83b36-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="83b36-121">Accept</span></span>|<span data-ttu-id="83b36-122">application/json</span><span class="sxs-lookup"><span data-stu-id="83b36-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83b36-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="83b36-123">Request body</span></span>
<span data-ttu-id="83b36-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs enrollmentConfigurationAssignment an.</span><span class="sxs-lookup"><span data-stu-id="83b36-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="83b36-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des enrollmentConfigurationAssignment-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="83b36-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="83b36-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83b36-126">Property</span></span>|<span data-ttu-id="83b36-127">Typ</span><span class="sxs-lookup"><span data-stu-id="83b36-127">Type</span></span>|<span data-ttu-id="83b36-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83b36-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83b36-129">id</span><span class="sxs-lookup"><span data-stu-id="83b36-129">id</span></span>|<span data-ttu-id="83b36-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83b36-130">String</span></span>|<span data-ttu-id="83b36-131">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="83b36-131">Not yet documented</span></span>|
|<span data-ttu-id="83b36-132">target</span><span class="sxs-lookup"><span data-stu-id="83b36-132">target</span></span>|[<span data-ttu-id="83b36-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="83b36-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_onboarding_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="83b36-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="83b36-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="83b36-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="83b36-135">Response</span></span>
<span data-ttu-id="83b36-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="83b36-136">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83b36-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="83b36-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="83b36-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="83b36-138">Request</span></span>
<span data-ttu-id="83b36-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83b36-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="83b36-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="83b36-140">Response</span></span>
<span data-ttu-id="83b36-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="83b36-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



