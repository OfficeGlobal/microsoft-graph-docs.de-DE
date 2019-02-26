---
title: roleAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines roleAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 674a1baeb9f15dfb6eeb601784ed69f4b93c5955
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253225"
---
# <a name="update-roleassignment"></a><span data-ttu-id="3878d-103">roleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3878d-103">Update roleAssignment</span></span>

> <span data-ttu-id="3878d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3878d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3878d-105">Aktualisieren der Eigenschaften eines [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3878d-105">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3878d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3878d-106">Prerequisites</span></span>
<span data-ttu-id="3878d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3878d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3878d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3878d-109">Permission type</span></span>|<span data-ttu-id="3878d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3878d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3878d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3878d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3878d-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3878d-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="3878d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3878d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3878d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3878d-114">Not supported.</span></span>|
|<span data-ttu-id="3878d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3878d-115">Application</span></span>|<span data-ttu-id="3878d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3878d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3878d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3878d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3878d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3878d-118">Request headers</span></span>
|<span data-ttu-id="3878d-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3878d-119">Header</span></span>|<span data-ttu-id="3878d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3878d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3878d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3878d-121">Authorization</span></span>|<span data-ttu-id="3878d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3878d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3878d-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3878d-123">Accept</span></span>|<span data-ttu-id="3878d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3878d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3878d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3878d-125">Request body</span></span>
<span data-ttu-id="3878d-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="3878d-126">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="3878d-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [roleAssignment](../resources/intune-rbac-roleassignment.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3878d-127">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="3878d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3878d-128">Property</span></span>|<span data-ttu-id="3878d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3878d-129">Type</span></span>|<span data-ttu-id="3878d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3878d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3878d-131">id</span><span class="sxs-lookup"><span data-stu-id="3878d-131">id</span></span>|<span data-ttu-id="3878d-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3878d-132">String</span></span>|<span data-ttu-id="3878d-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3878d-133">Key of the entity.</span></span> <span data-ttu-id="3878d-134">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="3878d-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="3878d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3878d-135">displayName</span></span>|<span data-ttu-id="3878d-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3878d-136">String</span></span>|<span data-ttu-id="3878d-137">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="3878d-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="3878d-138">description</span><span class="sxs-lookup"><span data-stu-id="3878d-138">description</span></span>|<span data-ttu-id="3878d-139">String</span><span class="sxs-lookup"><span data-stu-id="3878d-139">String</span></span>|<span data-ttu-id="3878d-140">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="3878d-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="3878d-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="3878d-141">resourceScopes</span></span>|<span data-ttu-id="3878d-142">String collection</span><span class="sxs-lookup"><span data-stu-id="3878d-142">String collection</span></span>|<span data-ttu-id="3878d-143">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="3878d-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="3878d-144">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3878d-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="3878d-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="3878d-145">Response</span></span>
<span data-ttu-id="3878d-146">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3878d-146">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3878d-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3878d-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="3878d-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3878d-148">Request</span></span>
<span data-ttu-id="3878d-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3878d-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="3878d-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="3878d-150">Response</span></span>
<span data-ttu-id="3878d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3878d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```



