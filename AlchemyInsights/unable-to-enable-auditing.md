---
title: 2419-ανίκανος-να-ενεργοποίηση-έλεγχος
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510428"
---
# <a name="unable-to-enable-unified-auditing"></a>Δεν είναι δυνατή η ενεργοποίηση ενοποιημένου ελέγχου

Όταν προσπαθείτε να ενεργοποιήσετε τον ενοποιημένο έλεγχο για τον οργανισμό σας, ενδέχεται να λάβετε ένα σφάλμα παρόμοιο με το ακόλουθο:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Για να επιλύσετε αυτό το ζήτημα, ακολουθήστε τα εξής βήματα:

1. [Σύνδεση στο Ηλεκτρονικό Powershell του Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Εκτελέστε το ακόλουθο cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Περιμένετε 60 λεπτά για να τεθεί σε ισχύ η προηγούμενη ρύθμιση.

4. Εκτελέστε την ακόλουθη εντολή στο Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Για περισσότερες πληροφορίες, ανατρέξτε στα ακόλουθα άρθρα:

- [Σύνδεση στο Exchange Online PowerShell με χρήση ελέγχου ταυτότητας πολλών παραγόντων](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Ενεργοποίηση ή απενεργοποίηση της αναζήτησης καταγραφής ελέγχου](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
