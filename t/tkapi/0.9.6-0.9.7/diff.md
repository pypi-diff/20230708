# Comparing `tmp/tkapi-0.9.6.tar.gz` & `tmp/tkapi-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tkapi-0.9.6.tar", last modified: Fri Dec 20 15:22:40 2019, max compression
+gzip compressed data, was "tkapi-0.9.7.tar", last modified: Sat Jul  8 13:37:15 2023, max compression
```

## Comparing `tkapi-0.9.6.tar` & `tkapi-0.9.7.tar`

### file list

```diff
@@ -1,36 +1,56 @@
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2019-12-20 15:22:40.000000 tkapi-0.9.6/
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2019-12-20 15:22:40.000000 tkapi-0.9.6/tkapi/
--rw-rw-r--   0 bart      (1000) bart      (1000)     8757 2019-12-14 11:20:46.000000 tkapi-0.9.6/tkapi/persoon.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1951 2019-12-13 23:34:14.000000 tkapi-0.9.6/tkapi/dossier.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      723 2019-12-13 22:46:47.000000 tkapi-0.9.6/tkapi/info.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    12925 2019-12-20 15:17:04.000000 tkapi-0.9.6/tkapi/document.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      845 2019-09-27 13:55:07.000000 tkapi-0.9.6/tkapi/order.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     5390 2019-12-14 11:43:11.000000 tkapi-0.9.6/tkapi/core.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1175 2019-12-13 23:16:18.000000 tkapi-0.9.6/tkapi/kamervraag.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1129 2019-12-07 16:23:49.000000 tkapi-0.9.6/tkapi/verslag.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8932 2019-12-14 11:13:11.000000 tkapi-0.9.6/tkapi/zaak.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     7155 2019-12-14 10:29:09.000000 tkapi-0.9.6/tkapi/activiteit.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     6460 2019-12-14 00:09:27.000000 tkapi-0.9.6/tkapi/commissie.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2010 2019-12-13 23:18:42.000000 tkapi-0.9.6/tkapi/stemming.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1242 2019-12-14 00:08:02.000000 tkapi-0.9.6/tkapi/agendapunt.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3083 2019-12-07 16:10:08.000000 tkapi-0.9.6/tkapi/filter.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1779 2019-12-13 23:38:51.000000 tkapi-0.9.6/tkapi/besluit.py
--rw-rw-r--   0 bart      (1000) bart      (1000)       25 2019-12-13 22:59:19.000000 tkapi-0.9.6/tkapi/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2019-12-20 15:22:40.000000 tkapi-0.9.6/tkapi/util/
--rw-rw-r--   0 bart      (1000) bart      (1000)     2431 2019-12-08 11:39:14.000000 tkapi-0.9.6/tkapi/util/document.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      766 2019-12-13 22:56:31.000000 tkapi-0.9.6/tkapi/util/util.py
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2018-10-26 17:21:37.000000 tkapi-0.9.6/tkapi/util/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     6653 2019-12-13 22:46:47.000000 tkapi-0.9.6/tkapi/util/queries.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1705 2019-12-14 11:16:59.000000 tkapi-0.9.6/tkapi/vergadering.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8569 2019-12-20 15:17:04.000000 tkapi-0.9.6/tkapi/tkapi.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     5773 2019-12-14 11:22:30.000000 tkapi-0.9.6/tkapi/fractie.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2019-12-20 15:22:40.000000 tkapi-0.9.6/tkapi.egg-info/
--rw-rw-r--   0 bart      (1000) bart      (1000)      576 2019-12-20 15:22:40.000000 tkapi-0.9.6/tkapi.egg-info/SOURCES.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)     4617 2019-12-20 15:22:40.000000 tkapi-0.9.6/tkapi.egg-info/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)        1 2019-12-20 15:22:40.000000 tkapi-0.9.6/tkapi.egg-info/dependency_links.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        6 2019-12-20 15:22:40.000000 tkapi-0.9.6/tkapi.egg-info/top_level.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)       38 2019-12-20 15:22:40.000000 tkapi-0.9.6/tkapi.egg-info/requires.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)     4617 2019-12-20 15:22:40.000000 tkapi-0.9.6/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)      790 2019-12-20 15:19:27.000000 tkapi-0.9.6/setup.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3519 2019-12-14 12:23:28.000000 tkapi-0.9.6/README.md
--rw-rw-r--   0 bart      (1000) bart      (1000)       38 2019-12-20 15:22:40.000000 tkapi-0.9.6/setup.cfg
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-08 13:37:15.977025 tkapi-0.9.7/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1089 2023-07-04 18:25:05.000000 tkapi-0.9.7/LICENSE.md
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3892 2023-07-08 13:37:15.977025 tkapi-0.9.7/PKG-INFO
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3416 2023-07-04 18:43:30.000000 tkapi-0.9.7/README.md
+-rw-rw-r--   0 bart      (1000) bart      (1000)       38 2023-07-08 13:37:15.977025 tkapi-0.9.7/setup.cfg
+-rw-rw-r--   0 bart      (1000) bart      (1000)      790 2023-07-08 13:30:26.000000 tkapi-0.9.7/setup.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-08 13:37:15.973025 tkapi-0.9.7/tests/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5251 2023-07-04 19:08:18.000000 tkapi-0.9.7/tests/test_activiteit.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      908 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_agendapunt.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      544 2023-07-04 19:18:37.000000 tkapi-0.9.7/tests/test_api.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2786 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_besluit.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    10543 2023-07-04 19:50:01.000000 tkapi-0.9.7/tests/test_commissie.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     8527 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_document.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7735 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_dossier.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      628 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_filter.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5067 2023-07-04 19:45:35.000000 tkapi-0.9.7/tests/test_fractie.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4298 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_kamervraag.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2515 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_metadata.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1743 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_order.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    10095 2023-07-04 19:04:13.000000 tkapi-0.9.7/tests/test_persoon.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4826 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_stemming.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5688 2023-07-04 19:42:49.000000 tkapi-0.9.7/tests/test_util.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2023 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_vergadering.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1542 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_verslag.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     8328 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_zaak.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-08 13:37:15.977025 tkapi-0.9.7/tkapi/
+-rw-rw-r--   0 bart      (1000) bart      (1000)       25 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7420 2023-07-04 18:32:51.000000 tkapi-0.9.7/tkapi/activiteit.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1808 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/agendapunt.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1779 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/besluit.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     6452 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/commissie.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5390 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/core.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    12973 2023-07-04 18:47:45.000000 tkapi-0.9.7/tkapi/document.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1951 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/dossier.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3193 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/filter.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5852 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/fractie.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      723 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/info.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1175 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/kamervraag.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      845 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/order.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     8757 2023-07-04 19:03:47.000000 tkapi-0.9.7/tkapi/persoon.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2010 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/stemming.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     8500 2023-07-04 19:42:02.000000 tkapi-0.9.7/tkapi/tkapi.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-08 13:37:15.977025 tkapi-0.9.7/tkapi/util/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/util/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2431 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/util/document.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     6653 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/util/queries.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      766 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/util/util.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1929 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/vergadering.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1146 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/verslag.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     9224 2023-07-04 18:55:53.000000 tkapi-0.9.7/tkapi/zaak.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-08 13:37:15.977025 tkapi-0.9.7/tkapi.egg-info/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3892 2023-07-08 13:37:15.000000 tkapi-0.9.7/tkapi.egg-info/PKG-INFO
+-rw-rw-r--   0 bart      (1000) bart      (1000)      988 2023-07-08 13:37:15.000000 tkapi-0.9.7/tkapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)        1 2023-07-08 13:37:15.000000 tkapi-0.9.7/tkapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)       38 2023-07-08 13:37:15.000000 tkapi-0.9.7/tkapi.egg-info/requires.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)        6 2023-07-08 13:37:15.000000 tkapi-0.9.7/tkapi.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tkapi-0.9.6/tkapi/persoon.py` & `tkapi-0.9.7/tkapi/persoon.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,15 +341,15 @@
         return 'Datum'
 
 
 class PersoonContactinformatieSoort(Enum):
     EMAIL = 'E-mail'
     FACEBOOK = 'Facebook'
     INSTAGRAM = 'Instagram'
