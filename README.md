# ReversoTTS component for HomeAssistant

The `ReversoTTS` text-to-speech platform uses online Reverso Text-to-Speech engine to read a text with natural sounding voices.

## Configuration

To enable text-to-speech with Reverso , add the following lines to your `configuration.yaml`:

```yaml
# Example configuration.yaml entry
tts:
  - platform: reversotts
```

### Configuration Optinal Variables

```yaml
 language: "he-IL-Asaf-Hebrew"
```
The language to use. Supported languages are

default: "`en-US`"

```yaml
 pitch: "100"
```

The speak speed. Supported speed are `10-100`, 100 is normal speak.

default: "`100`"

```yaml
 bitrate: "128k"
```

The bitrate for sound quailty . Supported bitrate are `22k, 96k, 128, 192k, 320k`

default: "`128k`"

## Full configuration example

The configuration sample below shows how an entry can look like:

```yaml
# Example configuration.yaml entry
tts:
  - platform: reversotts
    language: 'he-IL-Asaf-Hebrew'
    pitch: "100"
    bitrate: "128k"
```
