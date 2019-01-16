---
title: Ερωτήσεις σχετικά με τον τρόπο χρήσης του Office ανάπτυξης Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28290365"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Ερωτήσεις σχετικά με τον τρόπο χρήσης του Office ανάπτυξης Tool (ODT)

Κάντε λήψη του εργαλείου ανάπτυξης του Office από το [Κέντρο λήψης της Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Μετά τη λήψη του αρχείου, εκτελέστε το αυτοαποσυμπιεζόμενο εκτελέσιμο αρχείο, που περιέχει το Office εργαλείο ανάπτυξης εκτελέσιμο (setup.exe) και ένα αρχείο ρύθμισης παραμέτρων δείγματος (configuration.xml).
  
 **Για να αποκλείσετε ή να καταργήσετε τα προϊόντα του Office 365 ProPlus από υπολογιστές-πελάτες:**
  
Κατά την εγκατάσταση του Office 365 ProPlus, μπορείτε να εξαιρέσετε συγκεκριμένα προϊόντα. Για να γίνει αυτό, ακολουθήστε τα βήματα για την εγκατάσταση του Office με το ODT, αλλά περιλαμβάνει το στοιχείο ExcludeApp στο αρχείο ρύθμισης παραμέτρων. Για παράδειγμα, αυτό το αρχείο παραμέτρων εγκαθιστά όλα τα προϊόντα του Office 365 ProPlus εκτός από το Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Επισκόπηση του εργαλείου ανάπτυξης του Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  
