---
description: Leer hoe u klantkenmerkgegevens uploadt via FTP naar Experience Cloud.
solution: Experience Cloud
title: Upload het bestand met kenmerkgegevens van de klant via FTP
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: ed9e4a8f-493a-4a0f-a87e-674c7da95b99
source-git-commit: c39672f0d8a0fd353b275b2ecd095ada1e2bf744
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Optioneel - Het gegevensbestand uploaden via FTP

Als u niet uploadt via slepen en neerzetten, kunt u gegevens van kenmerk Klant uploaden via FTP naar Experience Cloud.

U kunt de gegevens uploaden nadat u een bron van Kenmerken van de Klant en een rekening van FTP in Experience Cloud creeert. U maakt één FTP-account per kenmerkbron. De geüploade bestanden worden opgeslagen in de hoofdmap van dat account. De gegevens moeten in `.csv` formaat, met een tweede formaat `.fin` om aan te geven dat het uploaden is voltooid.

>[!IMPORTANT]
>
>Controleren [Gegevensbestandsvereisten voor het uploaden van klantkenmerken](crs-data-file.md) voordat u het bestand uploadt.

Het uploaden van bestanden naar de FTP-site met klantkenmerken kan worden uitgevoerd via FTP of SFTP:

* U hebt een client nodig die SFTP-verbindingen ondersteunt.
* U kunt verbinding maken met SFTP via gebruikersnaam/wachtwoord of zonder wachtwoord, zoals beschreven [hier](https://experienceleague.adobe.com/docs/analytics/export/ftp-and-sftp/secure-file-transfer-protocol/ftp-sftp-cert-auth.html).

**Het gegevensbestand uploaden via FTP**

1. [Een bron voor klantkenmerken maken en het gegevensbestand uploaden...](t-crs-usecase.md).

   Controleer of u bent aangemeld bij uw FTP-site op `ftp.adobe.com/<sftpname>`.

1. Selecteren **[!UICONTROL Actions]** > **[!UICONTROL File Upload]**.

1. Een `.fin` zodat het bestand kan worden opgehaald.

   Het bestandstype `.fin` is door de gebruiker gemaakt en geeft aan dat het uploaden is voltooid. Het kan een leeg notebookbestand zijn. Als u bijvoorbeeld uploadt `crs123.csv`, uploadt u ook `crs123.fin`.

   Als het uploaden is voltooid, worden beide bestanden verplaatst naar een map met de naam **verwerkt**.

   Zie [Gegevensbestandsvereisten voor het uploaden van klantkenmerken](crs-data-file.md) voor belangrijke informatie over bestandsnamen en -structuur.
