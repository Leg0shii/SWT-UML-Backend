# Backend - E-Learning-System

## Übersicht

Das Backend unseres E-Learning-Systems ist die zentrale Datenverarbeitungs- und Kommunikationskomponente. Es verwaltet die Datenbanken, Server-Logik und die Kommunikation zwischen Clients und dem Server. Entwickelt in Java, sorgt das Backend für eine zuverlässige und effiziente Datenverwaltung und Synchronisation.

## Funktionen

- **Benutzerverwaltung:** Verwaltung von Benutzerkonten, Rollen und Berechtigungen.
- **Klassenzimmer-Management:** Erstellung, Bearbeitung und Verwaltung von Klassenzimmern.
- **Aufgabenverwaltung:** Erstellung, Zuweisung und Verwaltung von Aufgaben und Lösungen.
- **Chat-Funktion:** Echtzeit-Kommunikation innerhalb von Sessions und Gruppen.
- **Datenbankintegration:** Persistente Speicherung aller relevanten Daten in einer MySQL-Datenbank.
- **Client-Server-Kommunikation:** Effiziente Synchronisation und Datenübertragung mittels RMI (Remote Method Invocation).

## Architektur

Das Backend ist modular aufgebaut, mit klar getrennten Komponenten für verschiedene Funktionalitäten:

- **Command Queues**: Verwaltung von Befehlsobjekten zur effizienten Verarbeitung von Client-Anfragen.
- **Manager-Klassen**: Verwaltung von Usern, Gruppen, Sessions und Klassen durch spezialisierte Manager.
- **RMI-Integration**: Ermöglicht Remote Method Invocation für die Kommunikation zwischen Client und Server.
- **Datenbankmanager**: Zuständig für die Interaktion mit der MySQL-Datenbank, einschließlich CRUD-Operationen und Daten-Caching.

## Geplante Verbesserungen

- **Fehlerbehebung**: Untersuchung und Behebung der Datenbankintegritätsprobleme und Memory Leaks.
- **Optimierung der Synchronisation**: Verbesserung der Synchronisationsmechanismen, um die CPU-Last zu reduzieren.
- **Erweiterung der Funktionalitäten**: Implementierung fehlender Features wie Admin-Übersicht und textuelle Use Case Spezifikation.

## Datenbankstruktur

Unsere MySQL-Datenbank ist in der dritten Normalform gestaltet und umfasst die folgenden Tabellen:

- User: Speicherung von Benutzerinformationen und Rollen.
- Groups: Verwaltung von Benutzergruppen innerhalb von Sessions.
- Courses: Repräsentation von Klassenzimmern und deren Teilnehmern.
- Sessions: Temporäre Repräsentationen von Klassenzimmern für aktuelle Sitzungen.
