---
title: TermsAndConditionsGroupAssignment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines TermsAndConditionsGroupAssignment-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ea202d33028d9eff66e06030d3049f4d6fa7aef1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393753"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="177f6-103">TermsAndConditionsGroupAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="177f6-103">Update termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="177f6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="177f6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="177f6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="177f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="177f6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="177f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="177f6-107">Aktualisieren Sie die Eigenschaften eines [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="177f6-107">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="177f6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="177f6-108">Prerequisites</span></span>
<span data-ttu-id="177f6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="177f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="177f6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="177f6-111">Permission type</span></span>|<span data-ttu-id="177f6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="177f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="177f6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="177f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="177f6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="177f6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="177f6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="177f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="177f6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="177f6-116">Not supported.</span></span>|
|<span data-ttu-id="177f6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="177f6-117">Application</span></span>|<span data-ttu-id="177f6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="177f6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="177f6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="177f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="177f6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="177f6-120">Request headers</span></span>
|<span data-ttu-id="177f6-121">Header</span><span class="sxs-lookup"><span data-stu-id="177f6-121">Header</span></span>|<span data-ttu-id="177f6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="177f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="177f6-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="177f6-123">Authorization</span></span>|<span data-ttu-id="177f6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="177f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="177f6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="177f6-125">Accept</span></span>|<span data-ttu-id="177f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="177f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="177f6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="177f6-127">Request body</span></span>
<span data-ttu-id="177f6-128">Geben Sie im Textkörper Anforderung für das Objekt [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="177f6-128">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="177f6-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="177f6-129">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="177f6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="177f6-130">Property</span></span>|<span data-ttu-id="177f6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="177f6-131">Type</span></span>|<span data-ttu-id="177f6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="177f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="177f6-133">id</span><span class="sxs-lookup"><span data-stu-id="177f6-133">id</span></span>|<span data-ttu-id="177f6-134">String</span><span class="sxs-lookup"><span data-stu-id="177f6-134">String</span></span>|<span data-ttu-id="177f6-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="177f6-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="177f6-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="177f6-136">targetGroupId</span></span>|<span data-ttu-id="177f6-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="177f6-137">String</span></span>|<span data-ttu-id="177f6-138">Eindeutiger Bezeichner der einer Gruppe, der die T&C Richtlinie zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="177f6-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="177f6-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="177f6-139">Response</span></span>
<span data-ttu-id="177f6-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="177f6-140">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="177f6-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="177f6-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="177f6-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="177f6-142">Request</span></span>
<span data-ttu-id="177f6-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="177f6-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="177f6-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="177f6-144">Response</span></span>
<span data-ttu-id="177f6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="177f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 169

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
  "targetGroupId": "Target Group Id value"
}
```




