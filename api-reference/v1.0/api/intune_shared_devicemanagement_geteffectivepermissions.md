# <a name="geteffectivepermissions-function"></a><span data-ttu-id="8524e-101">getEffectivePermissions-Funktion</span><span class="sxs-lookup"><span data-stu-id="8524e-101">getEffectivePermissions function</span></span>

> <span data-ttu-id="8524e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8524e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8524e-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8524e-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8524e-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8524e-104">Prerequisites</span></span>
<span data-ttu-id="8524e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8524e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8524e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8524e-107">Permission type</span></span>|<span data-ttu-id="8524e-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8524e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8524e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8524e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8524e-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="8524e-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="8524e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8524e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8524e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8524e-112">Not supported.</span></span>|
|<span data-ttu-id="8524e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8524e-113">Application</span></span>|<span data-ttu-id="8524e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8524e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8524e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8524e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="8524e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8524e-116">Request headers</span></span>
|<span data-ttu-id="8524e-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8524e-117">Header</span></span>|<span data-ttu-id="8524e-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8524e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8524e-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8524e-119">Authorization</span></span>|<span data-ttu-id="8524e-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8524e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8524e-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="8524e-121">Accept</span></span>|<span data-ttu-id="8524e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8524e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8524e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8524e-123">Request body</span></span>
<span data-ttu-id="8524e-124">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="8524e-124">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="8524e-125">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="8524e-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8524e-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8524e-126">Property</span></span>|<span data-ttu-id="8524e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="8524e-127">Type</span></span>|<span data-ttu-id="8524e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8524e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8524e-129">Bereich</span><span class="sxs-lookup"><span data-stu-id="8524e-129">scope</span></span>|<span data-ttu-id="8524e-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8524e-130">String</span></span>|<span data-ttu-id="8524e-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8524e-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8524e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="8524e-132">Response</span></span>
<span data-ttu-id="8524e-133">Wenn die Funktion erfolgreich verläuft, werden der Antwortcode `200 OK` und eine [rolePermission](../resources/intune_rbac_rolepermission.md)-Sammlung im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8524e-133">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune_rbac_rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8524e-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8524e-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="8524e-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8524e-135">Request</span></span>
<span data-ttu-id="8524e-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8524e-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="8524e-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="8524e-137">Response</span></span>
<span data-ttu-id="8524e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8524e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ]
}
```



