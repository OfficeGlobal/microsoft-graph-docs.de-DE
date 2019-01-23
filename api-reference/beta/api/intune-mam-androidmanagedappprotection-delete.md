---
title: androidManagedAppProtection löschen
description: Löscht Objekte des Typs androidManagedAppProtection.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3a0dbdbb5206fe2a1adb01029072cad799136b0f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403581"
---
# <a name="delete-androidmanagedappprotection"></a><span data-ttu-id="2f75f-103">androidManagedAppProtection löschen</span><span class="sxs-lookup"><span data-stu-id="2f75f-103">Delete androidManagedAppProtection</span></span>

> <span data-ttu-id="2f75f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2f75f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2f75f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2f75f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f75f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2f75f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f75f-107">Löscht Objekte des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2f75f-107">Deletes a [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f75f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2f75f-108">Prerequisites</span></span>
<span data-ttu-id="2f75f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f75f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f75f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f75f-111">Permission type</span></span>|<span data-ttu-id="2f75f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f75f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f75f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f75f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f75f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f75f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2f75f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f75f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f75f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f75f-116">Not supported.</span></span>|
|<span data-ttu-id="2f75f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f75f-117">Application</span></span>|<span data-ttu-id="2f75f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f75f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f75f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f75f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="2f75f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f75f-120">Request headers</span></span>
|<span data-ttu-id="2f75f-121">Header</span><span class="sxs-lookup"><span data-stu-id="2f75f-121">Header</span></span>|<span data-ttu-id="2f75f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2f75f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f75f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2f75f-123">Authorization</span></span>|<span data-ttu-id="2f75f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2f75f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f75f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2f75f-125">Accept</span></span>|<span data-ttu-id="2f75f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f75f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f75f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f75f-127">Request body</span></span>
<span data-ttu-id="2f75f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2f75f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f75f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f75f-129">Response</span></span>
<span data-ttu-id="2f75f-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f75f-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2f75f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f75f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f75f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f75f-132">Request</span></span>
<span data-ttu-id="2f75f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f75f-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="2f75f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f75f-134">Response</span></span>
<span data-ttu-id="2f75f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f75f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




