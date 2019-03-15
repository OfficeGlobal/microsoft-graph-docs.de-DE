---
title: Funktion „getManagedAppDiagnosticStatuses“
description: Diese Funktion ruft den Diagnosevalidierungsstatus des jeweils angegebenen Benutzers ab.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9fd3ab289e02c96f112a4abe6b698e8dd6134a2a
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571172"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="239f9-103">Funktion „getManagedAppDiagnosticStatuses“</span><span class="sxs-lookup"><span data-stu-id="239f9-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="239f9-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="239f9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="239f9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="239f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="239f9-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="239f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="239f9-107">Diese Funktion ruft den Diagnosevalidierungsstatus des jeweils angegebenen Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="239f9-107">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="239f9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="239f9-108">Prerequisites</span></span>
<span data-ttu-id="239f9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="239f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="239f9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="239f9-111">Permission type</span></span>|<span data-ttu-id="239f9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="239f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="239f9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="239f9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="239f9-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="239f9-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="239f9-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="239f9-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="239f9-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="239f9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="239f9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="239f9-117">Not supported.</span></span>|
|<span data-ttu-id="239f9-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="239f9-118">Application</span></span>|<span data-ttu-id="239f9-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="239f9-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="239f9-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="239f9-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="239f9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="239f9-121">Request headers</span></span>
|<span data-ttu-id="239f9-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="239f9-122">Header</span></span>|<span data-ttu-id="239f9-123">Wert</span><span class="sxs-lookup"><span data-stu-id="239f9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="239f9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="239f9-124">Authorization</span></span>|<span data-ttu-id="239f9-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="239f9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="239f9-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="239f9-126">Accept</span></span>|<span data-ttu-id="239f9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="239f9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="239f9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="239f9-128">Request body</span></span>
<span data-ttu-id="239f9-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="239f9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="239f9-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="239f9-130">Response</span></span>
<span data-ttu-id="239f9-131">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="239f9-131">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="239f9-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="239f9-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="239f9-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="239f9-133">Request</span></span>
<span data-ttu-id="239f9-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="239f9-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="239f9-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="239f9-135">Response</span></span>
<span data-ttu-id="239f9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="239f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






