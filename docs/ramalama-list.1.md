% ramalama-list 1

## NAME
ramalama\-list - List all AI models in local storage

## SYNOPSIS
**ramalama list** [*options*]

**ramalama ls** [*options*]

## DESCRIPTION
List all the AI Models in local storage

## OPTIONS

#### **--help**, **-h**
Print usage message

#### **--json**
Print model list in json format

#### **--noheading**, **-n**
Do not print heading

## EXAMPLE

List all models downloaded to users homedir
```
$ ramalama list
NAME                                                                MODIFIED     SIZE
ollama://tiny-llm:latest                                            16 hours ago 5.5M
huggingface://afrideva/Tiny-Vicuna-1B-GGUF/tiny-vicuna-1b.q2_k.gguf 14 hours ago 460M
ollama://granite-code:3b                                            5 days ago   1.9G
ollama://granite-code:latest                                        1 day ago    1.9G
ollama://moondream:latest                                           6 days ago   791M
```
List all models in json format
```
$ ramalama list --json
{"models": [{"name": "oci://quay.io/mmortari/gguf-py-example/v1/example.gguf", "modified": 427330, "size": "4.0K"}, {"name": "huggingface://afrideva/Tiny-Vicuna-1B-GGUF/tiny-vicuna-1b.q2_k.gguf", "modified": 427333, "size": "460M"}, {"name": "ollama://tiny-llm:latest", "modified": 420833, "size": "5.5M"}, {"name": "ollama://mistral:latest", "modified": 433998, "size": "3.9G"}, {"name": "ollama://granite-code:latest", "modified": 2180483, "size": "1.9G"}, {"name": "ollama://tinyllama:latest", "modified": 364870, "size": "609M"}, {"name": "ollama://tinyllama:1.1b", "modified": 364866, "size": "609M"}]}
```

## SEE ALSO
**[ramalama(1)](ramalama.1.md)**

## HISTORY
Aug 2024, Originally compiled by Dan Walsh <dwalsh@redhat.com>