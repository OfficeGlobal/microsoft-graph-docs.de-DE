# <a name="sync-action"></a><span data-ttu-id="f4489-101">Aktion „sync“</span><span class="sxs-lookup"><span data-stu-id="f4489-101">sync action</span></span>

> <span data-ttu-id="f4489-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f4489-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4489-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f4489-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f4489-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f4489-104">Prerequisites</span></span>
<span data-ttu-id="f4489-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f4489-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f4489-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f4489-107">Permission type</span></span>|<span data-ttu-id="f4489-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f4489-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4489-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f4489-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f4489-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4489-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f4489-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f4489-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4489-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4489-112">Not supported.</span></span>|
|<span data-ttu-id="f4489-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f4489-113">Application</span></span>|<span data-ttu-id="f4489-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4489-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4489-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4489-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="f4489-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f4489-116">Request headers</span></span>
|<span data-ttu-id="f4489-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f4489-117">Header</span></span>|<span data-ttu-id="f4489-118">Wert</span><span class="sxs-lookup"><span data-stu-id="f4489-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4489-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4489-119">Authorization</span></span>|<span data-ttu-id="f4489-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f4489-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f4489-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f4489-121">Accept</span></span>|<span data-ttu-id="f4489-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f4489-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4489-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f4489-123">Request body</span></span>
<span data-ttu-id="f4489-124">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="f4489-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="f4489-125">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="f4489-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f4489-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f4489-126">Property</span></span>|<span data-ttu-id="f4489-127">Typ</span><span class="sxs-lookup"><span data-stu-id="f4489-127">Type</span></span>|<span data-ttu-id="f4489-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4489-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4489-129">syncType</span><span class="sxs-lookup"><span data-stu-id="f4489-129">syncType</span></span>|<span data-ttu-id="f4489-130">String</span><span class="sxs-lookup"><span data-stu-id="f4489-130">String</span></span>|<span data-ttu-id="f4489-131">Typ der auszuführenden Synchronisierung (vollständige Synchronisierung oder Deltasynchronisierung)</span><span class="sxs-lookup"><span data-stu-id="f4489-131">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="f4489-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4489-132">Response</span></span>
<span data-ttu-id="f4489-133">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="f4489-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f4489-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f4489-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="f4489-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4489-135">Request</span></span>
<span data-ttu-id="f4489-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f4489-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="f4489-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4489-137">Response</span></span>
<span data-ttu-id="f4489-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f4489-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



