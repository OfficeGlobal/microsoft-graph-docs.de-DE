---
title: Organisation aktualisieren
description: Aktualisieren der Eigenschaften eines organization-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 67ce9fd0181c3f60f3615a29313e2da642e697ab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862146"
---
# <a name="update-organization"></a><span data-ttu-id="c0be8-103">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c0be8-103">Update organization</span></span>

> <span data-ttu-id="c0be8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c0be8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0be8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0be8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0be8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c0be8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0be8-107">Aktualisieren der Eigenschaften eines [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c0be8-107">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0be8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c0be8-108">Prerequisites</span></span>
<span data-ttu-id="c0be8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0be8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0be8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0be8-111">Permission type</span></span>|<span data-ttu-id="c0be8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0be8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0be8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0be8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0be8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0be8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c0be8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0be8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0be8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0be8-116">Not supported.</span></span>|
|<span data-ttu-id="c0be8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0be8-117">Application</span></span>|<span data-ttu-id="c0be8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0be8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0be8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0be8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="c0be8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0be8-120">Request headers</span></span>
|<span data-ttu-id="c0be8-121">Header</span><span class="sxs-lookup"><span data-stu-id="c0be8-121">Header</span></span>|<span data-ttu-id="c0be8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c0be8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0be8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0be8-123">Authorization</span></span>|<span data-ttu-id="c0be8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c0be8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0be8-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c0be8-125">Accept</span></span>|<span data-ttu-id="c0be8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0be8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0be8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0be8-127">Request body</span></span>
<span data-ttu-id="c0be8-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [organization](../resources/intune-onboarding-organization.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c0be8-128">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="c0be8-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [organization](../resources/intune-onboarding-organization.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c0be8-129">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="c0be8-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c0be8-130">Property</span></span>|<span data-ttu-id="c0be8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c0be8-131">Type</span></span>|<span data-ttu-id="c0be8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0be8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0be8-133">id</span><span class="sxs-lookup"><span data-stu-id="c0be8-133">id</span></span>|<span data-ttu-id="c0be8-134">String</span><span class="sxs-lookup"><span data-stu-id="c0be8-134">String</span></span>|<span data-ttu-id="c0be8-135">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="c0be8-135">The GUID for the object.</span></span>|
|<span data-ttu-id="c0be8-136">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="c0be8-136">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="c0be8-137">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="c0be8-137">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="c0be8-138">Autorität für die Verwaltung mobiler Geräte.</span><span class="sxs-lookup"><span data-stu-id="c0be8-138">Mobile device management authority.</span></span> <span data-ttu-id="c0be8-139">Mögliche Werte: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="c0be8-139">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="c0be8-140">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="c0be8-140">certificateConnectorSetting</span></span>|[<span data-ttu-id="c0be8-141">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="c0be8-141">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="c0be8-142">Connector-Einstellung Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="c0be8-142">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="c0be8-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0be8-143">Response</span></span>
<span data-ttu-id="c0be8-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [organization](../resources/intune-onboarding-organization.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0be8-144">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0be8-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0be8-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0be8-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0be8-146">Request</span></span>
<span data-ttu-id="c0be8-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0be8-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}
Content-type: application/json
Content-length: 441

{
  "mobileDeviceManagementAuthority": "intune",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 6,
    "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
    "enrollmentError": "Enrollment Error value",
    "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
    "connectorVersion": "Connector Version value",
    "lastUploadVersion": 1
  }
}
```

### <a name="response"></a><span data-ttu-id="c0be8-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0be8-148">Response</span></span>
<span data-ttu-id="c0be8-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0be8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 541

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 6,
    "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
    "enrollmentError": "Enrollment Error value",
    "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
    "connectorVersion": "Connector Version value",
    "lastUploadVersion": 1
  }
}
```