-    LINKEDIN = 'Linkedin'
+    LINKEDIN = 'LinkedIn'
     TWITTER = 'Twitter'
     WEBSITE = 'Website'
 
 
 class PersoonContactinformatie(PersoonEntity):
     type = 'PersoonContactinformatie'
```

### Comparing `tkapi-0.9.6/tkapi/dossier.py` & `tkapi-0.9.7/tkapi/dossier.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.6/tkapi/info.py` & `tkapi-0.9.7/tkapi/info.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.6/tkapi/document.py` & `tkapi-0.9.7/tkapi/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     ADVIES_AFDELING_ADVISERING_RAAD_VAN_STATE_EN_REACTIE_VAN_DE_INITIATIEFNEMERS = 'Advies Afdeling advisering Raad van State en Reactie van de initiatiefnemer(s)'
     ADVIES_COMMISSIE = 'Advies commissie'
     ADVIES_VAN_ANDERE_ADVIESORGANEN = 'Advies van andere adviesorganen'
     ADVIESAANVRAAG_AFDELING_ADVISERING_RAAD_VAN_STATE = 'Adviesaanvraag Afdeling advisering Raad van State'
     AGENDA_PLENAIRE_VERGADERING = 'Agenda plenaire vergadering'
     AGENDA_PROCEDUREVERGADERING = 'Agenda procedurevergadering'
     AMENDEMENT = 'Amendement'
+    AMENDEMENT_GEWIJZIGD = 'Amendement (gewijzigd/nader/vervangend)'
     ANTWOORD_SCHRIFTELIJKE_VRAGEN = 'Antwoord schriftelijke vragen'
     ANTWOORD_SCHRIFTELIJKE_VRAGEN_NADER = 'Antwoord schriftelijke vragen (nader)'
     BEGROTINGSTOELICHTING = 'Begrotingstoelichting'
     BESLUITENLIJST_PROCEDUREVERGADERING = 'Besluitenlijst procedurevergadering'
     BIJGEWERKTE_TEKST = 'Bijgewerkte tekst'
     BIJLAGE = 'Bijlage'
     BRIEF_AFDELING_ADVISERING_RAAD_VAN_STATE = 'Brief Afdeling advisering Raad van State'
