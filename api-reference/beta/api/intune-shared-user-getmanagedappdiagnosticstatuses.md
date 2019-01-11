---
title: Funktion „getManagedAppDiagnosticStatuses“
description: Diese Funktion ruft den Diagnosevalidierungsstatus des jeweils angegebenen Benutzers ab.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6879509d2ffac4c0d01d451f6efcddd973f846c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867809"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="0e265-103">Funktion „getManagedAppDiagnosticStatuses“</span><span class="sxs-lookup"><span data-stu-id="0e265-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="0e265-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0e265-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e265-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0e265-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e265-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0e265-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e265-107">Diese Funktion ruft den Diagnosevalidierungsstatus des jeweils angegebenen Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="0e265-107">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e265-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0e265-108">Prerequisites</span></span>
<span data-ttu-id="0e265-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e265-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e265-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e265-111">Permission type</span></span>|<span data-ttu-id="0e265-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e265-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e265-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e265-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0e265-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="0e265-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="0e265-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e265-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0e265-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e265-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e265-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e265-117">Not supported.</span></span>|
|<span data-ttu-id="0e265-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e265-118">Application</span></span>|<span data-ttu-id="0e265-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e265-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e265-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e265-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="0e265-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e265-121">Request headers</span></span>
|<span data-ttu-id="0e265-122">Header</span><span class="sxs-lookup"><span data-stu-id="0e265-122">Header</span></span>|<span data-ttu-id="0e265-123">Wert</span><span class="sxs-lookup"><span data-stu-id="0e265-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e265-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e265-124">Authorization</span></span>|<span data-ttu-id="0e265-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0e265-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e265-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0e265-126">Accept</span></span>|<span data-ttu-id="0e265-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0e265-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e265-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e265-128">Request body</span></span>
<span data-ttu-id="0e265-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0e265-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e265-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e265-130">Response</span></span>
<span data-ttu-id="0e265-131">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0e265-131">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e265-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e265-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="0e265-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e265-133">Request</span></span>
<span data-ttu-id="0e265-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e265-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="0e265-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e265-135">Response</span></span>
<span data-ttu-id="0e265-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e265-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






