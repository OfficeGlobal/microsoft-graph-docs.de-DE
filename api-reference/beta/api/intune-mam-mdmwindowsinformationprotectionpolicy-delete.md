---
title: mdmWindowsInformationProtectionPolicy löschen
description: Löscht Objekte des Typs mdmWindowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 22b5eb1392a31ed7d02be87d4fccc92e8e4280af
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974680"
---
# <a name="delete-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="61407-103">mdmWindowsInformationProtectionPolicy löschen</span><span class="sxs-lookup"><span data-stu-id="61407-103">Delete mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="61407-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="61407-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61407-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="61407-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61407-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="61407-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61407-107">Löscht ein [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="61407-107">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="61407-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="61407-108">Prerequisites</span></span>
<span data-ttu-id="61407-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61407-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61407-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="61407-111">Permission type</span></span>|<span data-ttu-id="61407-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="61407-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61407-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="61407-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61407-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61407-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="61407-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="61407-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61407-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61407-116">Not supported.</span></span>|
|<span data-ttu-id="61407-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="61407-117">Application</span></span>|<span data-ttu-id="61407-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61407-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61407-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="61407-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="61407-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="61407-120">Request headers</span></span>
|<span data-ttu-id="61407-121">Header</span><span class="sxs-lookup"><span data-stu-id="61407-121">Header</span></span>|<span data-ttu-id="61407-122">Wert</span><span class="sxs-lookup"><span data-stu-id="61407-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61407-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="61407-123">Authorization</span></span>|<span data-ttu-id="61407-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="61407-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61407-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="61407-125">Accept</span></span>|<span data-ttu-id="61407-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61407-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61407-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="61407-127">Request body</span></span>
<span data-ttu-id="61407-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="61407-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61407-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="61407-129">Response</span></span>
<span data-ttu-id="61407-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61407-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="61407-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61407-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="61407-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="61407-132">Request</span></span>
<span data-ttu-id="61407-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61407-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="61407-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="61407-134">Response</span></span>
<span data-ttu-id="61407-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61407-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