@@ -119,19 +120,19 @@
         self.add_filter_str(filter_str)
 
     def filter_has_activiteit(self):
         filter_str = 'Activiteit/any(a:a ne null)'
         self.add_filter_str(filter_str)
 
     def filter_onderwerp(self, onderwerp: str):
-        filter_str = 'Onderwerp eq ' + "'" + onderwerp.replace("'", "''") + "'"
+        filter_str = "Onderwerp eq '{}'".format(self.escape(onderwerp))
         self.add_filter_str(filter_str)
 
     def filter_titel(self, titel: str):
-        filter_str = 'Titel eq ' + "'" + titel.replace("'", "''") + "'"
+        filter_str = "Titel eq '{}'".format(self.escape(titel))
         self.add_filter_str(filter_str)
 
     def filter_aanhangselnummer(self, aanhangselnummer):
         filter_str = "Aanhangselnummer eq '{}'".format(aanhangselnummer)
         self.add_filter_str(filter_str)
 
     def filter_nummer(self, documentnummer):
@@ -297,15 +298,15 @@
 class VerslagAlgemeenOverleg(Document):
     filter_param = "Soort eq 'Verslag van een algemeen overleg'"
 
     @property
     def voortouwcommissie_namen(self):
         names = []
         for zaak in self.zaken:
-            for zaak_actor in zaak.zaak_actors:
+            for zaak_actor in zaak.actors:
                 if zaak_actor.is_voortouwcommissie:
                     names.append(zaak_actor.naam)
         return names
 
     @property
     def document_url(self):
         if not self.dossiers:
```

### Comparing `tkapi-0.9.6/tkapi/order.py` & `tkapi-0.9.7/tkapi/order.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.6/tkapi/core.py` & `tkapi-0.9.7/tkapi/core.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.6/tkapi/kamervraag.py` & `tkapi-0.9.7/tkapi/kamervraag.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.6/tkapi/verslag.py` & `tkapi-0.9.7/tkapi/verslag.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     expand_params = ['Vergadering']
 
     @staticmethod
     def create_filter():
         return VerslagFilter()
 
     @property
-    def vergadering(self):
+    def vergadering(self) -> "Vergadering":
         from tkapi.vergadering import Vergadering
         return self.related_item(Vergadering)
 
     @property
     def soort(self) -> VerslagSoort:
         return self.get_property_enum_or_none('Soort', VerslagSoort)
```

### Comparing `tkapi-0.9.6/tkapi/zaak.py` & `tkapi-0.9.7/tkapi/zaak.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     INITIATIEF_NOTA = 'Initiatiefnota'
     INITIATIEF_WETGEVING = 'Initiatiefwetgeving'
     LIJST_EU_VOORSTELLEN = 'Lijst met EU-voorstellen'
     MONDELINGE_VRAGEN = 'Mondelinge vragen'
     MOTIE = 'Motie'
     NATIONALE_OMBUDSMAN = 'Nationale ombudsman'
     NETWERKVERKENNING = 'Netwerkverkenning'
-    NOTA_VAN_VERSLAG = 'Nota naar aanleiding van het (nader) verslag'
+    NOTA_VAN_VERSLAG = 'Nota n.a.v. het (nader/tweede nader/enz.) verslag'
     NOTA_VAN_WIJZIGING = 'Nota van wijziging'
     OVERIG = 'Overig'
     PARLEMENTAIR_ONDERZOEKSRAPPORT = 'Parlementair onderzoeksrapport'
     PKB_STRUCTUURVISIE = 'PKB/Structuurvisie'
     POSITION_PAPER = 'Position paper'
     RAPPORT_ALGEMENE_REKENKAMER = 'Rapport/brief Algemene Rekenkamer'
     RONDVRAAGPUNT_PROCEDUREVERGADERING = 'Rondvraagpunt procedurevergadering'
@@ -104,15 +104,15 @@
         self.add_filter_str(filter_str)
 
     def filter_volgnummer(self, volgnummer):
         filter_str = "Volgnummer eq {}".format(volgnummer)
         self._filters.append(filter_str)
 
     def filter_onderwerp(self, onderwerp):
-        filter_str = "Onderwerp eq '{}'".format(onderwerp)
+        filter_str = "Onderwerp eq '{}'".format(self.escape(onderwerp))
         self._filters.append(filter_str)
 
     def filter_has_besluit(self):
         filter_str = 'Besluit/any(b:b ne null)'
         self._filters.append(filter_str)
 
     def filter_has_activiteit(self):
@@ -154,15 +154,15 @@
         return self.related_items(Activiteit)
 
     @property
     def besluiten(self) -> List[Besluit]:
         return self.related_items(Besluit)
 
     @property
-    def zaak_actors(self):
+    def actors(self):
         return self.related_items(ZaakActor)
 
     @property
     def dossier(self) -> Dossier:
         return self.related_item(Dossier)
 
     @property
