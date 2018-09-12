# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="62cf2-101">deviceEnrollmentLimitConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="62cf2-101">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="62cf2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="62cf2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62cf2-103">Aktualisieren der Eigenschaften eines [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="62cf2-103">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="62cf2-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="62cf2-104">Prerequisites</span></span>
<span data-ttu-id="62cf2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="62cf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="62cf2-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="62cf2-107">Permission type</span></span>|<span data-ttu-id="62cf2-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="62cf2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62cf2-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="62cf2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="62cf2-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62cf2-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="62cf2-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="62cf2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62cf2-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62cf2-112">Not supported.</span></span>|
|<span data-ttu-id="62cf2-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="62cf2-113">Application</span></span>|<span data-ttu-id="62cf2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62cf2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62cf2-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="62cf2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="62cf2-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="62cf2-116">Request headers</span></span>
|<span data-ttu-id="62cf2-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="62cf2-117">Header</span></span>|<span data-ttu-id="62cf2-118">Wert</span><span class="sxs-lookup"><span data-stu-id="62cf2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62cf2-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="62cf2-119">Authorization</span></span>|<span data-ttu-id="62cf2-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="62cf2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62cf2-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="62cf2-121">Accept</span></span>|<span data-ttu-id="62cf2-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="62cf2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62cf2-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="62cf2-123">Request body</span></span>
<span data-ttu-id="62cf2-124">Geben Sie im Anforderungstext eine JSON-Darstellung für das Objekt [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="62cf2-124">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="62cf2-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="62cf2-125">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="62cf2-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="62cf2-126">Property</span></span>|<span data-ttu-id="62cf2-127">Typ</span><span class="sxs-lookup"><span data-stu-id="62cf2-127">Type</span></span>|<span data-ttu-id="62cf2-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62cf2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62cf2-129">ID</span><span class="sxs-lookup"><span data-stu-id="62cf2-129">id</span></span>|<span data-ttu-id="62cf2-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62cf2-130">String</span></span>|<span data-ttu-id="62cf2-131">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62cf2-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="62cf2-132">displayName</span><span class="sxs-lookup"><span data-stu-id="62cf2-132">displayName</span></span>|<span data-ttu-id="62cf2-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62cf2-133">String</span></span>|<span data-ttu-id="62cf2-134">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62cf2-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="62cf2-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62cf2-135">description</span></span>|<span data-ttu-id="62cf2-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62cf2-136">String</span></span>|<span data-ttu-id="62cf2-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62cf2-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="62cf2-138">Priorität</span><span class="sxs-lookup"><span data-stu-id="62cf2-138">priority</span></span>|<span data-ttu-id="62cf2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="62cf2-139">Int32</span></span>|<span data-ttu-id="62cf2-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62cf2-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="62cf2-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62cf2-141">createdDateTime</span></span>|<span data-ttu-id="62cf2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62cf2-142">DateTimeOffset</span></span>|<span data-ttu-id="62cf2-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62cf2-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="62cf2-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62cf2-144">lastModifiedDateTime</span></span>|<span data-ttu-id="62cf2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62cf2-145">DateTimeOffset</span></span>|<span data-ttu-id="62cf2-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62cf2-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="62cf2-147">Version</span><span class="sxs-lookup"><span data-stu-id="62cf2-147">version</span></span>|<span data-ttu-id="62cf2-148">Int32</span><span class="sxs-lookup"><span data-stu-id="62cf2-148">Int32</span></span>|<span data-ttu-id="62cf2-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62cf2-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="62cf2-150">Begrenzung</span><span class="sxs-lookup"><span data-stu-id="62cf2-150">limit</span></span>|<span data-ttu-id="62cf2-151">Int32</span><span class="sxs-lookup"><span data-stu-id="62cf2-151">Int32</span></span>|<span data-ttu-id="62cf2-152">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="62cf2-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="62cf2-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="62cf2-153">Response</span></span>
<span data-ttu-id="62cf2-154">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="62cf2-154">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62cf2-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="62cf2-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="62cf2-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="62cf2-156">Request</span></span>
<span data-ttu-id="62cf2-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="62cf2-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 196

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="62cf2-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="62cf2-158">Response</span></span>
<span data-ttu-id="62cf2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="62cf2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```








