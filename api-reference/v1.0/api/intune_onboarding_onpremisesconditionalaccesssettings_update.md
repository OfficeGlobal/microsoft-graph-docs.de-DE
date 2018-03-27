# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="441ac-101">onPremisesConditionalAccessSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="441ac-101">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="441ac-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="441ac-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="441ac-103">Aktualisieren der Eigenschaften eines [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="441ac-103">Update the properties of a [calendar](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="441ac-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="441ac-104">Prerequisites</span></span>
<span data-ttu-id="441ac-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="441ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="441ac-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="441ac-107">Permission type</span></span>|<span data-ttu-id="441ac-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="441ac-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="441ac-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="441ac-109">Delegated (work or school account)</span></span>|<span data-ttu-id="441ac-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="441ac-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="441ac-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="441ac-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="441ac-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="441ac-112">Not supported.</span></span>|
|<span data-ttu-id="441ac-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="441ac-113">Application</span></span>|<span data-ttu-id="441ac-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="441ac-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="441ac-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="441ac-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="441ac-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="441ac-116">Request headers</span></span>
|<span data-ttu-id="441ac-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="441ac-117">Header</span></span>|<span data-ttu-id="441ac-118">Wert</span><span class="sxs-lookup"><span data-stu-id="441ac-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="441ac-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="441ac-119">Authorization</span></span>|<span data-ttu-id="441ac-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="441ac-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="441ac-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="441ac-121">Accept</span></span>|<span data-ttu-id="441ac-122">application/json</span><span class="sxs-lookup"><span data-stu-id="441ac-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="441ac-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="441ac-123">Request body</span></span>
<span data-ttu-id="441ac-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="441ac-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="441ac-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="441ac-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="441ac-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="441ac-126">Property</span></span>|<span data-ttu-id="441ac-127">Typ</span><span class="sxs-lookup"><span data-stu-id="441ac-127">Type</span></span>|<span data-ttu-id="441ac-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="441ac-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="441ac-129">id</span><span class="sxs-lookup"><span data-stu-id="441ac-129">id</span></span>|<span data-ttu-id="441ac-130">String</span><span class="sxs-lookup"><span data-stu-id="441ac-130">String</span></span>|<span data-ttu-id="441ac-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="441ac-131">Not yet documented</span></span>|
|<span data-ttu-id="441ac-132">aktiviert</span><span class="sxs-lookup"><span data-stu-id="441ac-132">enabled</span></span>|<span data-ttu-id="441ac-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="441ac-133">Boolean</span></span>|<span data-ttu-id="441ac-134">Gibt an, ob lokaler bedingter Zugriff für diese Organisation aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="441ac-134">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="441ac-135">includedGroups</span><span class="sxs-lookup"><span data-stu-id="441ac-135">includedGroups</span></span>|<span data-ttu-id="441ac-136">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="441ac-136">Guid collection</span></span>|<span data-ttu-id="441ac-137">Benutzergruppen, für die der lokale bedingte Zugriff gilt.</span><span class="sxs-lookup"><span data-stu-id="441ac-137">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="441ac-138">Alle Benutzer in diesen Gruppen müssen verwaltete und für den E-Mail-Zugriff kompatible Mobilgeräte verwenden.</span><span class="sxs-lookup"><span data-stu-id="441ac-138">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="441ac-139">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="441ac-139">excludedGroups</span></span>|<span data-ttu-id="441ac-140">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="441ac-140">Guid collection</span></span>|<span data-ttu-id="441ac-141">Benutzergruppen, die vom lokalen bedingten Zugriff ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="441ac-141">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="441ac-142">Alle Benutzer in diesen Gruppen werden von der Richtlinie zu bedingtem Zugriff ausgenommen.</span><span class="sxs-lookup"><span data-stu-id="441ac-142">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="441ac-143">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="441ac-143">overrideDefaultRule</span></span>|<span data-ttu-id="441ac-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="441ac-144">Boolean</span></span>|<span data-ttu-id="441ac-145">Überschreibt die Standardzugriffsregel, wenn zugelassen wird, dass einem Gerät Zugriff gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="441ac-145">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="441ac-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="441ac-146">Response</span></span>
<span data-ttu-id="441ac-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="441ac-147">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="441ac-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="441ac-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="441ac-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="441ac-149">Request</span></span>
<span data-ttu-id="441ac-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="441ac-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 195

{
  "enabled": true,
  "includedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "excludedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="441ac-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="441ac-151">Response</span></span>
<span data-ttu-id="441ac-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="441ac-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "excludedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "overrideDefaultRule": true
}
```



