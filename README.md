# ReversoTTS component for HomeAssistant

The `ReversoTTS` text-to-speech platform uses online Reverso Text-to-Speech engine to read a text with natural sounding voices.

## Configuration

To enable text-to-speech with Reverso , add the following lines to your `configuration.yaml`:

```yaml
# Example configuration.yaml entry
tts:
  - platform: reversotts
```

### CONFIGURATION VARIABLES

 - **language**:
        description: The language to use. Supported languages are ."
        required: `false`
        type: `string`
        default: "`en-US`"
- **pitch(speed)**:
	description: The speak speed. Supported speed are `10-100`
    required: `false`
    type: `string`
    default: "`100`"
- **bitrate**:
    description: The bitrate for sound quailty . Supported bitrate are `22k, 96k, 128, 192k, 320k`
    required: `false`
    type: `string`
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
