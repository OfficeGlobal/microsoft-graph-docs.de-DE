---
title: Funktion „getManagedAppDiagnosticStatuses“
description: Diese Funktion ruft den Diagnosevalidierungsstatus des jeweils angegebenen Benutzers ab.
author: tfitzmac
ms.openlocfilehash: 7318556fd6a87f9f71e5f0a68490a0293182c60d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314182"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="d254c-103">Funktion „getManagedAppDiagnosticStatuses“</span><span class="sxs-lookup"><span data-stu-id="d254c-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="d254c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d254c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d254c-105">Diese Funktion ruft den Diagnosevalidierungsstatus des jeweils angegebenen Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="d254c-105">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d254c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d254c-106">Prerequisites</span></span>
<span data-ttu-id="d254c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d254c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d254c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d254c-109">Permission type</span></span>|<span data-ttu-id="d254c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d254c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d254c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d254c-111">Delegated (work or school account)</span></span>| <span data-ttu-id="d254c-112">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="d254c-112">_varies by context_</span></span>|
| <span data-ttu-id="d254c-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="d254c-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="d254c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d254c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="d254c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d254c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d254c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d254c-116">Not supported.</span></span>|
|<span data-ttu-id="d254c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d254c-117">Application</span></span>|<span data-ttu-id="d254c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d254c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d254c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d254c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="d254c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d254c-120">Request headers</span></span>
|<span data-ttu-id="d254c-121">Header</span><span class="sxs-lookup"><span data-stu-id="d254c-121">Header</span></span>|<span data-ttu-id="d254c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d254c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d254c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d254c-123">Authorization</span></span>|<span data-ttu-id="d254c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d254c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d254c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d254c-125">Accept</span></span>|<span data-ttu-id="d254c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d254c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d254c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d254c-127">Request body</span></span>
<span data-ttu-id="d254c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d254c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d254c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d254c-129">Response</span></span>
<span data-ttu-id="d254c-130">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d254c-130">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d254c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d254c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d254c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d254c-132">Request</span></span>
<span data-ttu-id="d254c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d254c-133">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="d254c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d254c-134">Response</span></span>
<span data-ttu-id="d254c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d254c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



