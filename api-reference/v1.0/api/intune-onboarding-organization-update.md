---
title: Organisation aktualisieren
description: Aktualisieren der Eigenschaften eines organization-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b639ff8d3a2d043bd001f160a0c04ca97a11dbba
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258485"
---
# <a name="update-organization"></a><span data-ttu-id="db035-103">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="db035-103">Update organization</span></span>

> <span data-ttu-id="db035-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="db035-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db035-105">Aktualisieren der Eigenschaften eines [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="db035-105">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db035-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="db035-106">Prerequisites</span></span>
<span data-ttu-id="db035-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="db035-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="db035-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="db035-109">Permission type</span></span>|<span data-ttu-id="db035-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="db035-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db035-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="db035-111">Delegated (work or school account)</span></span>|<span data-ttu-id="db035-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db035-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="db035-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="db035-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db035-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db035-114">Not supported.</span></span>|
|<span data-ttu-id="db035-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="db035-115">Application</span></span>|<span data-ttu-id="db035-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db035-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db035-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="db035-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="db035-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="db035-118">Request headers</span></span>
|<span data-ttu-id="db035-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="db035-119">Header</span></span>|<span data-ttu-id="db035-120">Wert</span><span class="sxs-lookup"><span data-stu-id="db035-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db035-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="db035-121">Authorization</span></span>|<span data-ttu-id="db035-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="db035-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db035-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="db035-123">Accept</span></span>|<span data-ttu-id="db035-124">application/json</span><span class="sxs-lookup"><span data-stu-id="db035-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db035-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="db035-125">Request body</span></span>
<span data-ttu-id="db035-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [organization](../resources/intune-onboarding-organization.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="db035-126">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="db035-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [organization](../resources/intune-onboarding-organization.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="db035-127">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="db035-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="db035-128">Property</span></span>|<span data-ttu-id="db035-129">Typ</span><span class="sxs-lookup"><span data-stu-id="db035-129">Type</span></span>|<span data-ttu-id="db035-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="db035-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db035-131">id</span><span class="sxs-lookup"><span data-stu-id="db035-131">id</span></span>|<span data-ttu-id="db035-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="db035-132">String</span></span>|<span data-ttu-id="db035-133">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="db035-133">The GUID for the object.</span></span>|
|<span data-ttu-id="db035-134">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="db035-134">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="db035-135">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="db035-135">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="db035-136">Autorität für die Verwaltung mobiler Geräte.</span><span class="sxs-lookup"><span data-stu-id="db035-136">Mobile device management authority.</span></span> <span data-ttu-id="db035-137">Mögliche Werte: `unknown`, `intune`, `sccm` und `office365`.</span><span class="sxs-lookup"><span data-stu-id="db035-137">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="db035-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="db035-138">Response</span></span>
<span data-ttu-id="db035-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [organization](../resources/intune-onboarding-organization.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="db035-139">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db035-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="db035-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="db035-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="db035-141">Request</span></span>
<span data-ttu-id="db035-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="db035-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="db035-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="db035-143">Response</span></span>
<span data-ttu-id="db035-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="db035-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