@@ -202,14 +202,23 @@
         return self.get_property_enum_or_none('Kabinetsappreciatie', KabinetsAppreciatie)
 
     @staticmethod
     def begin_date_key():
         return 'GestartOp'
 
 
+class ZaakActorRelatieSoort(Enum):
+    GERICHT_AAN = 'Gericht aan'
+    INDIENER = 'Indiener'
+    MEDEINDIENER = 'Medeindiener'
+    RAPPORTEUR = 'Rapporteur'
+    VOLGCOMMISSIE = 'Volgcommissie'
+    VOORTOUWCOMMISSIE = 'Voortouwcommissie'
+
+
 class ZaakActor(TKItem):
     type = 'ZaakActor'
 
     @staticmethod
     def create_filter():
         return Filter()
 
@@ -223,15 +232,15 @@
 
     @property
     def functie(self):
         return self.get_property_or_empty_string('Functie')
 
     @property
     def relatie(self):
-        return self.get_property_or_empty_string('Relatie')
+        return self.get_property_enum_or_none('Relatie', ZaakActorRelatieSoort)
 
     @property
     def persoon(self) -> Persoon:
         return self.related_item(Persoon)
 
     @property
     def zaak(self) -> Zaak:
@@ -243,15 +252,15 @@
 
     @property
     def commissie(self) -> Commissie:
         return self.related_item(Commissie)
 
     @property
     def is_voortouwcommissie(self):
-        return self.relatie == 'Voortouwcommissie'
+        return self.relatie == ZaakActorRelatieSoort.VOORTOUWCOMMISSIE
 
 
 class ZaakMetBesluitBase(Zaak):
 
     @property
     def besluit(self):
         besluiten = self.besluiten
```

### Comparing `tkapi-0.9.6/tkapi/activiteit.py` & `tkapi-0.9.7/tkapi/activiteit.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 class ActiviteitSoort(Enum):
     AANBIEDING = 'Aanbieding'
     AFSCHEID = 'Afscheid'
     ALGEMEEN_OVERLEG = 'Algemeen overleg'
     BEEDIGING = 'Beëdiging'
     BEGROTINGSOVERLEG = 'Begrotingsoverleg'
     BIJZONDERE_PROCEDURE = 'Bijzondere procedure'
+    COMMISSIEDEBAT = 'Commissiedebat'
     CONSTITUERENDE_VERGADERING = 'Constituerende vergadering'
     DELEGATIEVERGADERING = 'Delegatievergadering'
     EMAILPROCEDURE = 'E-mailprocedure'
     GESPREK = 'Gesprek'
     HAMERSTUKKEN = 'Hamerstukken'
     HERDENKING = 'Herdenking'
     HOORZITTING = 'Hoorzitting'
@@ -33,14 +34,17 @@
     MEDEDELINGEN = 'Mededelingen'
     NOTAOVERLEG = 'Notaoverleg'
     ONTBIJTBIJEENKOMST_PARLEMENT_WETENSCHAP = 'Ontbijtbijeenkomst Parlement en Wetenschap'
     OPENING = 'Opening'
     OVERIG = 'Overig'
     PETITIE = 'Petitie'
     PLENAIR_DEBAT = 'Plenair debat'
+    PLENAIR_DEBAT_2MIN = 'Plenair debat (tweeminutendebat)'
+    PLENAIR_DEBAT_INITIATIEF_WETGEVING = 'Plenair debat (initiatiefwetgeving)'
+    PLENAIR_DEBAT_WETGEVING = 'Plenair debat (wetgeving)'
     PROCEDUREVERGADERING = 'Procedurevergadering'
     REGELING_VAN_WERKZAAMHEDEN = 'Regeling van werkzaamheden'
     RONDETAFELGESPREK = 'Rondetafelgesprek'
     SCHRIFTELIJK_COMMENTAAR_ALGEMEEN = 'Schriftelijk commentaar algemeen'
     SCHRIFTELIJK_COMMENTAAR_GERICHT = 'Schriftelijk commentaar gericht'
     SLUITING = 'Sluiting'
     STEMMINGEN = 'Stemmingen'
@@ -213,15 +217,15 @@
         return self.reservering.activiteit
 
     @property
     def naam(self):
         return self.get_property_or_empty_string('Naam')
 
 
-class RelatieSoort(Enum):
+class ActiviteitRelatieSoort(Enum):
     AFGEMELD = 'Afgemeld'
     BEWINDSPERSOON = 'Bewindspersoon c.a.'
     DEELNEMER = 'Deelnemer'
     INITIATIEFNEMER = 'Initiatiefnemer'
     INTERPELLANT = 'Interpellant'
     VOLGCOMMISSIE = 'Volgcommissie'
 
@@ -266,9 +270,9 @@
         return self.get_property_or_empty_string('Spreektijd')
 
     @property
     def volgorde(self):
         return self.get_property_or_none('Volgorde')
 
     @property
