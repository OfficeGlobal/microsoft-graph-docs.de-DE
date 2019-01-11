---
title: Organisation aktualisieren
description: Aktualisieren der Eigenschaften eines organization-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d7ecdb1ea142f31b07038f1ffe8779c675eeaaf4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835525"
---
# <a name="update-organization"></a><span data-ttu-id="2e1d0-103">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2e1d0-103">Update organization</span></span>

> <span data-ttu-id="2e1d0-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2e1d0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e1d0-105">Aktualisieren der Eigenschaften eines [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2e1d0-105">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e1d0-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2e1d0-106">Prerequisites</span></span>
<span data-ttu-id="2e1d0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e1d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e1d0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e1d0-109">Permission type</span></span>|<span data-ttu-id="2e1d0-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e1d0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e1d0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e1d0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2e1d0-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e1d0-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2e1d0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e1d0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e1d0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e1d0-114">Not supported.</span></span>|
|<span data-ttu-id="2e1d0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e1d0-115">Application</span></span>|<span data-ttu-id="2e1d0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e1d0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e1d0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e1d0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="2e1d0-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e1d0-118">Request headers</span></span>
|<span data-ttu-id="2e1d0-119">Header</span><span class="sxs-lookup"><span data-stu-id="2e1d0-119">Header</span></span>|<span data-ttu-id="2e1d0-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2e1d0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e1d0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e1d0-121">Authorization</span></span>|<span data-ttu-id="2e1d0-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2e1d0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e1d0-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2e1d0-123">Accept</span></span>|<span data-ttu-id="2e1d0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2e1d0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e1d0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2e1d0-125">Request body</span></span>
<span data-ttu-id="2e1d0-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [organization](../resources/intune-onboarding-organization.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="2e1d0-126">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="2e1d0-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [organization](../resources/intune-onboarding-organization.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2e1d0-127">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="2e1d0-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e1d0-128">Property</span></span>|<span data-ttu-id="2e1d0-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2e1d0-129">Type</span></span>|<span data-ttu-id="2e1d0-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e1d0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e1d0-131">id</span><span class="sxs-lookup"><span data-stu-id="2e1d0-131">id</span></span>|<span data-ttu-id="2e1d0-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2e1d0-132">String</span></span>|<span data-ttu-id="2e1d0-133">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="2e1d0-133">The GUID for the object.</span></span>|
|<span data-ttu-id="2e1d0-134">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="2e1d0-134">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="2e1d0-135">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="2e1d0-135">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="2e1d0-136">Autorität für die Verwaltung mobiler Geräte.</span><span class="sxs-lookup"><span data-stu-id="2e1d0-136">Mobile device management authority.</span></span> <span data-ttu-id="2e1d0-137">Mögliche Werte: `unknown`, `intune`, `sccm` und `office365`.</span><span class="sxs-lookup"><span data-stu-id="2e1d0-137">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="2e1d0-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e1d0-138">Response</span></span>
<span data-ttu-id="2e1d0-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [organization](../resources/intune-onboarding-organization.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e1d0-139">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e1d0-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e1d0-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e1d0-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e1d0-141">Request</span></span>
<span data-ttu-id="2e1d0-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e1d0-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="2e1d0-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e1d0-143">Response</span></span>
<span data-ttu-id="2e1d0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e1d0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune"
}
```



