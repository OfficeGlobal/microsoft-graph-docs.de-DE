# <a name="update-androidforworksettings"></a><span data-ttu-id="0af1f-101">Aktualisieren von „androidForWorkSettings“</span><span class="sxs-lookup"><span data-stu-id="0af1f-101">Update androidForWorkSettings</span></span>

> <span data-ttu-id="0af1f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0af1f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0af1f-103">Aktualisiert die Eigenschaften eines [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0af1f-103">Update the properties of a [calendar](../resources/intune_androidforwork_androidforworksettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0af1f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0af1f-104">Prerequisites</span></span>
<span data-ttu-id="0af1f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0af1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0af1f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0af1f-107">Permission type</span></span>|<span data-ttu-id="0af1f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0af1f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0af1f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0af1f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0af1f-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0af1f-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0af1f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0af1f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0af1f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0af1f-112">Not supported.</span></span>|
|<span data-ttu-id="0af1f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0af1f-113">Application</span></span>|<span data-ttu-id="0af1f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0af1f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0af1f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0af1f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="0af1f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0af1f-116">Request headers</span></span>
|<span data-ttu-id="0af1f-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0af1f-117">Header</span></span>|<span data-ttu-id="0af1f-118">Wert</span><span class="sxs-lookup"><span data-stu-id="0af1f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0af1f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0af1f-119">Authorization</span></span>|<span data-ttu-id="0af1f-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0af1f-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0af1f-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0af1f-121">Accept</span></span>|<span data-ttu-id="0af1f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0af1f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0af1f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0af1f-123">Request body</span></span>
<span data-ttu-id="0af1f-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="0af1f-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_androidforwork_androidforworksettings.md) object.</span></span>

<span data-ttu-id="0af1f-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0af1f-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="0af1f-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0af1f-126">Property</span></span>|<span data-ttu-id="0af1f-127">Typ</span><span class="sxs-lookup"><span data-stu-id="0af1f-127">Type</span></span>|<span data-ttu-id="0af1f-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0af1f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0af1f-129">id</span><span class="sxs-lookup"><span data-stu-id="0af1f-129">id</span></span>|<span data-ttu-id="0af1f-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0af1f-130">String</span></span>|<span data-ttu-id="0af1f-131">Android for Work-Einstellungsbezeichner.</span><span class="sxs-lookup"><span data-stu-id="0af1f-131">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="0af1f-132">bindStatus</span><span class="sxs-lookup"><span data-stu-id="0af1f-132">bindStatus</span></span>|<span data-ttu-id="0af1f-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0af1f-133">String</span></span>|<span data-ttu-id="0af1f-134">Status der Bindung des Mandanten mit der EMM-API von Google. Mögliche Werte sind: `notBound`, `bound`, `boundAndValidated` und `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="0af1f-134">Bind status of the tenant with the Google EMM API Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="0af1f-135">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0af1f-135">lastAppSyncDateTime</span></span>|<span data-ttu-id="0af1f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0af1f-136">DateTimeOffset</span></span>|<span data-ttu-id="0af1f-137">Zeitpunkt, zu dem zuletzt eine App-Synchronisierung abgeschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="0af1f-137">Last completion time for app sync</span></span>|
|<span data-ttu-id="0af1f-138">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="0af1f-138">lastAppSyncStatus</span></span>|<span data-ttu-id="0af1f-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0af1f-139">String</span></span>|<span data-ttu-id="0af1f-140">Ergebnis der letzten Anwendungssynchronisierung. Mögliche Werte sind: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError` und `none`.</span><span class="sxs-lookup"><span data-stu-id="0af1f-140">Last application sync result Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="0af1f-141">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0af1f-141">ownerUserPrincipalName</span></span>|<span data-ttu-id="0af1f-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0af1f-142">String</span></span>|<span data-ttu-id="0af1f-143">Besitzer-UPN, der das Unternehmen erstellt hat</span><span class="sxs-lookup"><span data-stu-id="0af1f-143">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="0af1f-144">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="0af1f-144">ownerOrganizationName</span></span>|<span data-ttu-id="0af1f-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0af1f-145">String</span></span>|<span data-ttu-id="0af1f-146">Organisationsname, der beim Android for Work-Onboarding verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0af1f-146">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="0af1f-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0af1f-147">lastModifiedDateTime</span></span>|<span data-ttu-id="0af1f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0af1f-148">DateTimeOffset</span></span>|<span data-ttu-id="0af1f-149">Zeitpunkt, zu dem die Android for Work-Einstellungen zuletzt geändert wurden</span><span class="sxs-lookup"><span data-stu-id="0af1f-149">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="0af1f-150">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="0af1f-150">enrollmentTarget</span></span>|<span data-ttu-id="0af1f-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0af1f-151">String</span></span>|<span data-ttu-id="0af1f-152">Gibt an, welche Benutzer Geräte in der Android for Work-Geräteverwaltung registrieren dürfen. Mögliche Werte sind: `none`, `all`, `targeted` und `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="0af1f-152">Indicates which users can enroll devices in Android for Work device management Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="0af1f-153">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="0af1f-153">targetGroupIds</span></span>|<span data-ttu-id="0af1f-154">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="0af1f-154">String collection</span></span>|<span data-ttu-id="0af1f-155">Gibt an, welche AAD-Gruppen Geräte in der Android for Work-Geräteverwaltung registrieren dürfen, wenn die Eigenschaft „enrollmentTarget“ auf „Targeted“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="0af1f-155">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|



## <a name="response"></a><span data-ttu-id="0af1f-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="0af1f-156">Response</span></span>
<span data-ttu-id="0af1f-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0af1f-157">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_androidforwork_androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0af1f-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0af1f-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="0af1f-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0af1f-159">Request</span></span>
<span data-ttu-id="0af1f-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0af1f-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 417

{
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="0af1f-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="0af1f-161">Response</span></span>
<span data-ttu-id="0af1f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0af1f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 527

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ]
}
```



