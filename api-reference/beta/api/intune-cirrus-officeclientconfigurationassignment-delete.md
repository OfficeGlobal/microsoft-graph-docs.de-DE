---
title: OfficeClientConfigurationAssignment löschen
description: Löscht eine OfficeClientConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c2ab631c6b7e864def9abafac183377294a22737
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808127"
---
# <a name="delete-officeclientconfigurationassignment"></a><span data-ttu-id="c8229-103">OfficeClientConfigurationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="c8229-103">Delete officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="c8229-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c8229-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8229-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8229-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8229-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c8229-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8229-107">Löscht eine [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c8229-107">Deletes a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8229-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c8229-108">Prerequisites</span></span>
<span data-ttu-id="c8229-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8229-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8229-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8229-111">Permission type</span></span>|<span data-ttu-id="c8229-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8229-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8229-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8229-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8229-114">\*\* Zu erledigen: Bestimmen der Bereiche \*\*</span><span class="sxs-lookup"><span data-stu-id="c8229-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="c8229-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8229-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8229-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8229-116">Not supported.</span></span>|
|<span data-ttu-id="c8229-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8229-117">Application</span></span>|<span data-ttu-id="c8229-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8229-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8229-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8229-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c8229-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8229-120">Request headers</span></span>
|<span data-ttu-id="c8229-121">Header</span><span class="sxs-lookup"><span data-stu-id="c8229-121">Header</span></span>|<span data-ttu-id="c8229-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c8229-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8229-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8229-123">Authorization</span></span>|<span data-ttu-id="c8229-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c8229-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8229-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c8229-125">Accept</span></span>|<span data-ttu-id="c8229-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8229-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8229-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8229-127">Request body</span></span>
<span data-ttu-id="c8229-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c8229-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8229-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8229-129">Response</span></span>
<span data-ttu-id="c8229-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8229-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c8229-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8229-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8229-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8229-132">Request</span></span>
<span data-ttu-id="c8229-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8229-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="c8229-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8229-134">Response</span></span>
<span data-ttu-id="c8229-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8229-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



