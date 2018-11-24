# <a name="geteffectivepermissions-function"></a><span data-ttu-id="65e71-101">getEffectivePermissions-Funktion</span><span class="sxs-lookup"><span data-stu-id="65e71-101">getEffectivePermissions function</span></span>

> <span data-ttu-id="65e71-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="65e71-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65e71-103">Ruft die effektiven Berechtigungen des derzeit authentifizierten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="65e71-103">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65e71-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="65e71-104">Prerequisites</span></span>
<span data-ttu-id="65e71-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="65e71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="65e71-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="65e71-107">Permission type</span></span>|<span data-ttu-id="65e71-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="65e71-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65e71-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="65e71-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="65e71-110">&nbsp;&nbsp; Rollenbasierte Zugriffssteuerung</span><span class="sxs-lookup"><span data-stu-id="65e71-110">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="65e71-111">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="65e71-111">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="65e71-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="65e71-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65e71-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65e71-113">Not supported.</span></span>|
|<span data-ttu-id="65e71-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="65e71-114">Application</span></span>|<span data-ttu-id="65e71-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65e71-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65e71-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="65e71-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="65e71-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="65e71-117">Request headers</span></span>
|<span data-ttu-id="65e71-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="65e71-118">Header</span></span>|<span data-ttu-id="65e71-119">Wert</span><span class="sxs-lookup"><span data-stu-id="65e71-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65e71-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="65e71-120">Authorization</span></span>|<span data-ttu-id="65e71-121">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="65e71-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65e71-122">Accept</span><span class="sxs-lookup"><span data-stu-id="65e71-122">Accept</span></span>|<span data-ttu-id="65e71-123">application/json</span><span class="sxs-lookup"><span data-stu-id="65e71-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65e71-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="65e71-124">Request body</span></span>
<span data-ttu-id="65e71-125">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="65e71-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="65e71-126">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="65e71-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="65e71-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="65e71-127">Property</span></span>|<span data-ttu-id="65e71-128">Typ</span><span class="sxs-lookup"><span data-stu-id="65e71-128">Type</span></span>|<span data-ttu-id="65e71-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65e71-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65e71-130">scope</span><span class="sxs-lookup"><span data-stu-id="65e71-130">scope</span></span>|<span data-ttu-id="65e71-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65e71-131">String</span></span>|<span data-ttu-id="65e71-132">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="65e71-132">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="65e71-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="65e71-133">Response</span></span>
<span data-ttu-id="65e71-134">Wenn die Funktion erfolgreich verläuft, werden der Antwortcode `200 OK` und eine [rolePermission](../resources/intune_rbac_rolepermission.md)-Sammlung im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65e71-134">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune_rbac_rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65e71-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="65e71-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="65e71-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65e71-136">Request</span></span>
<span data-ttu-id="65e71-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="65e71-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="65e71-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="65e71-138">Response</span></span>
<span data-ttu-id="65e71-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65e71-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



