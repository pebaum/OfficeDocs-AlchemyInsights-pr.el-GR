---
title: Ενεργοποίηση ελέγχου γραμματοκιβωτίου
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506954"
---
# <a name="enable-mailbox-auditing"></a>Ενεργοποίηση ελέγχου γραμματοκιβωτίου

Για να ενεργοποιήσετε τον έλεγχο γραμματοκιβωτίου για έναν μεμονωμένο χρήστη ή για έναν ολόκληρο οργανισμό, τα ακόλουθα cmdlets πρέπει να εκτελούνται από το απομακρυσμένο κέλυφος ενέργειας:
  
 **Μεμονωμένος χρήστης**
  
Set-Γραμματοκιβώτιο -Ταυτότητα "Jane Dow" -ΈλεγχοςΕνεργοποιημένο $true
  
 **Οργάνωση**
  
Get-Γραμματοκιβώτιο -ResultSize Απεριόριστα -Φίλτρο {RecipientTypeDetails -eq "UserMailbox"} | Ορισμός γραμματοκιβωτίου -Ενεργοποίηση ελέγχου $true
  
[Μάθε περισσότερα](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

