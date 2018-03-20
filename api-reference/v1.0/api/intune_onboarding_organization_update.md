# <a name="update-organization"></a><span data-ttu-id="cd9e7-101">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="cd9e7-101">Update organization</span></span>

> <span data-ttu-id="cd9e7-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cd9e7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd9e7-103">Aktualisieren der Eigenschaften eines [organization](../resources/intune_onboarding_organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cd9e7-103">Update the properties of a [calendar](../resources/intune_onboarding_organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd9e7-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cd9e7-104">Prerequisites</span></span>
<span data-ttu-id="cd9e7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cd9e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cd9e7-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd9e7-107">Permission type</span></span>|<span data-ttu-id="cd9e7-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd9e7-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd9e7-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd9e7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cd9e7-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd9e7-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cd9e7-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd9e7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd9e7-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd9e7-112">Not supported.</span></span>|
|<span data-ttu-id="cd9e7-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd9e7-113">Application</span></span>|<span data-ttu-id="cd9e7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd9e7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd9e7-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd9e7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="cd9e7-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd9e7-116">Request headers</span></span>
|<span data-ttu-id="cd9e7-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cd9e7-117">Header</span></span>|<span data-ttu-id="cd9e7-118">Wert</span><span class="sxs-lookup"><span data-stu-id="cd9e7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd9e7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd9e7-119">Authorization</span></span>|<span data-ttu-id="cd9e7-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cd9e7-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cd9e7-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cd9e7-121">Accept</span></span>|<span data-ttu-id="cd9e7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cd9e7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd9e7-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd9e7-123">Request body</span></span>
<span data-ttu-id="cd9e7-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [organization](../resources/intune_onboarding_organization.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="cd9e7-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_organization.md) object.</span></span>

<span data-ttu-id="cd9e7-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [organization](../resources/intune_onboarding_organization.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="cd9e7-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="cd9e7-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cd9e7-126">Property</span></span>|<span data-ttu-id="cd9e7-127">Typ</span><span class="sxs-lookup"><span data-stu-id="cd9e7-127">Type</span></span>|<span data-ttu-id="cd9e7-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd9e7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd9e7-129">id</span><span class="sxs-lookup"><span data-stu-id="cd9e7-129">id</span></span>|<span data-ttu-id="cd9e7-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd9e7-130">String</span></span>|<span data-ttu-id="cd9e7-131">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="cd9e7-131">The resource GUID for the security object is not valid.</span></span>|
|<span data-ttu-id="cd9e7-132">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="cd9e7-132">mobileDeviceManagementAuthority</span></span>|<span data-ttu-id="cd9e7-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd9e7-133">String</span></span>|<span data-ttu-id="cd9e7-134">Autorität für die Verwaltung mobiler Geräte.</span><span class="sxs-lookup"><span data-stu-id="cd9e7-134">Mobile device management authority.</span></span> <span data-ttu-id="cd9e7-135">Mögliche Werte: `unknown`, `intune`, `sccm` und `office365`.</span><span class="sxs-lookup"><span data-stu-id="cd9e7-135">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="cd9e7-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd9e7-136">Response</span></span>
<span data-ttu-id="cd9e7-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [organization](../resources/intune_onboarding_organization.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd9e7-137">If successful, this method returns a `200 OK` response code and updated [organization](../resources/intune_onboarding_organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd9e7-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd9e7-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd9e7-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd9e7-139">Request</span></span>
<span data-ttu-id="cd9e7-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd9e7-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 51

{
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="cd9e7-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd9e7-141">Response</span></span>
<span data-ttu-id="cd9e7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd9e7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune"
}
```