-    def relatie(self) -> RelatieSoort:
-        return self.get_property_enum_or_none('Relatie', RelatieSoort)
+    def relatie(self) -> ActiviteitRelatieSoort:
+        return self.get_property_enum_or_none('Relatie', ActiviteitRelatieSoort)
```

### Comparing `tkapi-0.9.6/tkapi/commissie.py` & `tkapi-0.9.7/tkapi/commissie.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     VERVANGER_AMBTELIJK_LID = 'Vervanger (ambtelijk lid)'
     EERSTE_ONDERVOORZITTER_TK = 'Eerste ondervoorzitter Tweede Kamer'
 
 
 class CommissieFilter(SoortFilter):
 
     def filter_naam(self, naam):
-        filter_str = "NaamNL eq " + "'" + naam.replace("'", "''") + "'"
+        filter_str = "NaamNL eq '{}'".format(self.escape(naam))
         self._filters.append(filter_str)
 
 
 class CommissieZetelFilter(Filter):
 
     def filter_commissie(self, commissie):
         filter_str = "Commissie_Id eq {}".format(commissie.id)
```

### Comparing `tkapi-0.9.6/tkapi/stemming.py` & `tkapi-0.9.7/tkapi/stemming.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.6/tkapi/filter.py` & `tkapi-0.9.7/tkapi/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,26 @@
         if self._filters_or:
             if filter_str:
                 filter_str += ' and '
             sep = ' or '
             filter_str += sep.join(self._filters_or)
         return filter_str
 
+    @staticmethod
+    def escape(value: str) -> str:
+        return value.replace("'", "''")
+
 
 class PropertyFilter(Filter):
 
     def filter_property(self, property_name, value, is_or=False):
         if isinstance(value, Enum):
             value = value.value
-        filter_str = "{} eq '{}'".format(property_name, value.replace("'", "''"))
+        value = self.escape(value)
+        filter_str = "{} eq '{}'".format(property_name, value)
         self.add_filter_str(filter_str, is_or)
 
 
 class SoortFilter(PropertyFilter):
 
     def filter_soort(self, soort, is_or=False):
         self.filter_property(property_name='Soort', value=soort, is_or=is_or)
```

### Comparing `tkapi-0.9.6/tkapi/besluit.py` & `tkapi-0.9.7/tkapi/besluit.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.6/tkapi/util/document.py` & `tkapi-0.9.7/tkapi/util/document.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.6/tkapi/util/util.py` & `tkapi-0.9.7/tkapi/util/util.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.6/tkapi/util/queries.py` & `tkapi-0.9.7/tkapi/util/queries.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.6/tkapi/vergadering.py` & `tkapi-0.9.7/tkapi/vergadering.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,18 +12,24 @@
 
 
 class VergaderingFilter(SoortFilter):
 
     def __init__(self):
         super().__init__()
 
-    def filter_date_range(self, begin_datetime, end_datetime):
+    def filter_date_range(self, begin_datetime, end_datetime=None):
         filter_str = "Begin ge {}".format(util.datetime_to_odata(begin_datetime))
         self._filters.append(filter_str)
-        filter_str = "Einde lt {}".format(util.datetime_to_odata(end_datetime))
+
+        if end_datetime:
+            filter_str = "Einde lt {}".format(util.datetime_to_odata(end_datetime))
+            self._filters.append(filter_str)
+
+    def filter_changed_since(self, since_datetime):
+        filter_str = "ApiGewijzigdOp ge {}".format(util.datetime_to_odata(since_datetime))
         self._filters.append(filter_str)
 
 
 class Vergadering(TKItem):
     type = 'Vergadering'
     expand_params = ['Verslag']
```

### Comparing `tkapi-0.9.6/tkapi/tkapi.py` & `tkapi-0.9.7/tkapi/tkapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,22 +160,21 @@
             timeout=60
         )
         if cls._verbose:
             print('url ({} ms): {}'.format(
                 int(response.elapsed.total_seconds() * 1000),
                 urllib.parse.unquote(response.url))
             )
-        if response.status_code in [204, 404, 500]:
-            logger.warning('HTTP STATUS CODE: {}'.format(response.status_code))
-            logger.warning('WARNING: requested item does not exist: {}'.format(url))
+        if response.status_code in [204, 404]:
+            logger.info('HTTP STATUS CODE: {}'.format(response.status_code))
+            logger.info('Requested item does not exist: {}'.format(url))
             return {}
         elif response.status_code != 200:
-            logger.warning('HTTP STATUS CODE: {}'.format(response.status_code))
-            logger.warning('ODATA ERROR: {}'.format(response.json()['error']['message']))
-        # assert response.status_code == 200
+            logger.error('HTTP STATUS CODE: {}'.format(response.status_code))
+            logger.error('ODATA ERROR: {}'.format(response.json()['error']['message']))
         return response.json()
 
     @classmethod
     def get_item(cls, tkitem, id: str):
         url = '{}({})'.format(tkitem.type, id)
         params = tkitem.get_param_expand()
         return tkitem(cls._request_json(url, params))
```

### Comparing `tkapi-0.9.6/tkapi/fractie.py` & `tkapi-0.9.7/tkapi/fractie.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,40 +111,42 @@
         self._filters.append("TotEnMet eq null")
         self._filters.append("Verwijderd eq false")
 
 
 class FractieFilter(Filter):
 
     def filter_fractie(self, naam):
