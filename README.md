# comfyui_dagthomas

### 🌟 Advanced Prompt Generation and Image Analysis

Dieses Plugin erweitert ComfyUI mit fortschrittlichen Prompt-Generierungsmöglichkeiten und Bildanalysen durch die Nutzung von GPT-4 Vision. Es beinhaltet die folgenden Komponenten:

## 🧑‍🏫 Klassen

### 1. **PromptGenerator**

Ein vielseitiger Prompt-Generator für Text-zu-Bild-KI-Systeme.

**Features:**
- Generiert Prompts basierend auf verschiedenen anpassbaren Parametern
- Unterstützt verschiedene Kunstformen, Fotografiestile und digitale Kunst
- Ermöglicht zufällige Auswahl oder spezifische Entscheidungen für jeden Parameter
- Gibt separate Prompts für verschiedene Modellkomponenten aus (z. B. CLIP, T5)

📝 **Hinweis**:
- Das "subject"-Eingabefeld kann so geändert werden, dass es deinen Stil oder Lora unterstützt, indem du dein Thema hinzufügst.
- Das "custom"-Eingabefeld fügt einen Prompt am Anfang der Prompt-Zeichenkette hinzu.

![image](https://github.com/dagthomas/comfyui_dagthomas/assets/4311672/2c6e7418-51a6-465c-8573-36f36300e8a6)

### 2. **GPT4VisionNode**

Analysiert Bilder mithilfe des GPT-4 Vision-Modells von OpenAI.

**Features:**
- Nimmt Bild-Eingaben an und generiert detaillierte Beschreibungen
- Unterstützt benutzerdefinierte Basis-Prompts
- Bietet Optionen für "detaillierte Beschreibungen" oder einfache Ausgaben
- Komprimierungsoptionen zur Begrenzung der Ausgabelänge
- Fähigkeit, Poster zu erstellen

![gpt-4o vision](https://github.com/dagthomas/comfyui_dagthomas/blob/master/examples/flux/gpt-4o_vision/dagthomas_gpt-4o-vision-workflow.png)

[Workflow](https://github.com/dagthomas/comfyui_dagthomas/blob/master/examples/flux/gpt-4o_vision/dagthomas_gpt4o_vision_workflow.json)

### 3. **GPT4MiniNode**

Erzeugt Texte basierend auf Eingabetexten mithilfe des GPT-4-Modells.

**Features:**
- Nimmt Texteingaben an und generiert verbesserte Beschreibungen
- Unterstützt benutzerdefinierte Basis-Prompts
- Bietet Optionen für "detaillierte Beschreibungen" oder einfache Ausgaben
- Komprimierungsoptionen zur Begrenzung der Ausgabelänge

![gpt-4o-mini](https://github.com/dagthomas/comfyui_dagthomas/blob/master/examples/flux/gpt-4o-mini/dagthomas_gpt-4o-mini_workflow.png)

[Workflow](https://github.com/dagthomas/comfyui_dagthomas/blob/master/examples/flux/gpt-4o-mini/dagthomas_gpt-4o-mini_workflow.json)

### 4. **OllamaNode**

Generiert Texte mithilfe von benutzerdefinierten Ollama-Modellen basierend auf Eingabetexten.

**Features:**
- Nimmt Texteingaben an und generiert verbesserte Beschreibungen
- Unterstützt benutzerdefinierte Basis-Prompts
- Bietet Optionen für "detaillierte Beschreibungen" oder einfache Ausgaben
- Komprimierungsoptionen zur Begrenzung der Ausgabelänge

![Ollama](https://github.com/dagthomas/comfyui_dagthomas/blob/master/examples/flux/ollama_local_llm/comfyui_dagthomas_localllm__00044_.png)

[Workflow](https://github.com/dagthomas/comfyui_dagthomas/blob/master/examples/flux/ollama_local_llm/dagthomas_ollama_workflow.json)

### 5. **Pure Florence Workflow**

Du kannst auch einen rein lokalen Florence-Workflow verwenden, ohne andere Nodes.

![Florence2](https://github.com/dagthomas/comfyui_dagthomas/blob/master/examples/flux/florence2/dagthomas_florence2_workflow.png)

[Workflow](https://github.com/dagthomas/comfyui_dagthomas/blob/master/examples/flux/florence2/dagthomas_florence2_workflow.json)

### 6. **PGSD3LatentGenerator**

Generiert latente Repräsentationen für die Verwendung in Stable Diffusion 3-Pipelines.

**Features:**
- Erstellt latente Tensoren mit angegebenen Dimensionen
- Unterstützt Stapelverarbeitung
- Passt die Dimensionen automatisch an, um eine konsistente Megapixel-Zahl aufrechtzuerhalten

![image](https://github.com/user-attachments/assets/b4e0bb6e-fded-4a99-b8d4-558f21124863)

## 🚀 Verwendung

Diese Klassen können in ComfyUI-Workflows integriert werden, um die Prompt-Generierung, Bildanalyse und die Manipulation des latenten Raums für fortschrittliche KI-Bildgenerierungspipelines zu verbessern.

## 🔧 Anforderungen

- OpenAI API-Schlüssel (für GPT4VisionNode und GPT4MiniNode)
- ComfyUI-Umgebung
- Zusätzliche Abhängigkeiten gemäß den Import-Anweisungen

## 📝 Hinweise

- Stelle sicher, dass dein OpenAI API-Schlüssel in den Umgebungsvariablen gesetzt ist.
- Einige Klassen erfordern möglicherweise zusätzliche Datendateien (JSON), um vollständig zu funktionieren.
- Weitere Details zur Verwendung und zu den Eingabetypen findest du in der Dokumentation der jeweiligen Klasse.

## 🖼️ Beispiele (Flux Dev - 03/08/2024)

![ComfyUI_00005_](https://github.com/user-attachments/assets/d760bb22-797e-441e-a5b5-52e793a2b7c8)
![ComfyUI_00007_](https://github.com/user-attachments/assets/6975521b-85e3-4e18-a061-8cefb95159e5)
![ComfyUI_00034_](https://github.com/user-attachments/assets/470426d5-9320-40a3-816e-9d4bcfda6940)

## 🖼️ Beispiele (SD3 Medium - 06/15/2024)

![image](https://github.com/dagthomas/comfyui_dagthomas/assets/4311672/94c76273-0a16-450a-876c-9eb515d995d5)
![image](https://github.com/dagthomas/comfyui_dagthomas/assets/4311672/37924320-6b46-48fb-9c5d-a24da2d3fd4c)

# 🔮 **Advanced Prompts**

## **APNext Workflow Beispiel**

[Workflow](https://github.com/dagthomas/comfyui_dagthomas/blob/master/examples/flux/apnext/APNext_Examples.json)

## **APNextNode Funktion**

Der `APNextNode` ist ein benutzerdefinierter Node, der Eingabeprompts verarbeitet und um zusätzliche kontextuelle Informationen erweitert. Er eignet sich besonders für die Erstellung kreativer Inhalte durch die Einbeziehung zufälliger Elemente aus vordefinierten Kategorien.

**Features:**
- Verarbeitet Eingabeprompts und fügt Kontexte aus verschiedenen Kategorien hinzu
- Unterstützt mehrere Eingabetypen, einschließlich erforderlicher und optionaler Parameter
- Lädt Kategoriedaten dynamisch aus JSON-Dateien
- Bietet Optionen für die zufällige Auswahl von Elementen innerhalb der Kategorien
- Ermöglicht das Hinzufügen von Attributen zu ausgewählten Elementen

## 📂 Kategorien

Die Funktion unterstützt mehrere Kategorien, die aus JSON-Dateien geladen werden:

1. Architektur
2. Kunst
3. Künstler
4. Marken
5. Charakter
6. Kinematografisch
7. Mode
8. Gefühle
9. Geografie
10. Mensch
11. Interaktion
12. Schlüsselwörter
13. Personen
14. Fotografie
15. Handlungen
16. Posen
17. Szene
18. Wissenschaft
19. Gegenstände
20. Zeit
21. Typografie
22. Fahrzeuge
23. Videospiel

## 📖 Verwendung

Der `APNextNode` ist so konzipiert, dass er in größere Systeme integriert wird. Er verarbeitet Eingabeprompts und optional Kategorieauswahlen, um einen verbesserten Prompt und eine zufällige Ausgabe zu generieren.

## 🚀 Dateistruktur

Die Funktion erwartet eine spezifische Dateistruktur für Kategoriedaten:

```
data/
└── next/
    └── [KATEGORIE]/
        └── [feld_name].json
```

Jede JSON-Datei sollte entweder ein Array von Elementen oder ein Wörterbuch mit Schlüsseln wie "items", "preprompt", "separator", "endprompt" und "attributes" enthalten.

## 🔧 Anpassung

Füge eigene Kategorien hinzu, indem du im Verzeichnis `data/next/` neue Ordner und JSON-Dateien erstellst.
