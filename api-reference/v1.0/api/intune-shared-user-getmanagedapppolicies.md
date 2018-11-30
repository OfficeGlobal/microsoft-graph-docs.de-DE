---
title: Funktion „getManagedAppPolicies“
description: Diese Funktion ruft die App-Einschränkungen für einen bestimmten Benutzer ab.
ms.openlocfilehash: 6cb9b388b8b999b298da070f592ebf7a19d851c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018498"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="e1c2b-103">Funktion „getManagedAppPolicies“</span><span class="sxs-lookup"><span data-stu-id="e1c2b-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="e1c2b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e1c2b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1c2b-105">Diese Funktion ruft die App-Einschränkungen für einen bestimmten Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="e1c2b-105">Gets app restrictions for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1c2b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e1c2b-106">Prerequisites</span></span>
<span data-ttu-id="e1c2b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1c2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1c2b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1c2b-109">Permission type</span></span>|<span data-ttu-id="e1c2b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1c2b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1c2b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1c2b-111">Delegated (work or school account)</span></span>| <span data-ttu-id="e1c2b-112">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="e1c2b-112">_varies by context_</span></span>|
| <span data-ttu-id="e1c2b-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="e1c2b-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="e1c2b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1c2b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="e1c2b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1c2b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1c2b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1c2b-116">Not supported.</span></span>|
|<span data-ttu-id="e1c2b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1c2b-117">Application</span></span>|<span data-ttu-id="e1c2b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1c2b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1c2b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1c2b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="e1c2b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1c2b-120">Request headers</span></span>
|<span data-ttu-id="e1c2b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e1c2b-121">Header</span></span>|<span data-ttu-id="e1c2b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e1c2b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1c2b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1c2b-123">Authorization</span></span>|<span data-ttu-id="e1c2b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e1c2b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1c2b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1c2b-125">Accept</span></span>|<span data-ttu-id="e1c2b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1c2b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1c2b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1c2b-127">Request body</span></span>
<span data-ttu-id="e1c2b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e1c2b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1c2b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1c2b-129">Response</span></span>
<span data-ttu-id="e1c2b-130">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e1c2b-130">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1c2b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1c2b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1c2b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1c2b-132">Request</span></span>
<span data-ttu-id="e1c2b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1c2b-133">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="e1c2b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1c2b-134">Response</span></span>
<span data-ttu-id="e1c2b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1c2b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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


