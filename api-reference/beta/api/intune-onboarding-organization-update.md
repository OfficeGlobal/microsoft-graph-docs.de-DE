---
title: Organisation aktualisieren
description: Aktualisieren der Eigenschaften eines organization-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0263fc0ddf565da7c01ae8fbc6f9b20cbb405d5c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983617"
---
# <a name="update-organization"></a><span data-ttu-id="38f01-103">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="38f01-103">Update organization</span></span>

> <span data-ttu-id="38f01-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="38f01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38f01-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="38f01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38f01-106">Aktualisieren der Eigenschaften eines [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="38f01-106">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38f01-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="38f01-107">Prerequisites</span></span>
<span data-ttu-id="38f01-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38f01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38f01-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38f01-110">Permission type</span></span>|<span data-ttu-id="38f01-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38f01-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38f01-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38f01-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38f01-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38f01-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="38f01-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38f01-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38f01-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38f01-115">Not supported.</span></span>|
|<span data-ttu-id="38f01-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38f01-116">Application</span></span>|<span data-ttu-id="38f01-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38f01-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38f01-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38f01-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="38f01-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38f01-119">Request headers</span></span>
|<span data-ttu-id="38f01-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="38f01-120">Header</span></span>|<span data-ttu-id="38f01-121">Wert</span><span class="sxs-lookup"><span data-stu-id="38f01-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38f01-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="38f01-122">Authorization</span></span>|<span data-ttu-id="38f01-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="38f01-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38f01-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="38f01-124">Accept</span></span>|<span data-ttu-id="38f01-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38f01-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38f01-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38f01-126">Request body</span></span>
<span data-ttu-id="38f01-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [organization](../resources/intune-onboarding-organization.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="38f01-127">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="38f01-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [organization](../resources/intune-onboarding-organization.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="38f01-128">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="38f01-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="38f01-129">Property</span></span>|<span data-ttu-id="38f01-130">Typ</span><span class="sxs-lookup"><span data-stu-id="38f01-130">Type</span></span>|<span data-ttu-id="38f01-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38f01-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38f01-132">id</span><span class="sxs-lookup"><span data-stu-id="38f01-132">id</span></span>|<span data-ttu-id="38f01-133">String</span><span class="sxs-lookup"><span data-stu-id="38f01-133">String</span></span>|<span data-ttu-id="38f01-134">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="38f01-134">The GUID for the object.</span></span>|
|<span data-ttu-id="38f01-135">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="38f01-135">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="38f01-136">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="38f01-136">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="38f01-137">Autorität für die Verwaltung mobiler Geräte.</span><span class="sxs-lookup"><span data-stu-id="38f01-137">Mobile device management authority.</span></span> <span data-ttu-id="38f01-138">Mögliche Werte: `unknown`, `intune`, `sccm` und `office365`.</span><span class="sxs-lookup"><span data-stu-id="38f01-138">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="38f01-139">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="38f01-139">certificateConnectorSetting</span></span>|[<span data-ttu-id="38f01-140">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="38f01-140">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="38f01-141">Zertifikat-Connector-Einstellung.</span><span class="sxs-lookup"><span data-stu-id="38f01-141">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="38f01-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="38f01-142">Response</span></span>
<span data-ttu-id="38f01-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [organization](../resources/intune-onboarding-organization.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38f01-143">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38f01-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38f01-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="38f01-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38f01-145">Request</span></span>
<span data-ttu-id="38f01-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38f01-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}
Content-type: application/json
Content-length: 492

{
  "@odata.type": "#microsoft.graph.organization",
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

### <a name="response"></a><span data-ttu-id="38f01-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="38f01-147">Response</span></span>
<span data-ttu-id="38f01-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38f01-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




