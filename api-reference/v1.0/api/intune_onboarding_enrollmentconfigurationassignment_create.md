# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="16e51-101">enrollmentConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="16e51-101">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="16e51-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="16e51-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16e51-103">Erstellen eines neuen [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="16e51-103">Create a new [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16e51-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="16e51-104">Prerequisites</span></span>
<span data-ttu-id="16e51-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="16e51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="16e51-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="16e51-107">Permission type</span></span>|<span data-ttu-id="16e51-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="16e51-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16e51-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="16e51-109">Delegated (work or school account)</span></span>|<span data-ttu-id="16e51-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16e51-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="16e51-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="16e51-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16e51-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16e51-112">Not supported.</span></span>|
|<span data-ttu-id="16e51-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="16e51-113">Application</span></span>|<span data-ttu-id="16e51-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16e51-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16e51-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="16e51-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="16e51-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="16e51-116">Request headers</span></span>
|<span data-ttu-id="16e51-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="16e51-117">Header</span></span>|<span data-ttu-id="16e51-118">Wert</span><span class="sxs-lookup"><span data-stu-id="16e51-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16e51-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="16e51-119">Authorization</span></span>|<span data-ttu-id="16e51-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="16e51-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16e51-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="16e51-121">Accept</span></span>|<span data-ttu-id="16e51-122">application/json</span><span class="sxs-lookup"><span data-stu-id="16e51-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16e51-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="16e51-123">Request body</span></span>
<span data-ttu-id="16e51-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs enrollmentConfigurationAssignment an.</span><span class="sxs-lookup"><span data-stu-id="16e51-124">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="16e51-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des enrollmentConfigurationAssignment-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="16e51-125">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="16e51-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16e51-126">Property</span></span>|<span data-ttu-id="16e51-127">Typ</span><span class="sxs-lookup"><span data-stu-id="16e51-127">Type</span></span>|<span data-ttu-id="16e51-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16e51-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16e51-129">ID</span><span class="sxs-lookup"><span data-stu-id="16e51-129">id</span></span>|<span data-ttu-id="16e51-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="16e51-130">String</span></span>|<span data-ttu-id="16e51-131">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="16e51-131">Not yet documented</span></span>|
|<span data-ttu-id="16e51-132">Ziel</span><span class="sxs-lookup"><span data-stu-id="16e51-132">target</span></span>|[<span data-ttu-id="16e51-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="16e51-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="16e51-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="16e51-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="16e51-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="16e51-135">Response</span></span>
<span data-ttu-id="16e51-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="16e51-136">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16e51-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="16e51-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="16e51-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="16e51-138">Request</span></span>
<span data-ttu-id="16e51-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="16e51-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16e51-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="16e51-140">Response</span></span>
<span data-ttu-id="16e51-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="16e51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



