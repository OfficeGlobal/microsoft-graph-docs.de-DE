---
title: roleAssignment erstellen
description: Erstellen eines neuen roleAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 455d8ec127b1e86ffe1bfc319a94a973e9c40a2f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979921"
---
# <a name="create-roleassignment"></a><span data-ttu-id="e1a37-103">roleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="e1a37-103">Create roleAssignment</span></span>

> <span data-ttu-id="e1a37-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e1a37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1a37-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e1a37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1a37-106">Erstellen eines neuen [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e1a37-106">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1a37-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e1a37-107">Prerequisites</span></span>
<span data-ttu-id="e1a37-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1a37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1a37-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1a37-110">Permission type</span></span>|<span data-ttu-id="e1a37-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1a37-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1a37-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1a37-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1a37-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1a37-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="e1a37-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1a37-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1a37-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1a37-115">Not supported.</span></span>|
|<span data-ttu-id="e1a37-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1a37-116">Application</span></span>|<span data-ttu-id="e1a37-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1a37-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1a37-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1a37-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="e1a37-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1a37-119">Request headers</span></span>
|<span data-ttu-id="e1a37-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e1a37-120">Header</span></span>|<span data-ttu-id="e1a37-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e1a37-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1a37-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1a37-122">Authorization</span></span>|<span data-ttu-id="e1a37-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e1a37-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1a37-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e1a37-124">Accept</span></span>|<span data-ttu-id="e1a37-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e1a37-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1a37-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1a37-126">Request body</span></span>
<span data-ttu-id="e1a37-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs roleAssignment an.</span><span class="sxs-lookup"><span data-stu-id="e1a37-127">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="e1a37-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der roleAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e1a37-128">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="e1a37-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1a37-129">Property</span></span>|<span data-ttu-id="e1a37-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e1a37-130">Type</span></span>|<span data-ttu-id="e1a37-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1a37-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1a37-132">id</span><span class="sxs-lookup"><span data-stu-id="e1a37-132">id</span></span>|<span data-ttu-id="e1a37-133">String</span><span class="sxs-lookup"><span data-stu-id="e1a37-133">String</span></span>|<span data-ttu-id="e1a37-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e1a37-134">Key of the entity.</span></span> <span data-ttu-id="e1a37-135">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="e1a37-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="e1a37-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e1a37-136">displayName</span></span>|<span data-ttu-id="e1a37-137">String</span><span class="sxs-lookup"><span data-stu-id="e1a37-137">String</span></span>|<span data-ttu-id="e1a37-138">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="e1a37-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="e1a37-139">description</span><span class="sxs-lookup"><span data-stu-id="e1a37-139">description</span></span>|<span data-ttu-id="e1a37-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1a37-140">String</span></span>|<span data-ttu-id="e1a37-141">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="e1a37-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="e1a37-142">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="e1a37-142">scopeMembers</span></span>|<span data-ttu-id="e1a37-143">String collection</span><span class="sxs-lookup"><span data-stu-id="e1a37-143">String collection</span></span>|<span data-ttu-id="e1a37-144">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="e1a37-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="e1a37-145">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e1a37-145">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="e1a37-146">scopeType</span><span class="sxs-lookup"><span data-stu-id="e1a37-146">scopeType</span></span>|[<span data-ttu-id="e1a37-147">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="e1a37-147">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="e1a37-148">Gibt den Typ des Bereichs für eine Rollenzuweisung an.</span><span class="sxs-lookup"><span data-stu-id="e1a37-148">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="e1a37-149">Der Standardtyp "ResourceScope" ermöglicht die Zuweisung von ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="e1a37-149">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="e1a37-150">Für "allDevices", "AllLicensedUsers" und "AllDevicesAndLicensedUsers" sollte die ResourceScopes-Eigenschaft leer bleiben.</span><span class="sxs-lookup"><span data-stu-id="e1a37-150">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="e1a37-151">Mögliche Werte sind: `resourceScope`, `allDevices`, `allLicensedUsers` und `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="e1a37-151">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="e1a37-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="e1a37-152">resourceScopes</span></span>|<span data-ttu-id="e1a37-153">String collection</span><span class="sxs-lookup"><span data-stu-id="e1a37-153">String collection</span></span>|<span data-ttu-id="e1a37-154">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="e1a37-154">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="e1a37-155">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e1a37-155">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="e1a37-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1a37-156">Response</span></span>
<span data-ttu-id="e1a37-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e1a37-157">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1a37-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1a37-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1a37-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1a37-159">Request</span></span>
<span data-ttu-id="e1a37-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1a37-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
Content-type: application/json
Content-length: 277

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="e1a37-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1a37-161">Response</span></span>
<span data-ttu-id="e1a37-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1a37-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 326

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```




