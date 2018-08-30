# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="2ee42-101">onPremisesConditionalAccessSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2ee42-101">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="2ee42-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2ee42-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ee42-103">Aktualisieren der Eigenschaften eines [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2ee42-103">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2ee42-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2ee42-104">Prerequisites</span></span>
<span data-ttu-id="2ee42-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2ee42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2ee42-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2ee42-107">Permission type</span></span>|<span data-ttu-id="2ee42-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2ee42-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ee42-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2ee42-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2ee42-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ee42-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2ee42-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2ee42-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ee42-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ee42-112">Not supported.</span></span>|
|<span data-ttu-id="2ee42-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2ee42-113">Application</span></span>|<span data-ttu-id="2ee42-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ee42-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ee42-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ee42-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="2ee42-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2ee42-116">Request headers</span></span>
|<span data-ttu-id="2ee42-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2ee42-117">Header</span></span>|<span data-ttu-id="2ee42-118">Wert</span><span class="sxs-lookup"><span data-stu-id="2ee42-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ee42-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2ee42-119">Authorization</span></span>|<span data-ttu-id="2ee42-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2ee42-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ee42-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="2ee42-121">Accept</span></span>|<span data-ttu-id="2ee42-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="2ee42-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ee42-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2ee42-123">Request body</span></span>
<span data-ttu-id="2ee42-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="2ee42-124">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="2ee42-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2ee42-125">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="2ee42-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2ee42-126">Property</span></span>|<span data-ttu-id="2ee42-127">Typ</span><span class="sxs-lookup"><span data-stu-id="2ee42-127">Type</span></span>|<span data-ttu-id="2ee42-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ee42-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ee42-129">ID</span><span class="sxs-lookup"><span data-stu-id="2ee42-129">id</span></span>|<span data-ttu-id="2ee42-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ee42-130">String</span></span>|<span data-ttu-id="2ee42-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2ee42-131">Not yet documented</span></span>|
|<span data-ttu-id="2ee42-132">aktiviert</span><span class="sxs-lookup"><span data-stu-id="2ee42-132">enabled</span></span>|<span data-ttu-id="2ee42-133">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2ee42-133">Boolean</span></span>|<span data-ttu-id="2ee42-134">Gibt an, ob lokaler bedingter Zugriff für diese Organisation aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="2ee42-134">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="2ee42-135">includedGroups</span><span class="sxs-lookup"><span data-stu-id="2ee42-135">includedGroups</span></span>|<span data-ttu-id="2ee42-136">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2ee42-136">Guid collection</span></span>|<span data-ttu-id="2ee42-137">Benutzergruppen, für die der lokale bedingte Zugriff gilt.</span><span class="sxs-lookup"><span data-stu-id="2ee42-137">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="2ee42-138">Alle Benutzer in diesen Gruppen müssen verwaltete und für den E-Mail-Zugriff kompatible Mobilgeräte verwenden.</span><span class="sxs-lookup"><span data-stu-id="2ee42-138">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="2ee42-139">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="2ee42-139">excludedGroups</span></span>|<span data-ttu-id="2ee42-140">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2ee42-140">Guid collection</span></span>|<span data-ttu-id="2ee42-141">Benutzergruppen, die vom lokalen bedingten Zugriff ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="2ee42-141">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="2ee42-142">Alle Benutzer in diesen Gruppen werden von der Richtlinie zu bedingtem Zugriff ausgenommen.</span><span class="sxs-lookup"><span data-stu-id="2ee42-142">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="2ee42-143">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="2ee42-143">overrideDefaultRule</span></span>|<span data-ttu-id="2ee42-144">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2ee42-144">Boolean</span></span>|<span data-ttu-id="2ee42-145">Überschreibt die Standardzugriffsregel, wenn zugelassen wird, dass einem Gerät Zugriff gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="2ee42-145">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="2ee42-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ee42-146">Response</span></span>
<span data-ttu-id="2ee42-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2ee42-147">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ee42-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2ee42-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="2ee42-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ee42-149">Request</span></span>
<span data-ttu-id="2ee42-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2ee42-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 195

{
  "enabled": true,
  "includedGroups": [
    "79199ed9-e50b-4257-8de4-70b9c8685061"
  ],
  "excludedGroups": [
    "79199ed9-e50b-4257-8de4-70b9c8685061"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="2ee42-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ee42-151">Response</span></span>
<span data-ttu-id="2ee42-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2ee42-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "79199ed9-e50b-4257-8de4-70b9c8685061"
  ],
  "excludedGroups": [
    "79199ed9-e50b-4257-8de4-70b9c8685061"
  ],
  "overrideDefaultRule": true
}
```



