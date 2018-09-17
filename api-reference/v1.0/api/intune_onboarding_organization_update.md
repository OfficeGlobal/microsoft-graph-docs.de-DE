# <a name="update-organization"></a><span data-ttu-id="fd3e9-101">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fd3e9-101">Update organization</span></span>

> <span data-ttu-id="fd3e9-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fd3e9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd3e9-103">Aktualisieren der Eigenschaften eines [organization](../resources/intune_onboarding_organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fd3e9-103">Update the properties of a [organization](../resources/intune_onboarding_organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd3e9-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fd3e9-104">Prerequisites</span></span>
<span data-ttu-id="fd3e9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd3e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd3e9-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd3e9-107">Permission type</span></span>|<span data-ttu-id="fd3e9-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd3e9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd3e9-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd3e9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fd3e9-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd3e9-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fd3e9-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd3e9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd3e9-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd3e9-112">Not supported.</span></span>|
|<span data-ttu-id="fd3e9-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd3e9-113">Application</span></span>|<span data-ttu-id="fd3e9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd3e9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd3e9-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd3e9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="fd3e9-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd3e9-116">Request headers</span></span>
|<span data-ttu-id="fd3e9-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fd3e9-117">Header</span></span>|<span data-ttu-id="fd3e9-118">Wert</span><span class="sxs-lookup"><span data-stu-id="fd3e9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd3e9-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fd3e9-119">Authorization</span></span>|<span data-ttu-id="fd3e9-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fd3e9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd3e9-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="fd3e9-121">Accept</span></span>|<span data-ttu-id="fd3e9-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="fd3e9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd3e9-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd3e9-123">Request body</span></span>
<span data-ttu-id="fd3e9-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [organization](../resources/intune_onboarding_organization.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="fd3e9-124">In the request body, supply a JSON representation for the [organization](../resources/intune_onboarding_organization.md) object.</span></span>

<span data-ttu-id="fd3e9-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [organization](../resources/intune_onboarding_organization.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="fd3e9-125">The following table shows the properties that are required when you create the [organization](../resources/intune_onboarding_organization.md).</span></span>

|<span data-ttu-id="fd3e9-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fd3e9-126">Property</span></span>|<span data-ttu-id="fd3e9-127">Typ</span><span class="sxs-lookup"><span data-stu-id="fd3e9-127">Type</span></span>|<span data-ttu-id="fd3e9-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd3e9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd3e9-129">id</span><span class="sxs-lookup"><span data-stu-id="fd3e9-129">id</span></span>|<span data-ttu-id="fd3e9-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fd3e9-130">String</span></span>|<span data-ttu-id="fd3e9-131">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="fd3e9-131">The GUID for the object.</span></span>|
|<span data-ttu-id="fd3e9-132">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="fd3e9-132">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="fd3e9-133">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="fd3e9-133">mdmAuthority</span></span>](../resources/intune_onboarding_mdmauthority.md)|<span data-ttu-id="fd3e9-p102">Managementautorität für mobile Geräte. Mögliche Werte sind: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="fd3e9-p102">Mobile device management authority. The possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="fd3e9-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd3e9-136">Response</span></span>
<span data-ttu-id="fd3e9-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [organization](../resources/intune_onboarding_organization.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd3e9-137">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune_onboarding_organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd3e9-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd3e9-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd3e9-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd3e9-139">Request</span></span>
<span data-ttu-id="fd3e9-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd3e9-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 51

{
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="fd3e9-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd3e9-141">Response</span></span>
<span data-ttu-id="fd3e9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd3e9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








