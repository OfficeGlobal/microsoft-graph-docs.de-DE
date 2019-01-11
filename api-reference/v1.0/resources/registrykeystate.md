---
title: Ressourcentyp registryKeyState
description: Enthält Informationen zur Registrierung wichtige Änderungen im Zusammenhang mit der Benachrichtigung, und der Prozess, der die Registrierungsschlüssel geändert.
localization_priority: Normal
ms.openlocfilehash: 688c690083e24dc6c8ee7229498910befd0fdf3e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884826"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="dc5e2-103">Ressourcentyp registryKeyState</span><span class="sxs-lookup"><span data-stu-id="dc5e2-103">registryKeyState resource type</span></span>

<span data-ttu-id="dc5e2-104">Enthält Informationen zur Registrierung wichtige Änderungen im Zusammenhang mit der Benachrichtigung, und der Prozess, der die Registrierungsschlüssel geändert.</span><span class="sxs-lookup"><span data-stu-id="dc5e2-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="dc5e2-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dc5e2-105">Properties</span></span>

| <span data-ttu-id="dc5e2-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dc5e2-106">Property</span></span>     | <span data-ttu-id="dc5e2-107">Typ</span><span class="sxs-lookup"><span data-stu-id="dc5e2-107">Type</span></span>        | <span data-ttu-id="dc5e2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dc5e2-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dc5e2-109">Struktur</span><span class="sxs-lookup"><span data-stu-id="dc5e2-109">hive</span></span>|<span data-ttu-id="dc5e2-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="dc5e2-110">registryHive</span></span>|<span data-ttu-id="dc5e2-111">Ein [Windows-Registrierungsstruktur](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span><span class="sxs-lookup"><span data-stu-id="dc5e2-111">A [Windows registry hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="dc5e2-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="dc5e2-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="dc5e2-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="dc5e2-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="dc5e2-114">HKEY_LOCAL_MACHINE\SAM</span><span class="sxs-lookup"><span data-stu-id="dc5e2-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="dc5e2-115">HKEY_LOCAL_MACHINE\Security</span><span class="sxs-lookup"><span data-stu-id="dc5e2-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="dc5e2-116">HKEY_LOCAL_MACHINE\Software</span><span class="sxs-lookup"><span data-stu-id="dc5e2-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="dc5e2-117">HKEY_LOCAL_MACHINE\SYSTEM</span><span class="sxs-lookup"><span data-stu-id="dc5e2-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="dc5e2-118">HKEY_USERS\\. Die standardmäßigen.</span><span class="sxs-lookup"><span data-stu-id="dc5e2-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="dc5e2-119">Mögliche Werte sind: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem` und `usersDefault`.</span><span class="sxs-lookup"><span data-stu-id="dc5e2-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="dc5e2-120">Key</span><span class="sxs-lookup"><span data-stu-id="dc5e2-120">key</span></span>|<span data-ttu-id="dc5e2-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dc5e2-121">String</span></span>|<span data-ttu-id="dc5e2-122">Aktuelle (d. h. geänderten) Registrierungsschlüssel (schließt die Struktur).</span><span class="sxs-lookup"><span data-stu-id="dc5e2-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="dc5e2-123">oldKey</span><span class="sxs-lookup"><span data-stu-id="dc5e2-123">oldKey</span></span>|<span data-ttu-id="dc5e2-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dc5e2-124">String</span></span>|<span data-ttu-id="dc5e2-125">Frühere (d. h., bevor geändert) Registrierungsschlüssel (schließt die Struktur).</span><span class="sxs-lookup"><span data-stu-id="dc5e2-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="dc5e2-126">oldValueData</span><span class="sxs-lookup"><span data-stu-id="dc5e2-126">oldValueData</span></span>|<span data-ttu-id="dc5e2-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dc5e2-127">String</span></span>|<span data-ttu-id="dc5e2-128">Frühere (d. h., bevor geändert) Schlüsselwert Registrierungsdaten (Inhalt).</span><span class="sxs-lookup"><span data-stu-id="dc5e2-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="dc5e2-129">oldValueName</span><span class="sxs-lookup"><span data-stu-id="dc5e2-129">oldValueName</span></span>|<span data-ttu-id="dc5e2-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dc5e2-130">String</span></span>|<span data-ttu-id="dc5e2-131">Frühere (d. h., bevor geändert) Registrierung Schlüsselwertname.</span><span class="sxs-lookup"><span data-stu-id="dc5e2-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="dc5e2-132">Operation</span><span class="sxs-lookup"><span data-stu-id="dc5e2-132">operation</span></span>|<span data-ttu-id="dc5e2-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="dc5e2-133">registryOperation</span></span>|<span data-ttu-id="dc5e2-134">Der Vorgang, der der Name des Registrierungsschlüssels und/oder Wert geändert.</span><span class="sxs-lookup"><span data-stu-id="dc5e2-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="dc5e2-135">Mögliche Werte: sind `unknown`, `create`, `modify` und `delete`.</span><span class="sxs-lookup"><span data-stu-id="dc5e2-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="dc5e2-136">processId</span><span class="sxs-lookup"><span data-stu-id="dc5e2-136">processId</span></span>|<span data-ttu-id="dc5e2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="dc5e2-137">Int32</span></span>|<span data-ttu-id="dc5e2-138">Werden Sie ID (PID) des Prozesses, der den Registrierungsschlüssel (Prozess, der in der Auflistung Warnung 'Prozesse' Details angezeigt werden) geändert.</span><span class="sxs-lookup"><span data-stu-id="dc5e2-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="dc5e2-139">valueData</span><span class="sxs-lookup"><span data-stu-id="dc5e2-139">valueData</span></span>|<span data-ttu-id="dc5e2-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dc5e2-140">String</span></span>|<span data-ttu-id="dc5e2-141">Aktuelle (d. h. geänderten) Schlüsselwert Registrierungsdaten (Inhalt).</span><span class="sxs-lookup"><span data-stu-id="dc5e2-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="dc5e2-142">Wertname</span><span class="sxs-lookup"><span data-stu-id="dc5e2-142">valueName</span></span>|<span data-ttu-id="dc5e2-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dc5e2-143">String</span></span>|<span data-ttu-id="dc5e2-144">Aktuelle (d. h. geänderten) Registrierung Schlüsselwertname</span><span class="sxs-lookup"><span data-stu-id="dc5e2-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="dc5e2-145">Werttyp</span><span class="sxs-lookup"><span data-stu-id="dc5e2-145">valueType</span></span>|<span data-ttu-id="dc5e2-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="dc5e2-146">registryValueType</span></span>|[<span data-ttu-id="dc5e2-147">Schlüsselwert Registrierungstyp</span><span class="sxs-lookup"><span data-stu-id="dc5e2-147">Registry key value type</span></span>](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="dc5e2-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="dc5e2-148">REG_BINARY</span></span></li> <li><span data-ttu-id="dc5e2-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="dc5e2-149">REG_DWORD</span></span></li> <li><span data-ttu-id="dc5e2-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="dc5e2-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="dc5e2-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="dc5e2-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="dc5e2-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="dc5e2-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="dc5e2-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="dc5e2-153">REG_LINK</span></span></li> <li><span data-ttu-id="dc5e2-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="dc5e2-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="dc5e2-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="dc5e2-155">REG_NONE</span></span></li> <li><span data-ttu-id="dc5e2-156">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="dc5e2-156">REG_QWORD</span></span></li> <li><span data-ttu-id="dc5e2-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="dc5e2-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="dc5e2-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="dc5e2-158">REG_SZ</span></span></li></ul> <span data-ttu-id="dc5e2-159">Mögliche Werte sind: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian` und `sz`.</span><span class="sxs-lookup"><span data-stu-id="dc5e2-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc5e2-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dc5e2-160">JSON representation</span></span>

<span data-ttu-id="dc5e2-161">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dc5e2-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
