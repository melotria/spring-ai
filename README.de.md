# Spring AI [![build status](https://github.com/spring-projects/spring-ai/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/spring-projects/spring-ai/actions/workflows/continuous-integration.yml) [![build status](https://github.com/spring-projects/spring-ai-integration-tests/actions/workflows/spring-ai-integration-tests.yml/badge.svg)](https://github.com/spring-projects/spring-ai-integration-tests/actions/workflows/spring-ai-integration-tests.yml)


Das Spring AI Projekt bietet eine Spring-freundliche API und Abstraktionen für die Entwicklung von KI-Anwendungen.

Sein Ziel ist es, die Designprinzipien des Spring-Ökosystems wie Portabilität und modulares Design auf den KI-Bereich anzuwenden und die Verwendung von POJOs als Bausteine einer Anwendung im KI-Bereich zu fördern.

![spring-ai-integration-diagram-3](https://docs.spring.io/spring-ai/reference/_images/spring-ai-integration-diagram-3.svg)

> Im Kern adressiert Spring AI die grundlegende Herausforderung der KI-Integration: Die Verbindung Ihrer Unternehmens-__Daten__ und __APIs__ mit den __KI-Modellen__.

Das Projekt lässt sich von bekannten Python-Projekten wie [LangChain](https://docs.langchain.com/docs/) und [LlamaIndex](https://gpt-index.readthedocs.io/en/latest/getting_started/concepts.html) inspirieren, aber Spring AI ist keine direkte Portierung dieser Projekte. Das Projekt wurde mit der Überzeugung gegründet, dass die nächste Welle von Generative-KI-Anwendungen nicht nur für Python-Entwickler sein wird, sondern in vielen Programmiersprachen allgegenwärtig sein wird.

Sie können den Blogbeitrag [Why Spring AI](https://spring.io/blog/2024/11/19/why-spring-ai) für weitere Motivationen lesen.

Dies ist ein Überblick über die wichtigsten Funktionen.
Weitere Details finden Sie in der [Referenzdokumentation](https://docs.spring.io/spring-ai/reference/)

* Unterstützung für alle wichtigen [KI-Modellanbieter](https://docs.spring.io/spring-ai/reference/api/index.html) wie Anthropic, OpenAI, Microsoft, Amazon, Google und Ollama. Unterstützte Modelltypen umfassen:
  - [Chat Completion](https://docs.spring.io/spring-ai/reference/api/chatmodel.html)
  - [Embedding](https://docs.spring.io/spring-ai/reference/api/embeddings.html)
  - [Text zu Bild](https://docs.spring.io/spring-ai/reference/api/imageclient.html)
  - [Audio-Transkription](https://docs.spring.io/spring-ai/reference/api/audio/transcriptions.html)
  - [Text zu Sprache](https://docs.spring.io/spring-ai/reference/api/audio/speech.html)
  - [Moderation](https://docs.spring.io/spring-ai/reference/api/index.html#api/moderation)
* Portable API-Unterstützung über KI-Anbieter hinweg für synchrone und Streaming-Optionen. Zugriff auf [modellspezifische Funktionen](https://docs.spring.io/spring-ai/reference/api/chatmodel.html#_chat_options) ist ebenfalls verfügbar.
* [Strukturierte Ausgaben](https://docs.spring.io/spring-ai/reference/api/structured-output-converter.html) - Mapping von KI-Modellausgaben zu POJOs.
* Unterstützung für alle wichtigen [Vektordatenbankanbieter](https://docs.spring.io/spring-ai/reference/api/vectordbs.html) wie *Apache Cassandra, Azure Vector Search, Chroma, Milvus, MongoDB Atlas, MariaDB, Neo4j, Oracle, PostgreSQL/PGVector, PineCone, Qdrant, Redis und Weaviate*.
* Portable API über Vektorspeicheranbieter hinweg, einschließlich einer neuartigen SQL-ähnlichen [Metadaten-Filter-API](https://docs.spring.io/spring-ai/reference/api/vectordbs.html#metadata-filters).
* [Tools/Funktionsaufrufe](https://docs.spring.io/spring-ai/reference/api/functions.html) - ermöglicht dem Modell, die Ausführung clientseitiger Tools und Funktionen anzufordern und so bei Bedarf auf notwendige Echtzeit-Informationen zuzugreifen.
* [Beobachtbarkeit](https://docs.spring.io/spring-ai/reference/observability/index.html) - Bietet Einblicke in KI-bezogene Operationen.
* Dokumenteninjektions-[ETL-Framework](https://docs.spring.io/spring-ai/reference/api/etl-pipeline.html) für Data Engineering.
* [KI-Modellbewertung](https://docs.spring.io/spring-ai/reference/api/testing.html) - Hilfsmittel zur Bewertung generierter Inhalte und zum Schutz vor halluzinierten Antworten.
* [ChatClient API](https://docs.spring.io/spring-ai/reference/api/chatclient.html) - Fluent API für die Kommunikation mit KI-Chat-Modellen, idiomatisch ähnlich zu den WebClient- und RestClient-APIs.
* [Advisors API](https://docs.spring.io/spring-ai/reference/api/advisors.html) - Kapselt wiederkehrende Generative-KI-Muster, transformiert Daten, die an Sprachmodelle (LLMs) gesendet und von diesen empfangen werden, und bietet Portabilität über verschiedene Modelle und Anwendungsfälle hinweg.
* Unterstützung für [Chat-Konversationsgedächtnis](https://docs.spring.io/spring-ai/reference/api/chatclient.html#_chat_memory) und [Retrieval Augmented Generation (RAG)](https://docs.spring.io/spring-ai/reference/api/chatclient.html#_retrieval_augmented_generation).
* Spring Boot Auto-Konfiguration und Starter für alle KI-Modelle und Vektorspeicher - verwenden Sie [start.spring.io](https://start.spring.io/), um das Modell oder den Vektorspeicher Ihrer Wahl auszuwählen.

## Erste Schritte

Bitte beziehen Sie sich auf die [Erste-Schritte-Anleitung](https://docs.spring.io/spring-ai/reference/getting-started.html) für Anweisungen zum Hinzufügen Ihrer Abhängigkeiten.

## Projektressourcen

* [Dokumentation](https://docs.spring.io/spring-ai/reference/)
* [Issues](https://github.com/spring-projects/spring-ai/issues)
<!-- * [Diskussionen](https://github.com/spring-projects/spring-ai/discussions) - Gehen Sie hierhin, wenn Sie eine Frage, einen Vorschlag oder Feedback haben! -->
* [Awesome Spring AI](https://github.com/danvega/awesome-spring-ai) - Eine kuratierte Liste von großartigen Ressourcen, Tools, Tutorials und Projekten zum Erstellen von generativen KI-Anwendungen mit Spring AI
* [Spring AI Beispiele](https://github.com/spring-projects/spring-ai-examples) enthält Beispielprojekte, die bestimmte Funktionen detaillierter erklären.

## Breaking Changes

* Lesen Sie die [Upgrade-Hinweise](https://docs.spring.io/spring-ai/reference/upgrade-notes.html), um zu erfahren, wie Sie auf 1.0.0.M1 oder höher upgraden können.

## Klonen des Repositories

Dieses Repository enthält [große Modelldateien](https://github.com/spring-projects/spring-ai/tree/main/models/spring-ai-transformers/src/main/resources/onnx/all-MiniLM-L6-v2).
Um es zu klonen, müssen Sie entweder:

- Die großen Dateien ignorieren (beeinflusst das Spring-AI-Verhalten nicht): `GIT_LFS_SKIP_SMUDGE=1 git clone git@github.com:spring-projects/spring-ai.git`.
- Oder [Git Large File Storage](https://git-lfs.com/) installieren, bevor Sie das Repository klonen.


## Bauen

Um mit Unit-Tests zu bauen:

```shell
./mvnw clean package
```

Um einschließlich Integrationstests zu bauen:

```shell
./mvnw clean verify -Pintegration-tests
```

Beachten Sie, dass Sie API-Schlüssel-Umgebungsvariablen für OpenAI oder andere Modellanbieter setzen sollten, bevor Sie ausführen. Wenn der API-Schlüssel für einen bestimmten Modellanbieter nicht gesetzt ist, wird der Integrationstest übersprungen.

Um einen bestimmten Integrationstest auszuführen, der bis zu zwei Versuche zulässt, um erfolgreich zu sein. Dies ist nützlich, wenn ein gehosteter Dienst nicht zuverlässig ist oder eine Zeitüberschreitung auftritt.
```shell
./mvnw -pl vector-stores/spring-ai-pgvector-store -Pintegration-tests -Dfailsafe.rerunFailingTestsCount=2 -Dit.test=PgVectorStoreIT verify
```

### Integrationstests
Es gibt viele Integrationstests, daher ist es oft nicht realistisch, sie alle auf einmal auszuführen.

Ein schneller Durchlauf durch die wichtigsten Pfade, der Integrationstests für

* OpenAI-Modelle
* OpenAI-Autokonfiguration
* PGVector
* Chroma

ausführt, kann mit dem Profil `-Pci-fast-integration-tests` durchgeführt werden und wird im Haupt-CI-Build dieses Projekts verwendet.

Ein vollständiger Integrationstest wird zweimal täglich im [Spring AI Integration Test Repository](https://github.com/spring-projects/spring-ai-integration-tests) durchgeführt.

Eine Möglichkeit, Integrationstests für einen Teil des Codes auszuführen, besteht darin, zunächst eine schnelle Kompilierung und Installation des Projekts durchzuführen:

```shell
./mvnw clean install -DskipTests -Dmaven.javadoc.skip=true
```
Dann führen Sie den Integrationstest für ein bestimmtes Modul mit der Option `-pl` aus:
```shell
./mvnw verify -Pintegration-tests -pl spring-ai-spring-boot-testcontainers
```

### Dokumentation

Um die Dokumentation zu erstellen:
```shell
./mvnw -pl spring-ai-docs antora
```

Die Dokumentation befindet sich dann im Verzeichnis `spring-ai-docs/target/antora/site/index.html`

Um mit dem [java-format plugin](https://github.com/spring-io/spring-javaformat) zu formatieren:
```shell
./mvnw spring-javaformat:apply
```

Um das Jahr in den Lizenzheadern mit dem [license-maven-plugin](https://oss.carbou.me/license-maven-plugin/#goals) zu aktualisieren:
```shell
./mvnw license:update-file-header -Plicense
```

Um Javadocs mit [javadoc:javadoc](https://maven.apache.org/plugins/maven-javadoc-plugin/) zu überprüfen:
```shell
./mvnw javadoc:javadoc -Pjavadoc
```

Um mit aktivierten Checkstyles zu bauen.
Checkstyles sind derzeit deaktiviert, aber Sie können sie aktivieren, indem Sie Folgendes tun:
```shell
./mvnw clean package -DskipTests -Ddisable.checks=false
```