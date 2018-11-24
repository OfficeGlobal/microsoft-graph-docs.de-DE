# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="4c3e2-101">enrollmentConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4c3e2-101">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="4c3e2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4c3e2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c3e2-103">Aktualisieren der Eigenschaften eines [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4c3e2-103">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c3e2-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4c3e2-104">Prerequisites</span></span>
<span data-ttu-id="4c3e2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4c3e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4c3e2-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4c3e2-107">Permission type</span></span>|<span data-ttu-id="4c3e2-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4c3e2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c3e2-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4c3e2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4c3e2-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c3e2-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4c3e2-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4c3e2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c3e2-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c3e2-112">Not supported.</span></span>|
|<span data-ttu-id="4c3e2-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4c3e2-113">Application</span></span>|<span data-ttu-id="4c3e2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c3e2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c3e2-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c3e2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4c3e2-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4c3e2-116">Request headers</span></span>
|<span data-ttu-id="4c3e2-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4c3e2-117">Header</span></span>|<span data-ttu-id="4c3e2-118">Wert</span><span class="sxs-lookup"><span data-stu-id="4c3e2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c3e2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c3e2-119">Authorization</span></span>|<span data-ttu-id="4c3e2-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4c3e2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c3e2-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4c3e2-121">Accept</span></span>|<span data-ttu-id="4c3e2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4c3e2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c3e2-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4c3e2-123">Request body</span></span>
<span data-ttu-id="4c3e2-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="4c3e2-124">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="4c3e2-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4c3e2-125">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="4c3e2-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4c3e2-126">Property</span></span>|<span data-ttu-id="4c3e2-127">Typ</span><span class="sxs-lookup"><span data-stu-id="4c3e2-127">Type</span></span>|<span data-ttu-id="4c3e2-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c3e2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c3e2-129">id</span><span class="sxs-lookup"><span data-stu-id="4c3e2-129">id</span></span>|<span data-ttu-id="4c3e2-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c3e2-130">String</span></span>|<span data-ttu-id="4c3e2-131">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="4c3e2-131">Not yet documented</span></span>|
|<span data-ttu-id="4c3e2-132">target</span><span class="sxs-lookup"><span data-stu-id="4c3e2-132">target</span></span>|[<span data-ttu-id="4c3e2-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4c3e2-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4c3e2-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="4c3e2-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4c3e2-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c3e2-135">Response</span></span>
<span data-ttu-id="4c3e2-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4c3e2-136">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c3e2-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4c3e2-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c3e2-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c3e2-138">Request</span></span>
<span data-ttu-id="4c3e2-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4c3e2-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="4c3e2-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c3e2-140">Response</span></span>
<span data-ttu-id="4c3e2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4c3e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



