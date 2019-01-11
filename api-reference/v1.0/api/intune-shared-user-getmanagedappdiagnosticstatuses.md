---
title: Funktion „getManagedAppDiagnosticStatuses“
description: Diese Funktion ruft den Diagnosevalidierungsstatus des jeweils angegebenen Benutzers ab.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af90cc194dc1e9c1a954a090c748ef679248d9d3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888585"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="e45bf-103">Funktion „getManagedAppDiagnosticStatuses“</span><span class="sxs-lookup"><span data-stu-id="e45bf-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="e45bf-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e45bf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e45bf-105">Diese Funktion ruft den Diagnosevalidierungsstatus des jeweils angegebenen Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="e45bf-105">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e45bf-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e45bf-106">Prerequisites</span></span>
<span data-ttu-id="e45bf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e45bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e45bf-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e45bf-109">Permission type</span></span>|<span data-ttu-id="e45bf-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e45bf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e45bf-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e45bf-111">Delegated (work or school account)</span></span>| <span data-ttu-id="e45bf-112">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="e45bf-112">_varies by context_</span></span>|
| <span data-ttu-id="e45bf-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="e45bf-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="e45bf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e45bf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="e45bf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e45bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e45bf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e45bf-116">Not supported.</span></span>|
|<span data-ttu-id="e45bf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e45bf-117">Application</span></span>|<span data-ttu-id="e45bf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e45bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e45bf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e45bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="e45bf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e45bf-120">Request headers</span></span>
|<span data-ttu-id="e45bf-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e45bf-121">Header</span></span>|<span data-ttu-id="e45bf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e45bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e45bf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e45bf-123">Authorization</span></span>|<span data-ttu-id="e45bf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e45bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e45bf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e45bf-125">Accept</span></span>|<span data-ttu-id="e45bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e45bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e45bf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e45bf-127">Request body</span></span>
<span data-ttu-id="e45bf-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e45bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e45bf-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e45bf-129">Response</span></span>
<span data-ttu-id="e45bf-130">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e45bf-130">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e45bf-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e45bf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e45bf-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e45bf-132">Request</span></span>
<span data-ttu-id="e45bf-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e45bf-133">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="e45bf-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e45bf-134">Response</span></span>
<span data-ttu-id="e45bf-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e45bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```



