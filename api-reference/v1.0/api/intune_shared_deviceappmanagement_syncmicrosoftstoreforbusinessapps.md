# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="cefb2-101">syncMicrosoftStoreForBusinessApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="cefb2-101">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="cefb2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cefb2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cefb2-103">Synchronisiert Intune-Konten mit dem Microsoft Store für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="cefb2-103">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cefb2-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cefb2-104">Prerequisites</span></span>
<span data-ttu-id="cefb2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cefb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cefb2-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cefb2-107">Permission type</span></span>|<span data-ttu-id="cefb2-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cefb2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cefb2-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cefb2-109">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="cefb2-110">&nbsp;&nbsp; _Onboarding_</span><span class="sxs-lookup"><span data-stu-id="cefb2-110">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="cefb2-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cefb2-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cefb2-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cefb2-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cefb2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cefb2-113">Not supported.</span></span>|
|<span data-ttu-id="cefb2-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cefb2-114">Application</span></span>|<span data-ttu-id="cefb2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cefb2-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cefb2-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cefb2-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="cefb2-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cefb2-117">Request headers</span></span>
|<span data-ttu-id="cefb2-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cefb2-118">Header</span></span>|<span data-ttu-id="cefb2-119">Wert</span><span class="sxs-lookup"><span data-stu-id="cefb2-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cefb2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cefb2-120">Authorization</span></span>|<span data-ttu-id="cefb2-121">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cefb2-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cefb2-122">Accept</span><span class="sxs-lookup"><span data-stu-id="cefb2-122">Accept</span></span>|<span data-ttu-id="cefb2-123">application/json</span><span class="sxs-lookup"><span data-stu-id="cefb2-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cefb2-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cefb2-124">Request body</span></span>
<span data-ttu-id="cefb2-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cefb2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cefb2-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="cefb2-126">Response</span></span>
<span data-ttu-id="cefb2-127">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="cefb2-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="cefb2-128">Beispielanforderung</span><span class="sxs-lookup"><span data-stu-id="cefb2-128">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="cefb2-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="cefb2-129">Response</span></span>

<span data-ttu-id="cefb2-130">Der Kürze halber werden möglicherweise im Response-Objekt dargestellten abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="cefb2-130">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cefb2-131">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cefb2-131">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



