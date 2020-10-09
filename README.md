[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs)
# ReversoTTS component for HomeAssistant

The `ReversoTTS` text-to-speech platform uses online Reverso Text-to-Speech engine to read a text with natural sounding voices.

## Installation

First download all files in folder https://github.com/rt400/ReversoTTS-HA/tree/master/custom_components/reversotts .
Now you need to create folder "reversotts" in your HomeAssistant config/custom_components folder and copy all files that you already download.
So after that you need to see like this example :

![GitHub Logo](/images/folders.png)


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
The language to use. Supported languages are in this table , please use only the name from **LangCode** column:

| LangCode | Voice | Gender | Language |
| ------------- | ------------- | ------------- | ------------- |
| Leila-Arabic | Leila22k | Female | Arabic |
| Mehdi-Arabic | Mehdi22k | Male | Arabic |
| Nizar-Arabic | Nizar22k | Male | Arabic |
| Salma-Arabic | Salma22k | Female | Arabic |
| Lisa-Australian-English | Lisa22k | Female | Australian English |
| Tyler-Australian-English | Tyler22k | Male | Australian English |
| Jeroen-Belgian-Dutch | Jeroen22k | Male | Belgian Dutch |
| Sofie-Belgian-Dutch | Sofie22k | Female | Belgian Dutch |
| Zoe-Belgian-Dutch | Zoe22k | Female | Belgian Dutch |
| Alice-BE-Belgian-French | Alice-BE22k | Female | Belgian French |
| Anais-BE-Belgian-French | Anais-BE22k | Female | Belgian French |
| Antoine-BE-Belgian-French | Antoine-BE22k | Male | Belgian French |
| Bruno-BE-Belgian-French | Bruno-BE22k | Male | Belgian French |
| Claire-BE-Belgian-French | Claire-BE22k | Female | Belgian French |
| Julie-BE-Belgian-French | Julie-BE22k | Female | Belgian French |
| Justine-Belgian-French | Justine22k | Female | Belgian French |
| Manon-BE-Belgian-French | Manon-BE22k | Female | Belgian French |
| Margaux-BE-Belgian-French | Margaux-BE22k | Female | Belgian French |
| Marcia-Brazilian | Marcia22k | Female | Brazilian |
| Graham-British | Graham22k | Male | British |
| Lucy-British | Lucy22k | Female | British |
| Peter-British | Peter22k | Male | British |
| QueenElizabeth-British | QueenElizabeth22k | Female | British |
| Rachel-British | Rachel22k | Female | British |
| Louise-Canadian-French | Louise22k | Female | Canadian French |
| Laia-Catalan | Laia22k | Female | Catalan |
| Eliska-Czech | Eliska22k | Female | Czech |
| Mette-Danish | Mette22k | Female | Danish |
| Rasmus-Danish | Rasmus22k | Male | Danish |
| Daan-Dutch | Daan22k | Male | Dutch |
| Femke-Dutch | Femke22k | Female | Dutch |
| Jasmijn-Dutch | Jasmijn22k | Female | Dutch |
| Max-Dutch | Max22k | Male | Dutch |
| Samuel-Finland-Swedish | Samuel22k | Male | Finland Swedish |
| Sanna-Finnish | Sanna22k | Female | Finnish |
| Alice-French | Alice22k | Female | French |
| Anais-French | Anais22k | Female | French |
| Antoine-French | Antoine22k | Male | French |
| Bruno-French | Bruno22k | Male | French |
| Claire-French | Claire22k | Female | French |
| Julie-French | Julie22k | Female | French |
| Manon-French | Manon22k | Female | French |
| Margaux-French | Margaux22k | Female | French |
| Andreas-German | Andreas22k | Male | German |
| Claudia-German | Claudia22k | Female | German |
| Julia-German | Julia22k | Female | German |
| Klaus-German | Klaus22k | Male | German |
| Sarah-German | Sarah22k | Female | German |
| Kal-Gothenburg-Swedish | Kal22k | Male | Gothenburg Swedish |
| Dimitris-Greek | Dimitris22k | Male | Greek |
| he-IL-Asaf-Hebrew | he-IL-Asaf | Male | Hebrew |
| Deepa-Indian-English | Deepa22k | Female | Indian English |
| Chiara-Italian | Chiara22k | Female | Italian |
| Fabiana-Italian | Fabiana22k | Female | Italian |
| Vittorio-Italian | Vittorio22k | Male | Italian |
| Sakura-Japanese | Sakura22k | Female | Japanese |
| Minji-Korean | Minji22k | Female | Korean |
| Lulu-Mandarin-Chinese | Lulu22k | Female | Mandarin Chinese |
| Bente-Norwegian | Bente22k | Female | Norwegian |
| Kari-Norwegian | Kari22k | Female | Norwegian |
| Olav-Norwegian | Olav22k | Male | Norwegian |
| Ania-Polish | Ania22k | Female | Polish |
| Monika-Polish | Monika22k | Female | Polish |
| Celia-Portuguese | Celia22k | Female | Portuguese |
| ro-RO-Andrei-Romanian | ro-RO-Andrei | Male | Romanian |
| Alyona-Russian | Alyona22k | Female | Russian |
| Mia-Scanian | Mia22k | Female | Scanian |
| Antonio-Spanish | Antonio22k | Male | Spanish |
| Ines-Spanish | Ines22k | Female | Spanish |
| Maria-Spanish | Maria22k | Female | Spanish |
| Elin-Swedish | Elin22k | Female | Swedish |
| Emil-Swedish | Emil22k | Male | Swedish |
| Emma-Swedish | Emma22k | Female | Swedish |
| Erik-Swedish | Erik22k | Male | Swedish |
| Ipek-Turkish | Ipek22k | Female | Turkish |
| Heather-US-English | Heather22k | Female | US English |
| Karen-US-English | Karen22k | Female | US English |
| Kenny-US-English | Kenny22k | Male | US English |
| Laura-US-English | Laura22k | Female | US English |
| Micah-US-English | Micah22k | Male | US English |
| Nelly-US-English | Nelly22k | Female | US English |
| Rod-US-English | Rod22k | Male | US English |
| Ryan-US-English | Ryan22k | Male | US English |
| Saul-US-English | Saul22k | Male | US English |
| Sharon-US-English | Sharon22k | Female | US English |
| Tracy-US-English | Tracy22k | Female | US English |
| Will-US-English | Will22k | Male | US English |
| Rodrigo-US-Spanish | Rodrigo22k | Male | US Spanish |
| Rosa-US-Spanish | Rosa22k | Female | US Spanish |


default: "`Sharon-US-English`"

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

## Examples of how to use

There are several ways how to use TTS service.

* Through call a service in HomeAssistant Developer Tools, in this example i used with Google Home Mini Speaker:

  ![GitHub Logo](/images/service_small.png)
  
* Through Automation in HomeAssistant , in this example i send to my Google HomeMini a meesage :

  ```
  - id: Test Message
    alias: Test Message
    initial_state: 'on'
    trigger:
    - platform: state
      entity_id: input_boolean.test
      from: 'off'
      to: 'on'
    condition:
    action:
    - data:
        message: "This is a Test For GitHub Readme"
      service: tts.reversotts_say
      entity_id: media_player.google_home_mini_salon 
  ```
  
  **Good Luck !**