-        self._filters.append("NaamNL eq '{}'".format(naam))
+        self._filters.append("NaamNL eq '{}'".format(self.escape(naam)))
 
     def filter_fractie_id(self, uid):
         self._filters.append("Id eq {}".format(uid))
 
     def filter_actief(self):
         self._filters.append("DatumInactief eq null")
         self._filters.append("DatumActief ne null")
 
 
 class FractieZetelPersoonFilter(LidFilter):
 
     def filter_fractie(self, naam):
+        naam = self.escape(naam)
         self._filters.append("FractieZetel/Fractie/NaamNL eq '{}'".format(naam))
 
     def filter_fractie_id(self, uid):
         self._filters.append("FractieZetel/Fractie/Id eq {}".format(uid))
 
     def filter_actief(self):
         self._filters.append("TotEnMet eq null")
         self._filters.append("Verwijderd eq false")
 
 
 class FractieZetelFilter(Filter):
 
     def filter_fractie(self, naam):
+        naam = self.escape(naam)
         self._filters.append("Fractie/NaamNL eq '{}'".format(naam))
 
     def filter_fractie_id(self, uid):
         self._filters.append("Fractie/Id eq {}".format(uid))
 
 
 class FractieZetel(TKItem):
```

### Comparing `tkapi-0.9.6/tkapi.egg-info/PKG-INFO` & `tkapi-0.9.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,89 @@
 Metadata-Version: 2.1
 Name: tkapi
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python bindings and ORM for the Tweede Kamer OData API
 Home-page: https://github.com/openkamer/tkapi
 Author: Open Kamer
 Author-email: info@openkamer.org
 License: MIT
