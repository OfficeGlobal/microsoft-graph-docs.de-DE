---
title: WindowsOfficeClientConfiguration löschen
description: Löschen Sie eine bestimmte nicht sicherheitsrelevante Richtlinie.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f270d92d894fa2b3b9e2efec4f8d420fda5e2807
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399136"
---
# <a name="delete-windowsofficeclientconfiguration"></a><span data-ttu-id="421ad-103">WindowsOfficeClientConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="421ad-103">Delete windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="421ad-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="421ad-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="421ad-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="421ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="421ad-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="421ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="421ad-107">Löschen Sie eine bestimmte nicht sicherheitsrelevante Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="421ad-107">Delete a specific non-security policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="421ad-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="421ad-108">Prerequisites</span></span>
<span data-ttu-id="421ad-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="421ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="421ad-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="421ad-111">Permission type</span></span>|<span data-ttu-id="421ad-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="421ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="421ad-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="421ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="421ad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="421ad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="421ad-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="421ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="421ad-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="421ad-116">Not supported.</span></span>|
|<span data-ttu-id="421ad-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="421ad-117">Application</span></span>|<span data-ttu-id="421ad-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="421ad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="421ad-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="421ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="421ad-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="421ad-120">Request headers</span></span>
|<span data-ttu-id="421ad-121">Header</span><span class="sxs-lookup"><span data-stu-id="421ad-121">Header</span></span>|<span data-ttu-id="421ad-122">Wert</span><span class="sxs-lookup"><span data-stu-id="421ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="421ad-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="421ad-123">Authorization</span></span>|<span data-ttu-id="421ad-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="421ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="421ad-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="421ad-125">Accept</span></span>|<span data-ttu-id="421ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="421ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="421ad-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="421ad-127">Request body</span></span>
<span data-ttu-id="421ad-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="421ad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="421ad-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="421ad-129">Response</span></span>
<span data-ttu-id="421ad-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="421ad-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="421ad-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="421ad-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="421ad-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="421ad-132">Request</span></span>
<span data-ttu-id="421ad-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="421ad-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="421ad-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="421ad-134">Response</span></span>
<span data-ttu-id="421ad-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="421ad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



