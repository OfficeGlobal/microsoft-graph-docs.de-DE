---
title: Funktion „getManagedAppDiagnosticStatuses“
description: Diese Funktion ruft den Diagnosevalidierungsstatus des jeweils angegebenen Benutzers ab.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 78eb68346d8269b7aa222949e285584b2ddce3cd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964584"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="c7857-103">Funktion „getManagedAppDiagnosticStatuses“</span><span class="sxs-lookup"><span data-stu-id="c7857-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="c7857-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="c7857-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c7857-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7857-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7857-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c7857-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7857-107">Diese Funktion ruft den Diagnosevalidierungsstatus des jeweils angegebenen Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="c7857-107">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c7857-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c7857-108">Prerequisites</span></span>
<span data-ttu-id="c7857-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7857-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7857-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c7857-111">Permission type</span></span>|<span data-ttu-id="c7857-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c7857-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7857-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c7857-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c7857-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c7857-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c7857-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7857-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c7857-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c7857-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7857-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7857-117">Not supported.</span></span>|
|<span data-ttu-id="c7857-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c7857-118">Application</span></span>|<span data-ttu-id="c7857-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7857-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7857-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7857-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c7857-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c7857-121">Request headers</span></span>
|<span data-ttu-id="c7857-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c7857-122">Header</span></span>|<span data-ttu-id="c7857-123">Wert</span><span class="sxs-lookup"><span data-stu-id="c7857-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7857-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7857-124">Authorization</span></span>|<span data-ttu-id="c7857-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c7857-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7857-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c7857-126">Accept</span></span>|<span data-ttu-id="c7857-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c7857-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7857-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c7857-128">Request body</span></span>
<span data-ttu-id="c7857-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c7857-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7857-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7857-130">Response</span></span>
<span data-ttu-id="c7857-131">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c7857-131">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7857-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c7857-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7857-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7857-133">Request</span></span>
<span data-ttu-id="c7857-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c7857-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="c7857-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7857-135">Response</span></span>
<span data-ttu-id="c7857-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7857-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






