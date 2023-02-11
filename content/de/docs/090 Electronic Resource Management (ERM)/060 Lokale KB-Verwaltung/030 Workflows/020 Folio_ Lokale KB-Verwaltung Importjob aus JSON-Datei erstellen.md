---
title: "Folio: Lokale KB-Verwaltung Importjob aus JSON-Datei erstellen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-lokale_kb_verwaltung, by-folio, cat-workflows, for-anwender]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/erm/local-kb-admin/#creating-a-json-import-job ) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Lokale+KB-Verwaltung+Importjob+aus+JSON-Datei+erstellen)
    "
---

{{% pageinfo %}}
JSON-Schema original nur verlink. Zusätzlich auch direkt eingefügt.
{{% /pageinfo %}}

Um der lokalen KB Daten hinzuzufügen, können JSON-Importdateien nach einem [JSON-Schema](https://drive.google.com/file/d/1ask-NiQwjgB70JroycsY78vfTYemgusy/view) erstellt werden.

1.  In der **Lokalen KB-Verwaltung** auf **Aktionen > JSON-Importjob** klicken.
2.  Im Fenster **Neuer JSON-Job** die **JSON-Datei in den Upload-Bereich ziehen** oder auf die Schaltfläche "**oder Datei auswählen**" klicken, um die JSON-Datei im Dateisystem auszuwählen.
3.  Auf **Speichern & schließen** klicken. Der Auftrag ist gespeichert und wird im Hintergrund verarbeitet.

## JSON-Schema
<pre>
{
  "$schema": "http://json-schema.org/draft-07/schema#",
  "type": "object",
  "properties": {
    "header": {
      "type": "object",
      "properties": {
        "dataSchema": {
          "type": "object",
          "properties": {
            "name": {
              "type": "string"
            },
            "version": {
              "type": "number"
            }
          },
          "required": \[
            "name",
            "version"
          \]
        }
      },
      "required": \[
        "dataSchema"
      \]
    },
    "records": {
      "type": "array",
      "items": {
        "type": "object",
        "properties": {
          "source": {
            "type": "string"
          },
          "reference": {
            "type": "string"
          },
          "name": {
            "type": "string"
          },
          "trustedSourceTI": {
            "type": "boolean"
          },
          "packageProvider": {
            "type": "object",
            "properties": {
              "name": {
                "type": "string"
              },
              "reference": {
                "type": "string"
              }
            }
          },
          "description": {
            "type": "string"
          },
          "lifecycleStatus": {
            "type": "string"
          },
          "availabilityScope": {
            "type": "string"
          },
          "availabilityConstraints": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {
                "body": {
                  "type": "string"
                }
              }
            }
          },
          "packageDescriptionUrls": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {
                "url": {
                  "type": "string"
                }
              }
            }
          },
          "alternateResourceNames": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {
                "name": {
                  "type": "string"
                }
              }
            }
          },
          "contentTypes": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {
                "contentType": {
                  "type": "string"
                }
              }
            }
          },
          "sourceDataCreated": {
            "type": "string"
          },
          "sourceDataUpdated": {
            "type": "string"
          },
          "identifiers": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {
                "value": {
                  "type": "string"
                },
                "namespace": {
                  "type": "string"
                }
              }
            }
          },
          "contentItems": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {
                "note": {
                  "type": "string"
                },
                "depth": {
                  "type": "string"
                },
                "accessStart": {
                  "type": "string",
                  "format": "date"
                },
                "accessEnd": {
                  "type": "string",
                  "format": "date"
                },
                "coverage": {
                  "type": "array",
                  "items": {
                    "type": "object",
                    "properties": {
                      "startDate": {
                        "type": "string",
                        "format": "date"
                      },
                      "startVolume": {
                        "type": "string"
                      },
                      "startIssue": {
                        "type": "string"
                      },
                      "endDate": {
                        "type": "string",
                        "format": "date"
                      },
                      "endVolume": {
                        "type": "string"
                      },
                      "endIssue": {
                        "type": "string"
                      }
                    }
                  }
                },
                "embargo": {
                  "type": "string"
                },
                "platformTitleInstance": {
                  "type": "object",
                  "properties": {
                    "platform": {
                      "type": "string"
                    },
                    "platformUrl": {
                      "type": "string",
                      "format": "uri"
                    },
                    "url": {
                      "type": "string",
                      "format": "uri"
                    },
                    "titleInstance": {
                      "type": "object",
                      "properties": {
                        "name": {
                          "type": "string"
                        },
                        "monographEdition": {
                          "type": "string"
                        },
                        "monographVolume": {
                          "type": "string"
                        },
                        "firstAuthor": {
                          "type": "string"
                        },
                        "firstEditor": {
                          "type": "string"
                        },
                        "dateMonographPublished": {
                          "type": "string",
                          "pattern": "^\\\\d\\\\d\\\\d\\\\d(-\\\\d\\\\d(-\\\\d\\\\d)?)?$"
                        },
                        "identifiers": {
                          "type": "array",
                          "items": {
                            "type": "object",
                            "properties": {
                              "value": {
                                "type": "string"
                              },
                              "namespace": {
                                "type": "string"
                              }
                            },
                            "required": \[
                              "value",
                              "namespace"
                            \]
                          }
                        },
                        "type": {
                          "type": "string"
                        },
                        "subType": {
                          "type": "string"
                        },
                        "publicationType": {
                          "type": "string"
                        }
                      },
                      "required": \[
                        "name"
                      \]
                    }
                  }
                }
              },
              "required": \[
                "platformTitleInstance"
              \]
            }
          }
        },
        "required": \[
          "source",
          "reference",
          "name"
        \]
      }
    }
  },
  "required": \[
    "header",
    "records"
  \]
}
</pre>
