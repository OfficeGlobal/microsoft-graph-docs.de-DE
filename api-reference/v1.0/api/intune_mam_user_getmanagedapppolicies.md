# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="97b4d-101">Funktion „getManagedAppPolicies“</span><span class="sxs-lookup"><span data-stu-id="97b4d-101">getManagedAppPolicies function</span></span>

> <span data-ttu-id="97b4d-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="97b4d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97b4d-103">Diese Funktion ruft die App-Einschränkungen für einen bestimmten Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="97b4d-103">Gets app restrictions for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97b4d-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="97b4d-104">Prerequisites</span></span>
<span data-ttu-id="97b4d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97b4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97b4d-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97b4d-107">Permission type</span></span>|<span data-ttu-id="97b4d-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97b4d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97b4d-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97b4d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="97b4d-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="97b4d-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="97b4d-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97b4d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97b4d-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97b4d-112">Not supported.</span></span>|
|<span data-ttu-id="97b4d-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97b4d-113">Application</span></span>|<span data-ttu-id="97b4d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97b4d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97b4d-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97b4d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="97b4d-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97b4d-116">Request headers</span></span>
|<span data-ttu-id="97b4d-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="97b4d-117">Header</span></span>|<span data-ttu-id="97b4d-118">Wert</span><span class="sxs-lookup"><span data-stu-id="97b4d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97b4d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="97b4d-119">Authorization</span></span>|<span data-ttu-id="97b4d-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="97b4d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="97b4d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="97b4d-121">Accept</span></span>|<span data-ttu-id="97b4d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="97b4d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97b4d-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97b4d-123">Request body</span></span>
<span data-ttu-id="97b4d-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="97b4d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97b4d-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="97b4d-125">Response</span></span>
<span data-ttu-id="97b4d-126">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="97b4d-126">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/intune_mam_managedapppolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97b4d-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97b4d-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="97b4d-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97b4d-128">Request</span></span>
<span data-ttu-id="97b4d-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97b4d-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="97b4d-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="97b4d-130">Response</span></span>
<span data-ttu-id="97b4d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97b4d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```



