---
title: roleAssignment erstellen
description: Erstellen eines neuen roleAssignment-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8a8c889e401664fb0fea66030ff3bcabd0631503
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399913"
---
# <a name="create-roleassignment"></a><span data-ttu-id="f6fe5-103">roleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="f6fe5-103">Create roleAssignment</span></span>

> <span data-ttu-id="f6fe5-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f6fe5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6fe5-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6fe5-107">Erstellen eines neuen [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-107">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6fe5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f6fe5-108">Prerequisites</span></span>
<span data-ttu-id="f6fe5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f6fe5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f6fe5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f6fe5-111">Permission type</span></span>|<span data-ttu-id="f6fe5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f6fe5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6fe5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f6fe5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6fe5-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6fe5-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f6fe5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f6fe5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6fe5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6fe5-116">Not supported.</span></span>|
|<span data-ttu-id="f6fe5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f6fe5-117">Application</span></span>|<span data-ttu-id="f6fe5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6fe5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6fe5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6fe5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="f6fe5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f6fe5-120">Request headers</span></span>
|<span data-ttu-id="f6fe5-121">Header</span><span class="sxs-lookup"><span data-stu-id="f6fe5-121">Header</span></span>|<span data-ttu-id="f6fe5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f6fe5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6fe5-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f6fe5-123">Authorization</span></span>|<span data-ttu-id="f6fe5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f6fe5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6fe5-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f6fe5-125">Accept</span></span>|<span data-ttu-id="f6fe5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6fe5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6fe5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f6fe5-127">Request body</span></span>
<span data-ttu-id="f6fe5-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs roleAssignment an.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-128">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="f6fe5-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der roleAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-129">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="f6fe5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f6fe5-130">Property</span></span>|<span data-ttu-id="f6fe5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f6fe5-131">Type</span></span>|<span data-ttu-id="f6fe5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6fe5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6fe5-133">id</span><span class="sxs-lookup"><span data-stu-id="f6fe5-133">id</span></span>|<span data-ttu-id="f6fe5-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6fe5-134">String</span></span>|<span data-ttu-id="f6fe5-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f6fe5-135">Key of the entity.</span></span> <span data-ttu-id="f6fe5-136">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="f6fe5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f6fe5-137">displayName</span></span>|<span data-ttu-id="f6fe5-138">String</span><span class="sxs-lookup"><span data-stu-id="f6fe5-138">String</span></span>|<span data-ttu-id="f6fe5-139">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="f6fe5-140">description</span><span class="sxs-lookup"><span data-stu-id="f6fe5-140">description</span></span>|<span data-ttu-id="f6fe5-141">String</span><span class="sxs-lookup"><span data-stu-id="f6fe5-141">String</span></span>|<span data-ttu-id="f6fe5-142">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="f6fe5-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="f6fe5-143">scopeMembers</span></span>|<span data-ttu-id="f6fe5-144">String collection</span><span class="sxs-lookup"><span data-stu-id="f6fe5-144">String collection</span></span>|<span data-ttu-id="f6fe5-145">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="f6fe5-146">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="f6fe5-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="f6fe5-147">scopeType</span></span>|[<span data-ttu-id="f6fe5-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="f6fe5-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="f6fe5-149">Gibt den Typ des Bereichs für eine Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="f6fe5-150">Standardtyp 'ResourceScope' ermöglicht die Zuweisung von ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="f6fe5-151">Für 'AllDevices', 'AllLicensedUsers' und 'AllDevicesAndLicensedUsers' sollte die ResourceScopes-Eigenschaft leer bleiben.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="f6fe5-152">Mögliche Werte: sind `resourceScope`, `allDevices`, `allLicensedUsers` und `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="f6fe5-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="f6fe5-153">resourceScopes</span></span>|<span data-ttu-id="f6fe5-154">String collection</span><span class="sxs-lookup"><span data-stu-id="f6fe5-154">String collection</span></span>|<span data-ttu-id="f6fe5-155">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="f6fe5-156">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="f6fe5-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6fe5-157">Response</span></span>
<span data-ttu-id="f6fe5-158">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-158">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6fe5-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f6fe5-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6fe5-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6fe5-160">Request</span></span>
<span data-ttu-id="f6fe5-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f6fe5-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6fe5-162">Response</span></span>
<span data-ttu-id="f6fe5-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6fe5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




