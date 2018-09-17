# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="36eb8-101">syncMicrosoftStoreForBusinessApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="36eb8-101">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="36eb8-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="36eb8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36eb8-103">Synchronisiert Intune-Konten mit dem Microsoft Store für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="36eb8-103">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36eb8-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="36eb8-104">Prerequisites</span></span>
<span data-ttu-id="36eb8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="36eb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="36eb8-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="36eb8-107">Permission type</span></span>|<span data-ttu-id="36eb8-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="36eb8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36eb8-109">Delegiert (Arbeits- oder Schulkonto)</span><span class="sxs-lookup"><span data-stu-id="36eb8-109">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="36eb8-110">&nbsp; &nbsp; _Onboarding_</span><span class="sxs-lookup"><span data-stu-id="36eb8-110">&nbsp; &nbsp; _On-boarding_</span></span> | <span data-ttu-id="36eb8-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36eb8-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="36eb8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="36eb8-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36eb8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36eb8-113">Not supported.</span></span>|
|<span data-ttu-id="36eb8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="36eb8-114">Application</span></span>|<span data-ttu-id="36eb8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36eb8-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36eb8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="36eb8-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="36eb8-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="36eb8-117">Request headers</span></span>
|<span data-ttu-id="36eb8-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="36eb8-118">Header</span></span>|<span data-ttu-id="36eb8-119">Wert</span><span class="sxs-lookup"><span data-stu-id="36eb8-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36eb8-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="36eb8-120">Authorization</span></span>|<span data-ttu-id="36eb8-121">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="36eb8-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36eb8-122">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="36eb8-122">Accept</span></span>|<span data-ttu-id="36eb8-123">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="36eb8-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36eb8-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="36eb8-124">Request body</span></span>
<span data-ttu-id="36eb8-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="36eb8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36eb8-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="36eb8-126">Response</span></span>
<span data-ttu-id="36eb8-127">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="36eb8-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="36eb8-128">Beispielanforderung</span><span class="sxs-lookup"><span data-stu-id="36eb8-128">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="36eb8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="36eb8-129">Response</span></span>

<span data-ttu-id="36eb8-130">Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="36eb8-130">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="36eb8-131">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36eb8-131">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