-Description: # tkapi
-        [![PyPI version](https://badge.fury.io/py/tkapi.svg)](https://badge.fury.io/py/tkapi)  
-        Python ORM and bindings for the [Tweede Kamer](https://tweedekamer.nl) [Open Data Portaal](https://opendata.tweedekamer.nl) OData API.
-        
-        A pure Python interface for the Tweede Kamer API with type annotations for easy data model discovery.
-        
-        Requires Python 3.5+.
-        
-        Please create an issue if you have any problems, questions or suggestions.
-        
-        ## Installation
-        ```
-        pip install tkapi
-        ```
-        
-        ## Authentication
-        You need to whitelist your IP by registering at https://opendata.tweedekamer.nl.
-        
-        ## Data model
-        See [Open Kamer Data Model documentation](https://opendata.tweedekamer.nl/documentatie/informatiemodel-20) for the data model that is mapped to Python classes.
-        
-        ## Usage
-        A simple first example,
-        ```python
-        import tkapi
-        
-        api = tkapi.TKApi()
-        personen = api.get_personen(max_items=100)
-        for persoon in personen:
-            print(persoon.achternaam)
-        ```
-        
-        For more examples see the [examples](./examples) and [tests](./tests).
-        
-        ## Entities
-        
-        See Tweede Kamer [documentation](https://opendata.tweedekamer.nl/documentatie/informatiemodel-20) for details.
-        
-        | Algemeen                    | Persoon                       | Fractie                  | Commissie                       |
-        |-----------------------------|-------------------------------|--------------------------|---------------------------------|
-        | Activiteit                  | Persoon                       | Fractie                  | Commissie                       |
-        | ActiviteitActor             | PersoonContactinformatie      | FractieAanvullendGegeven | CommissieContactinformatie      |
-        | Agendapunt                  | PersoonFunctie                | FractieZetel             | CommissieZetel                  |
-        | Besluit                     | PersoonGeschenk               | FractieZetelPersoon      | CommissieZetelVastPersoon       |
-        | Document                    | PersoonLoopbaan               | FractieZetelVacature     | CommissieZetelVastVacature      |
-        | DocumentActor               | PersoonNevenfunctie           |                          | CommissieZetelVervangerPersoon  |
-        | DocumentVersie              | PersoonNevenfunctieInkomsten  |                          | CommissieZetelVervangerVacature |
-        | Kamerstukdossier            | PersoonOnderwijs              |                          |                                 |
-        | Reservering                 | PersoonReis                   |                          |                                 |
-        | Stemming                    |                               |                          |                                 |
-        | Vergadering                 |                               |                          |                                 |
-        | Verslag                     |                               |                          |                                 |
-        | Zaak                        |                               |                          |                                 |
-        | ZaakActor                   |                               |                          |                                 |
-        | Zaal                        |                               |                          |                                 |
-        
-        ## Development
-        
-        ### Tests
-        
-        Run all tests,
-        ```bash
-        python -m unittest discover
-        ```
-        
-        #### Coverage report
-        
-        Run all tests,
-        ```bash
-        coverage run -m unittest discover
-        ```
-        
-        Create coverage report,
-        ```bash
-        coverage html
-        ```
-        Then visit htmlcov/index.html in your browser.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# tkapi
+[![PyPI version](https://badge.fury.io/py/tkapi.svg)](https://badge.fury.io/py/tkapi)  
+Python ORM and bindings for the [Tweede Kamer](https://tweedekamer.nl) [Open Data Portaal](https://opendata.tweedekamer.nl) OData API.
+
+A pure Python interface for the Tweede Kamer API with type annotations for easy data model discovery.
+
+Requires Python 3.5+.
+
+Please create an issue if you have any problems, questions or suggestions.
+
+## Installation
+```
+pip install tkapi
+```
+
+## Data model
+See [Open Kamer Data Model documentation](https://opendata.tweedekamer.nl/documentatie/informatiemodel) for the data model that is mapped to Python classes.
+
+## Usage
+A simple first example,
+```python
+import tkapi
+
+api = tkapi.TKApi()
+personen = api.get_personen(max_items=100)
+for persoon in personen:
+    print(persoon.achternaam)
+```
+
+For more examples see the [examples](./examples) and [tests](./tests).
+
+## Entities
+
+See Tweede Kamer [documentation](https://opendata.tweedekamer.nl/documentatie/informatiemodel-20) for details.
+
+| Algemeen                    | Persoon                       | Fractie                  | Commissie                       |
+|-----------------------------|-------------------------------|--------------------------|---------------------------------|
+| Activiteit                  | Persoon                       | Fractie                  | Commissie                       |
+| ActiviteitActor             | PersoonContactinformatie      | FractieAanvullendGegeven | CommissieContactinformatie      |
+| Agendapunt                  | PersoonFunctie                | FractieZetel             | CommissieZetel                  |
+| Besluit                     | PersoonGeschenk               | FractieZetelPersoon      | CommissieZetelVastPersoon       |
+| Document                    | PersoonLoopbaan               | FractieZetelVacature     | CommissieZetelVastVacature      |
+| DocumentActor               | PersoonNevenfunctie           |                          | CommissieZetelVervangerPersoon  |
+| DocumentVersie              | PersoonNevenfunctieInkomsten  |                          | CommissieZetelVervangerVacature |
+| Kamerstukdossier            | PersoonOnderwijs              |                          |                                 |
+| Reservering                 | PersoonReis                   |                          |                                 |
+| Stemming                    |                               |                          |                                 |
+| Vergadering                 |                               |                          |                                 |
+| Verslag                     |                               |                          |                                 |
+| Zaak                        |                               |                          |                                 |
+| ZaakActor                   |                               |                          |                                 |
+| Zaal                        |                               |                          |                                 |
+
+## Development
+
+### Tests
+
+Run all tests,
+```bash
+python -m unittest discover
+```
+
+#### Coverage report
+
+Run all tests,
+```bash
+coverage run -m unittest discover
+```
+
+Create coverage report,
+```bash
+coverage html
+```
+Then visit htmlcov/index.html in your browser.
```

### Comparing `tkapi-0.9.6/PKG-INFO` & `tkapi-0.9.7/tkapi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,89 @@
 Metadata-Version: 2.1
 Name: tkapi
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python bindings and ORM for the Tweede Kamer OData API
 Home-page: https://github.com/openkamer/tkapi
 Author: Open Kamer
 Author-email: info@openkamer.org
 License: MIT
-Description: # tkapi
-        [![PyPI version](https://badge.fury.io/py/tkapi.svg)](https://badge.fury.io/py/tkapi)  
-        Python ORM and bindings for the [Tweede Kamer](https://tweedekamer.nl) [Open Data Portaal](https://opendata.tweedekamer.nl) OData API.
-        
-        A pure Python interface for the Tweede Kamer API with type annotations for easy data model discovery.
-        
-        Requires Python 3.5+.
-        
-        Please create an issue if you have any problems, questions or suggestions.
-        
-        ## Installation
-        ```
-        pip install tkapi
-        ```
-        
-        ## Authentication
-        You need to whitelist your IP by registering at https://opendata.tweedekamer.nl.
-        
-        ## Data model
-        See [Open Kamer Data Model documentation](https://opendata.tweedekamer.nl/documentatie/informatiemodel-20) for the data model that is mapped to Python classes.
-        
-        ## Usage
-        A simple first example,
-        ```python
-        import tkapi
-        
-        api = tkapi.TKApi()
-        personen = api.get_personen(max_items=100)
-        for persoon in personen:
-            print(persoon.achternaam)
-        ```
-        
-        For more examples see the [examples](./examples) and [tests](./tests).
-        
-        ## Entities
-        
-        See Tweede Kamer [documentation](https://opendata.tweedekamer.nl/documentatie/informatiemodel-20) for details.
-        
-        | Algemeen                    | Persoon                       | Fractie                  | Commissie                       |
-        |-----------------------------|-------------------------------|--------------------------|---------------------------------|
-        | Activiteit                  | Persoon                       | Fractie                  | Commissie                       |
-        | ActiviteitActor             | PersoonContactinformatie      | FractieAanvullendGegeven | CommissieContactinformatie      |
-        | Agendapunt                  | PersoonFunctie                | FractieZetel             | CommissieZetel                  |
-        | Besluit                     | PersoonGeschenk               | FractieZetelPersoon      | CommissieZetelVastPersoon       |
-        | Document                    | PersoonLoopbaan               | FractieZetelVacature     | CommissieZetelVastVacature      |
-        | DocumentActor               | PersoonNevenfunctie           |                          | CommissieZetelVervangerPersoon  |
-        | DocumentVersie              | PersoonNevenfunctieInkomsten  |                          | CommissieZetelVervangerVacature |
-        | Kamerstukdossier            | PersoonOnderwijs              |                          |                                 |
-        | Reservering                 | PersoonReis                   |                          |                                 |
-        | Stemming                    |                               |                          |                                 |
-        | Vergadering                 |                               |                          |                                 |
-        | Verslag                     |                               |                          |                                 |
-        | Zaak                        |                               |                          |                                 |
-        | ZaakActor                   |                               |                          |                                 |
-        | Zaal                        |                               |                          |                                 |
-        
-        ## Development
-        
-        ### Tests
-        
-        Run all tests,
-        ```bash
-        python -m unittest discover
-        ```
-        
-        #### Coverage report
-        
-        Run all tests,
-        ```bash
-        coverage run -m unittest discover
-        ```
-        
-        Create coverage report,
-        ```bash
-        coverage html
-        ```
-        Then visit htmlcov/index.html in your browser.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# tkapi
+[![PyPI version](https://badge.fury.io/py/tkapi.svg)](https://badge.fury.io/py/tkapi)  
+Python ORM and bindings for the [Tweede Kamer](https://tweedekamer.nl) [Open Data Portaal](https://opendata.tweedekamer.nl) OData API.
+
+A pure Python interface for the Tweede Kamer API with type annotations for easy data model discovery.
+
+Requires Python 3.5+.
+
+Please create an issue if you have any problems, questions or suggestions.
+
+## Installation
+```
+pip install tkapi
+```
+
+## Data model
+See [Open Kamer Data Model documentation](https://opendata.tweedekamer.nl/documentatie/informatiemodel) for the data model that is mapped to Python classes.
+
+## Usage
+A simple first example,
+```python
+import tkapi
+
+api = tkapi.TKApi()
+personen = api.get_personen(max_items=100)
+for persoon in personen:
+    print(persoon.achternaam)
+```
+
+For more examples see the [examples](./examples) and [tests](./tests).
+
+## Entities
+
+See Tweede Kamer [documentation](https://opendata.tweedekamer.nl/documentatie/informatiemodel-20) for details.
+
+| Algemeen                    | Persoon                       | Fractie                  | Commissie                       |
+|-----------------------------|-------------------------------|--------------------------|---------------------------------|
+| Activiteit                  | Persoon                       | Fractie                  | Commissie                       |
+| ActiviteitActor             | PersoonContactinformatie      | FractieAanvullendGegeven | CommissieContactinformatie      |
+| Agendapunt                  | PersoonFunctie                | FractieZetel             | CommissieZetel                  |
+| Besluit                     | PersoonGeschenk               | FractieZetelPersoon      | CommissieZetelVastPersoon       |
+| Document                    | PersoonLoopbaan               | FractieZetelVacature     | CommissieZetelVastVacature      |
+| DocumentActor               | PersoonNevenfunctie           |                          | CommissieZetelVervangerPersoon  |
+| DocumentVersie              | PersoonNevenfunctieInkomsten  |                          | CommissieZetelVervangerVacature |
+| Kamerstukdossier            | PersoonOnderwijs              |                          |                                 |
+| Reservering                 | PersoonReis                   |                          |                                 |
+| Stemming                    |                               |                          |                                 |
+| Vergadering                 |                               |                          |                                 |
+| Verslag                     |                               |                          |                                 |
+| Zaak                        |                               |                          |                                 |
+| ZaakActor                   |                               |                          |                                 |
+| Zaal                        |                               |                          |                                 |
+
+## Development
+
+### Tests
+
+Run all tests,
+```bash
+python -m unittest discover
+```
+
+#### Coverage report
+
+Run all tests,
+```bash
+coverage run -m unittest discover
+```
+
+Create coverage report,
+```bash
+coverage html
+```
+Then visit htmlcov/index.html in your browser.
```

### Comparing `tkapi-0.9.6/setup.py` & `tkapi-0.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name='tkapi',
     description='Python bindings and ORM for the Tweede Kamer OData API',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version='0.9.6',
+    version='0.9.7',
     url='https://github.com/openkamer/tkapi',
     author='Open Kamer',
     author_email='info@openkamer.org',
     license='MIT',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

### Comparing `tkapi-0.9.6/README.md` & `tkapi-0.9.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,19 +9,16 @@
 Please create an issue if you have any problems, questions or suggestions.
 
 ## Installation
 ```
 pip install tkapi
 ```
 
-## Authentication
-You need to whitelist your IP by registering at https://opendata.tweedekamer.nl.
-
 ## Data model
-See [Open Kamer Data Model documentation](https://opendata.tweedekamer.nl/documentatie/informatiemodel-20) for the data model that is mapped to Python classes.
+See [Open Kamer Data Model documentation](https://opendata.tweedekamer.nl/documentatie/informatiemodel) for the data model that is mapped to Python classes.
 
 ## Usage
 A simple first example,
 ```python
 import tkapi
 
 api = tkapi.TKApi()
```

