# MMS Skin Example

In this repo you can find an example for the File adapter of [MMS](https://t.me/MoeMoeSecretaryEN)<br>
If you want a more detailed guide, follow [this](https://telegra.ph/Moe-Moe-Secretary-File-Adapter-Configuration-01-12)!

## Structure
- `base_folder`
  - `audios`
  - `skins`
  - `data.yaml`

## Example data.yaml
```yaml
dialogs:
  # This text will appear at the login
  - dialog: Welcome back!
    event: onLogin
    audio: ''
    
  # This text will appear when you click on the character
  # In this case we also have an audio
  - dialog: Nepu!?
    event: onClick
    audio: 'audios/nepu.mp3'
    
  # This text will appear if you don't interact with the character for a certain number of seconds (see dialogs.idle.frequency)
  - dialog: Hmmm hello?
    event: onIdle
    audio: ''

skins:
  - skins/Neptune.png
  # You can set more skins
```
